# 示例三：配置云服务器高可用的虚拟IP功能<a name="vpc_apieg_0004"></a>

## 操作场景<a name="section138381652181710"></a>

虚拟IP主要用在弹性云服务器的主备切换，达到高可用性的目的。当主服务器发生故障无法对外提供服务时，动态将虚拟IP切换到备服务器，继续对外提供服务。

本章节指导用户通过调用一系列虚拟IP相关API，使应用具备高可用性。

## 前提条件<a name="section109541355172116"></a>

-   已创建VPC和子网，并获取VPC和子网的ID，具体请参见[创建VPC和子网](https://support.huaweicloud.com/api-cce/cce_02_0100.html)。
-   已创建弹性云服务器，具体请参见[创建ECS](https://support.huaweicloud.com/qs-ecs/ecs_02_0009.html)。
-   当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。Token认证，具体操作请参考[认证鉴权](认证鉴权.md)。

>![](public_sys-resources/icon-note.gif) **说明：**   
>通过IAM服务获取到的Token有效期为24小时，需要使用同一个Token鉴权时，可以先将Token缓存，避免频繁调用。  

## 操作步骤<a name="section7856948"></a>

1.  创建虚拟IP。
    1.  发送“POST  https://VPC的Endpoint/v2.0/ports”。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下，其中vip所在子网需与ECS同子网。

        ```
        {
        	"port": {
        		"network_id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
        		"device_owner": "neutron:VIP_PORT",
        		"name": "vip_port_test"
        	}
        }
        ```

        或者如下，可以指定IP创建：

        ```
        {
        	"port": {
        		"network_id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
        		"device_owner": "neutron:VIP_PORT",
        		"name": "vip_port_test",
        		"fixed_ips": [
        			{
        				"ip_address": "192.168.0.220"
        			}
        		]
        	}
        }
        ```

    4.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            {
            	"port": {
            		"id": "a7d98f3c-b42f-460b-96a1-07601e145961",
            		"name": "port-test",
            		"status": "DOWN",
            		"admin_state_up": true,
            		"fixed_ips": [{
            			"subnet_id": "213cb9d-3122-2ac1-1a29-91ffc1231a12",
            			"ip_address": "192.168.0.220"
            		}],
            		"mac_address": "fa:16:3e:01:f7:90",
            		"network_id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
            		"tenant_id": "db82c9e1415a464ea68048baa8acc6b8",
            		"project_id": "db82c9e1415a464ea68048baa8acc6b8",
            		"device_id": "",
            		"device_owner": "neutron:VIP_PORT",
            		"security_groups": ["d0d58aa9-cda9-414c-9c52-6c3daf8534e6"],
            		"extra_dhcp_opts": [],
            		"allowed_address_pairs": [],
            		"binding:vnic_type": "normal",
            		"binding:vif_details": {},
            		"binding:profile": {},
            		"port_security_enabled": true,
            		"created_at": "2018-09-20T01:45:26",
            		"updated_at": "2018-09-20T01:45:26"
            	}
            }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。

2.  <a name="li293133115119"></a>通过云服务器的ID查询网卡信息。
    1.  发送“GET  https://VPC的Endpoint/v2.0/ports?device\_id=\{ecs\_id\}&network\_id=\{network\_id\}”
    2.  在Request Header中增加“X-Auth-Token”。
    3.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            {
            	"ports": [{
            		"id": "02c72193-efec-42fb-853b-c33f2b802467",
            		"name": "",
            		"status": "ACTIVE",
            		"admin_state_up": true,
            		"fixed_ips": [{
            			"subnet_id": "213cb9d-3122-2ac1-1a29-91ffc1231a12",
            			"ip_address": "192.168.0.75"
            		}],
            		"mac_address": "fa:16:3e:47:5f:c1",
            		"network_id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
            		"tenant_id": "db82c9e1415a464ea68048baa8acc6b8",
            		"project_id": "db82c9e1415a464ea68048baa8acc6b8",
            		"device_id": "ea61f836-b52f-41bf-9d06-685644001d6f",
            		"device_owner": "compute:br-iaas-odin1a",
            		"security_groups": [
            			"e0598d96-9451-4f8a-8de0-b8b4d451d9e7"
            		],
            		"extra_dhcp_opts": [],
            		"allowed_address_pairs": [],
            		"binding:vnic_type": "normal",
            		"binding:vif_details": {
            			"primary_interface": true
            		},
            		"binding:profile": {},
            		"port_security_enabled": true,
            		"created_at": "2020-06-20T08:07:29",
            		"updated_at": "2020-06-20T08:07:29"
            	}]
            }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。

3.  将云服务器与虚拟IP绑定。
    1.  发送“PUT  https://VPC的Endpoint/v2.0/ports/\{port\_id\}”。port\_id为上面创建的虚拟IP对应的port\_id。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下，ip\_address为[2](#li293133115119)查询出的云服务器的网卡ip。

        ```
        {
        	"port": {
        		"allowed_address_pairs": [{
        			"ip_address": "192.168.0.75"
        		}]
        	}
        }
        ```

    4.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            {
            	"port": {
            		"id": "a7d98f3c-b42f-460b-96a1-07601e145961",
            		"name": "port-test",
            		"status": "DOWN",
            		"admin_state_up": true,
            		"fixed_ips": [{
            			"subnet_id": "213cb9d-3122-2ac1-1a29-91ffc1231a12",
            			"ip_address": "192.168.0.220"
            		}],
            		"mac_address": "fa:16:3e:01:f7:90",
            		"network_id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
            		"tenant_id": "db82c9e1415a464ea68048baa8acc6b8",
            		"project_id": "db82c9e1415a464ea68048baa8acc6b8",
            		"device_id": "",
            		"device_owner": "neutron:VIP_PORT",
            		"security_groups": ["d0d58aa9-cda9-414c-9c52-6c3daf8534e6"],
            		"extra_dhcp_opts": [],
            		"allowed_address_pairs": [{
            			"ip_address": "192.168.0.75"
            		}]
            		"binding:vnic_type": "normal",
            		"binding:vif_details": {},
            		"binding:profile": {},
            		"port_security_enabled": true,
            		"created_at": "2018-09-20T01:45:26",
            		"updated_at": "2018-09-20T01:45:26"
            	}
            }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。

4.  关闭云服务器网卡的源/目的检查。
    1.  发送“PUT  https://VPC的Endpoint/v2.0/ports/\{port\_id\}”。port\_id为[2](#li293133115119)查询到的网卡ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下：ip\_address为[2](#li293133115119)查询出的云服务器的网卡ip。

        ```
        {
        	"port": {
        		"allowed_address_pairs": [{
        			"ip_address": "1.1.1.1/0"
        		}]
        	}
        }
        ```

    4.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            {
            	"port": {
            		"id": "02c72193-efec-42fb-853b-c33f2b802467",
            		"name": "",
            		"status": "ACTIVE",
            		"admin_state_up": true,
            		"fixed_ips": [{
            			"subnet_id": "213cb9d-3122-2ac1-1a29-91ffc1231a12",
            			"ip_address": "192.168.0.75"
            		}],
            		"mac_address": "fa:16:3e:47:5f:c1",
            		"network_id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
            		"tenant_id": "db82c9e1415a464ea68048baa8acc6b8",
            		"project_id": "db82c9e1415a464ea68048baa8acc6b8",
            		"device_id": "ea61f836-b52f-41bf-9d06-685644001d6f",
            		"device_owner": "compute:br-iaas-odin1a",
            		"security_groups": ["e0598d96-9451-4f8a-8de0-b8b4d451d9e7"],
            		"extra_dhcp_opts": [],
            		"allowed_address_pairs": [{
            			"ip_address": "1.1.1.1/0"
            		}],
            		"binding:vnic_type": "normal",
            		"binding:vif_details": {
            			"primary_interface": true
            		},
            		"binding:profile": {},
            		"port_security_enabled": true,
            		"created_at": "2020-06-20T08:07:29",
            		"updated_at": "2020-06-20T08:07:29"
            	}
            }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。



