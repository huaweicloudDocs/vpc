# 示例一：创建云服务器所需要的VPC和子网<a name="vpc_apieg_0002"></a>

## 操作场景<a name="section138381652181710"></a>

本章节指导用户通过调用API来创建云服务器所需要的VPC和子网。

## 前提条件<a name="section109541355172116"></a>

您需要规划VPC所在的区域信息，并根据区域确定调用API的Endpoint，详细信息请参见[终端节点](终端节点.md)。

当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。Token认证，具体操作请参考[认证鉴权](认证鉴权.md)。

>![](public_sys-resources/icon-note.gif) **说明：**   
>通过IAM服务获取到的Token有效期为24小时，需要使用同一个Token鉴权时，可以先将Token缓存，避免频繁调用。  

## 操作步骤<a name="section7856948"></a>

1.  创建VPC。
    1.  发送“POST  https://VPC的Endpoint/v1/\{project\_id\}/vpcs”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下，其中cidr字段需要提前进行网络规划。

        ```
        {
            "vpc": {
                "name": "vpc", //虚拟私有云名称
                "cidr": "192.168.0.0/16" //虚拟私有云下可用子网的范围
            }
        }
        ```

    4.  查看请求响应结果。
        -   请求成功时，响应参数如下，id就是vpc\_id。

            ```
            {
                "vpc": {
                    "id": "b6684a27-b049-407d-90b4-c9551f2390e1",
                    "name": "vpc",
                    "cidr": "192.168.0.0/16",
                    "status": "CREATING",
                    "routes": []
                }
            }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。



1.  查询VPC详情。
    1.  发送“GET  https://VPC的Endpoint/v1/\{project\_id\}/vpcs/\{vpc\_id\}”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  查看请求响应结果。
        -   请求成功时，响应参数如下，id就是vpc\_id。

            ```
            {
                "vpc": {
                    "id": "b6684a27-b049-407d-90b4-c9551f2390e1",
                    "name": "vpc",
                    "description": "",
                    "cidr": "192.168.0.0/16",
                    "status": "OK",
                    "enterprise_project_id": "0" ,
                    "routes": []
                }
            }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。

2.  指定VPC创建子网。
    1.  发送“POST  https://VPC的Endpoint/v1/\{project\_id\}/subnets”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下，其中dnsList参数参见[华为云提供的内网DNS地址是多少？](https://support.huaweicloud.com/dns_faq/dns_faq_002.html)，availability\_zone参数可通过[地区和终端节点](https://developer.huaweicloud.com/endpoint?VPC)获取。

        ```
        {
        	"subnet": {
        		"name": "subnet",
        		"description": "",
        		"cidr": "192.168.0.0/24",
        		"gateway_ip": "192.168.0.1",
        		"dhcp_enable": true,
        		"dnsList": ["114.xx.xx.114", "114.xx.xx.115"],
        		"availability_zone": "aa-bb-cc",
        		"vpc_id": "b6684a27-b049-407d-90b4-c9551f2390e1"
        	}
        }
        ```

    4.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            {
            	"subnet": {
            		"id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
            		"name": "subnet",
            		"description": "",
            		"cidr": "192.168.0.0/24",
            		"dnsList": ["114.xx.xx.114", "1114.xx.xx.115"],
            		"status": "UNKNOWN",
            		"vpc_id": "b6684a27-b049-407d-90b4-c9551f2390e1",
            		"gateway_ip": "192.168.0.1",
            		"dhcp_enable": true,
            		"primary_dns": "114.xx.xx.114",
            		"secondary_dns": "114.xx.xx.115",
            		"availability_zone": "aa-bb-cc",
            		"neutron_network_id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
            		"neutron_subnet_id": "213cb9d-3122-2ac1-1a29-91ffc1231a12",
            		"extra_dhcp_opts": []
            	}
            }
            ```

        -   请求异常时，错误码请参见[错误码](错误码.md)。



1.  查询子网详情。
    1.  发送“GET  https://VPC的Endpoint/v1/\{project\_id\}/subnets/\{subnet\_id\}”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  查看请求响应结果。

        ```
        {
        	"subnet": {
        		"id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
        		"name": "subnet",
        		"description": "",
        		"cidr": "192.168.20.0/24",
        		"dnsList": ["114.xx.xx.114", "114.xx.xx.115"],
        		"status": "ACTIVE",
        		"vpc_id": "b6684a27-b049-407d-90b4-c9551f2390e1",
        		"gateway_ip": "192.168.20.1",
        		"ipv6_enable": false,
        		"dhcp_enable": true,
        		"primary_dns": "114.xx.xx.114",
        		"secondary_dns": "114.xx.xx.115",
        		"availability_zone": "aa-bb-cc",
        		"neutron_network_id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d",
        		"neutron_subnet_id": "213cb9d-3122-2ac1-1a29-91ffc1231a12",
        		"extra_dhcp_opts": []
        	}
        }
        ```



