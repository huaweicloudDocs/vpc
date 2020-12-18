# 示例四：配置云服务器高可用的IPv6虚拟IP功能<a name="vpc_apieg_0006"></a>

## 操作场景<a name="section138381652181710"></a>

虚拟IP主要用在弹性云服务器的主备切换，达到高可用性的目的。当主服务器发生故障无法对外提供服务时，动态将虚拟IP切换到备服务器，继续对外提供服务。

本章节指导用户通过调用一系列IPv6虚拟IP相关API，使应用具备高可用性。

## 前提条件<a name="section109541355172116"></a>

-   已创建VPC和IPv6双栈子网，并获取VPC和子网的ID，具体请参见[创建VPC和子网](https://support.huaweicloud.com/api-cce/cce_02_0100.html)。
-   已创建弹性云服务器，具体请参见[创建ECS](https://support.huaweicloud.com/qs-ecs/ecs_02_0009.html)。
-   当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。Token认证，具体操作请参考[认证鉴权](认证鉴权.md)。

>![](public_sys-resources/icon-note.gif) **说明：** 
>通过IAM服务获取到的Token有效期为24小时，需要使用同一个Token鉴权时，可以先将Token缓存，避免频繁调用。

## 操作步骤<a name="section7856948"></a>

1.  创建IPv6虚拟IP。
    1.  发送“POST  https://VPC的Endpoint/v2.0/ports”。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下，其中vip所在子网需与ECS同子网，subnet\_id需要指定为IPv6的subnets对应ID。

        ```
        {
            "port":{
                "network_id":"b0ad9b80-bb16-4550-8ce0-514f949e35ee",
                "device_owner":"neutron:VIP_PORT",
                "name":"ipv6_vip_port_test",
                "fixed_ips":[
                    {
                        "subnet_id":"33ce2628-6246-4e3a-859f-99cd753ff704"
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
                    "id": "d92cfee7-9ebe-4483-85c1-00ffb1e45cd8",
                    "name": "ipv6_vip_port_test",
                    "status": "DOWN",
                    "admin_state_up": true,
                    "fixed_ips": [
                        {
                            "subnet_id": "33ce2628-6246-4e3a-859f-99cd753ff704",
                            "ip_address": "2001:db8:a583:21d:2e25:9403:6f3d:4664"
                        }
                    ],
                    "mac_address": "fa:16:3e:99:2e:92",
                    "network_id": "b0ad9b80-bb16-4550-8ce0-514f949e35ee",
                    "tenant_id": "060576782980d5762f9ec014dd2f1148",
                    "project_id": "060576782980d5762f9ec014dd2f1148",
                    "device_id": "",
                    "device_owner": "neutron:VIP_PORT",
                    "security_groups": [],
                    "extra_dhcp_opts": [],
                    "allowed_address_pairs": [],
                    "binding:vnic_type": "normal",
                    "binding:vif_details": {},
                    "binding:profile": {},
                    "port_security_enabled": true,
                    "created_at": "2020-12-15T03:01:07",
                    "updated_at": "2020-12-15T03:01:07"
                }
            }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。


2.  <a name="li293133115119"></a>通过云服务器的ID查询网卡信息，fixed\_ips中存在IPv4地址和IPv6地址。
    1.  发送“GET  https://VPC的Endpoint/v2.0/ports?device\_id=\{ecs\_id\}&network\_id=\{network\_id\}”
    2.  在Request Header中增加“X-Auth-Token”。
    3.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            { 
                 "ports": [{
                        "id": "47b4cd46-cfe5-415d-957f-5068189dce94",
                        "name": "",
                        "status": "ACTIVE",
                        "admin_state_up": true,
                        "fixed_ips": [
                            {
                                "subnet_id": "0dd17989-1c23-4501-8dc1-40e4085f793f",
                                "ip_address": "172.16.0.191"
                            },
                            {
                                "subnet_id": "33ce2628-6246-4e3a-859f-99cd753ff704",
                                "ip_address": "2001:db8:a583:21d:dfc0:d452:e9ab:65cf"
                            }
                        ],
                        "mac_address": "fa:16:3e:1e:f7:9a",
                        "network_id": "b0ad9b80-bb16-4550-8ce0-514f949e35ee",
                        "tenant_id": "060576782980d5762f9ec014dd2f1148",
                        "project_id": "060576782980d5762f9ec014dd2f1148",
                        "device_id": "ab7ca781-66bf-48a8-814b-1568cb393a38",
                        "device_owner": "compute:xxx",
                        "security_groups": [
                            "0552091e-b83a-49dd-88a7-4a5c86fd9ec3"
                        ],
                        "extra_dhcp_opts": [],
                        "allowed_address_pairs": [],
                        "binding:vnic_type": "normal",
                        "binding:vif_details": {
                            "primary_interface": true
                        },
                        "binding:profile": {},
                        "port_security_enabled": true,
                        "dns_assignment": [
                            {
                                "hostname": "ip-172-16-0-191",
                                "ip_address": "172.16.0.191",
                                "fqdn": "ip-172-16-0-191.br-iaas-odin1.compute.internal."
                            }
                        ],
                        "dns_name": "ip-172-16-0-191",
                        "created_at": "2020-11-19T13:32:37",
                        "updated_at": "2020-11-19T13:33:50"
                    }] 
             }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。


3.  将云服务器与虚拟IP绑定。
    1.  发送“PUT  https://VPC的Endpoint/v2.0/ports/\{port\_id\}”。port\_id为上面创建的IPv6虚拟IP对应的port\_id。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下，ip\_address为[2](#li293133115119)查询出的云服务器的网卡的IPv6 ip。

        ```
        { 
             "port": { 
                 "allowed_address_pairs": [{ 
                     "ip_address": "2001:db8:a583:21d:dfc0:d452:e9ab:65cf" 
                 }] 
             } 
         }
        ```

    4.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            {
                "port": {
                    "id": "d92cfee7-9ebe-4483-85c1-00ffb1e45cd8",
                    "name": "ipv6_vip_port_test",
                    "status": "DOWN",
                    "admin_state_up": true,
                    "fixed_ips": [
                        {
                            "subnet_id": "33ce2628-6246-4e3a-859f-99cd753ff704",
                            "ip_address": "2001:db8:a583:21d:2e25:9403:6f3d:4664"
                        }
                    ],
                    "mac_address": "fa:16:3e:99:2e:92",
                    "network_id": "b0ad9b80-bb16-4550-8ce0-514f949e35ee",
                    "tenant_id": "060576782980d5762f9ec014dd2f1148",
                    "project_id": "060576782980d5762f9ec014dd2f1148",
                    "device_id": "",
                    "device_owner": "neutron:VIP_PORT",
                    "security_groups": [],
                    "extra_dhcp_opts": [],
                    "allowed_address_pairs": [{ 
                         "ip_address": "2001:db8:a583:21d:dfc0:d452:e9ab:65cf " 
                     }],
                    "binding:vnic_type": "normal",
                    "binding:vif_details": {},
                    "binding:profile": {},
                    "port_security_enabled": true,
                    "created_at": "2020-12-15T03:01:07",
                    "updated_at": "2020-12-15T03:01:07"
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
            "id": "47b4cd46-cfe5-415d-957f-5068189dce94",
                        "name": "",
                        "status": "ACTIVE",
                        "admin_state_up": true,
                        "fixed_ips": [
                            {
                                "subnet_id": "0dd17989-1c23-4501-8dc1-40e4085f793f",
                                "ip_address": "172.16.0.191"
                            },
                            {
                                "subnet_id": "33ce2628-6246-4e3a-859f-99cd753ff704",
                                "ip_address": "2001:db8:a583:21d:dfc0:d452:e9ab:65cf"
                            }
                        ],
                        "mac_address": "fa:16:3e:1e:f7:9a",
                        "network_id": "b0ad9b80-bb16-4550-8ce0-514f949e35ee",
                        "tenant_id": "060576782980d5762f9ec014dd2f1148",
                        "project_id": "060576782980d5762f9ec014dd2f1148",
                        "device_id": "ab7ca781-66bf-48a8-814b-1568cb393a38",
                        "device_owner": "compute:xxx",
                        "security_groups": [
                            "0552091e-b83a-49dd-88a7-4a5c86fd9ec3"
                        ],
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
                        "dns_assignment": [
                            {
                                "hostname": "ip-172-16-0-191",
                                "ip_address": "172.16.0.191",
                                "fqdn": "ip-172-16-0-191.br-iaas-odin1.compute.internal."
                            }
                        ],
                        "dns_name": "ip-172-16-0-191",
                        "created_at": "2020-11-19T13:32:37",
                        "updated_at": "2020-11-19T13:33:50"
            
                 } 
             }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。



