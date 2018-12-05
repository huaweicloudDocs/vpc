# 查询端口列表<a name="ZH-CN_TOPIC_0062207806"></a>

## 功能介绍<a name="zh-cn_topic_0062207386_section66569185"></a>

查询提交请求的租户的所有端口，单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="zh-cn_topic_0062207386_section62251757"></a>

GET /v2.0/ports

样例：

```
/v2.0/ports?id={port_id}&name={port_name}&admin_state_up={is_admin_status_up}&network_id={network_id}&mac_address={port_mac}&device_id={port_device_id}&device_owner={device_owner}&tenant_id={tenant_id}&status={port_status}&fixed_ips=ip_address={ip_address}&fixed_ips=subnet_id={subnet_id}&dns_name={dns_name}
```

## 请求消息<a name="zh-cn_topic_0062207386_section15938858"></a>

无

## 响应参数<a name="zh-cn_topic_0062207386_section9232000"></a>

**表 1**  响应参数

<a name="zh-cn_topic_0062207386_table48620262"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207386_row18332862"><th class="cellrowborder" valign="top" width="22.32%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207386_p8566882"><a name="zh-cn_topic_0062207386_p8566882"></a><a name="zh-cn_topic_0062207386_p8566882"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="24.67%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207386_p22828842"><a name="zh-cn_topic_0062207386_p22828842"></a><a name="zh-cn_topic_0062207386_p22828842"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.010000000000005%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207386_p60161096"><a name="zh-cn_topic_0062207386_p60161096"></a><a name="zh-cn_topic_0062207386_p60161096"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207386_row41210606"><td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207386_p49724760"><a name="zh-cn_topic_0062207386_p49724760"></a><a name="zh-cn_topic_0062207386_p49724760"></a>ports</p>
</td>
<td class="cellrowborder" valign="top" width="24.67%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207386_p1173742"><a name="zh-cn_topic_0062207386_p1173742"></a><a name="zh-cn_topic_0062207386_p1173742"></a>List(port)</p>
</td>
<td class="cellrowborder" valign="top" width="53.010000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207386_p50516929"><a name="zh-cn_topic_0062207386_p50516929"></a><a name="zh-cn_topic_0062207386_p50516929"></a>port对象列表，参见<a href="端口API简介-OpenStack.md#table15919752145624">表1</a></p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0062207386_section15979144"></a>

【样例一】

-   JSON请求样例

    ```
    GET /v2.0/ports?limit=1
    ```

-   JSON响应样例

    ```
    {
     "ports": [{
           "id": "791870bd-36a7-4d9b-b015-a78e9b06af08",
           "name": "port-test",
           "status": "DOWN",
           "admin_state_up": true,
           "fixed_ips": [],
           "mac_address": "fa:16:3e:01:e0:b2",
           "network_id": "00ae08c5-f727-49ab-ad4b-b069398aa171",
           "tenant_id": "db82c9e1415a464ea68048baa8acc6b8",
           "project_id": "db82c9e1415a464ea68048baa8acc6b8",
           "device_id": "",
           "device_owner": "",
           "security_groups": [d0d58aa9-cda9-414c-9c52-6c3daf8534e6"],
           "extra_dhcp_opts": [],
           "allowed_address_pairs": [],
           "binding: vnic_type": "normal",
           "binding: vif_details": {},
           "binding: profile": {},
           "port_security_enabled": true,
           "created_at": "2018-09-13T01: 43: 41",
           "updated_at": "2018-09-13T01: 43: 41"
     }]
    }
    ```


【样例二】

-   JSON请求样例

    ```
    GET /v2.0/ports?mac_address=fa:16:3e:f1:0b:09
    ```


-   JSON响应样例

    ```
    {
        "ports": [
            {
                "admin_state_up": true,
                "allowed_address_pairs": [],
                "binding:vnic_type": "normal",
                "device_id": "e6c05704-c907-4cc1-8106-69b0996c43b9",
                "device_owner": "compute:az3.dc1",
                "port_security_enabled":true,
                "extra_dhcp_opts": [],
                "fixed_ips": [
                    {
                        "ip_address": "172.16.0.37",
                        "subnet_id": "b3ac1347-63f2-4e82-b853-3d86416a0db5"
                    }
                ],
                "dns_assignment": [
                    {
                        "hostname": "ip-172-16-0-37",
                        "ip_address": "172.16.0.37",
                        "fqdn": "ip-172-16-0-37.xxx.compute.internal."
                    }
                ],
                "dns_name": "ip-172-16-0-37",
                "id": "7bb64706-6e46-4f94-a28a-4bc7caaab87d",
                "mac_address": "fa:16:3e:f1:0b:09",
                "name": "port_vm_50_3",
                "network_id": "a54e1b19-ce78-4b7e-b28b-d2d716cdc161",
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ],
                "status": "ACTIVE",
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41"
            }
        ]
    }
    ```


【样例三】

-   JSON请求样例

    ```
    GET /v2.0/ports?admin_state_up=False
    ```


-   JSON响应样例

    ```
    {
        "ports": [
    
            {
                "admin_state_up": false, 
                "allowed_address_pairs": [], 
                "binding:vnic_type": "normal", 
                "device_id": "", 
                "device_owner": "", 
                "port_security_enabled":true,
                "extra_dhcp_opts": [], 
                "fixed_ips": [
                    {
                        "ip_address": "10.100.100.62", 
                        "subnet_id": "9b28f20c-0234-419f-a0b4-4a84f182f64b"
                    }
                ], 
                "dns_name": "",
                "id": "ffc0bdee-8413-4fa2-bd82-fa8efe5b3a87", 
                "mac_address": "fa:16:3e:2b:bc:57", 
                "name": "small_net_port", 
                "network_id": "b299b151-7a66-4c6f-a313-cdd3b5724296", 
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ], 
                "status": "DOWN", 
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41"
            }
        ]
    }
    ```


【样例四】

-   JSON请求样例

    ```
    GET /v2.0/ports?device_id=e6c05704-c907-4cc1-8106-69b0996c43b9
    ```


-   JSON响应样例

    ```
    {
        "ports": [
            {
                "admin_state_up": true, 
                "allowed_address_pairs": [], 
                "binding:vnic_type": "normal", 
                "device_id": "e6c05704-c907-4cc1-8106-69b0996c43b9", 
                "device_owner": "compute:az3.dc1", 
                "port_security_enabled":true,
                "extra_dhcp_opts": [], 
                "fixed_ips": [
                    {
                        "ip_address": "10.1.0.37", 
                        "subnet_id": "b3ac1347-63f2-4e82-b853-3d86416a0db5"
                    }
                ], 
                "dns_assignment": [
                    {
                        "hostname": "ip-10-1-0-37",
                        "ip_address": "10.1.0.37",
                        "fqdn": "ip-10-1-0-37.xxx.compute.internal."//xxx为区域名称。
                    }
                ],
                "dns_name": "ip-10-1-0-37",
                "id": "7bb64706-6e46-4f94-a28a-4bc7caaab87d", 
                "mac_address": "fa:16:3e:f1:0b:09", 
                "name": "port_vm_50_3", 
                "network_id": "a54e1b19-ce78-4b7e-b28b-d2d716cdc161", 
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ], 
                "status": "ACTIVE", 
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "6c9298ec8c874f7f99688489ab65f90e" ,
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41"
            }
        ]
    }
    ```


【样例五】

-   JSON请求样例

    ```
    GET /v2.0/ports?tenant_id=6c9298ec8c874f7f99688489ab65f90e&name=port_vm_50_3
    ```


-   JSON响应样例

    ```
    {
        "ports": [
            {
                "admin_state_up": true, 
                "allowed_address_pairs": [], 
                "binding:vnic_type": "normal", 
                "device_id": "e6c05704-c907-4cc1-8106-69b0996c43b9", 
                "device_owner": "compute:az3.dc1", 
                "port_secuirty_enabled":true,
                "extra_dhcp_opts": [], 
                "fixed_ips": [
                    {
                        "ip_address": "10.1.0.37", 
                        "subnet_id": "b3ac1347-63f2-4e82-b853-3d86416a0db5"
                    }
                ], 
                "dns_assignment": [
                    {
                        "hostname": "ip-10-1-0-37",
                        "ip_address": "10.1.0.37",
                        "fqdn": "ip-10-1-0-37.xxx.compute.internal."//xxx为区域名称。
                    }
                ],
                "dns_name": "ip-10-1-0-37",
                "id": "7bb64706-6e46-4f94-a28a-4bc7caaab87d", 
                "mac_address": "fa:16:3e:f1:0b:09", 
                "name": "port_vm_50_3", 
                "network_id": "a54e1b19-ce78-4b7e-b28b-d2d716cdc161", 
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ], 
                "status": "ACTIVE", 
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "6c9298ec8c874f7f99688489ab65f90e" ,
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41"
            }
        ]
    }
    ```


【样例六】

-   JSON请求样例

    ```
    GET /v2.0/ports?name=port_vm_50_3
    ```


-   JSON响应样例

    ```
    {
        "ports": [
            {
                "status": "DOWN",
                "allowed_address_pairs": [],
                "extra_dhcp_opts": [],
                "device_owner": "",
                "port_security_enabled":true,
                "fixed_ips": [
                    {
                        "subnet_id": "391c74f7-e3b1-405c-8473-2f71a0aec7dc",
                        "ip_address": "10.1.0.33"
                    }
                ],
                "dns_name": "",
                "id": "0f405555-739f-4a19-abb7-ec11d005b3a9",
                "security_groups": [
                    "043548bc-1020-4be0-885a-caac8530e8f6"
                ],
                "device_id": "",
                "port_security_enabled":true,
                "name": "port_vm_50_3",
                "admin_state_up": true,
                "network_id": "9898a82d-7795-4ad5-bf2c-0ed8b822be4f",
                "tenant_id": "3e4a1816927f405cacbc3dca1e05111e",
                "project_id": "3e4a1816927f405cacbc3dca1e05111e",
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41",
                "binding:vnic_type": "normal",
                "mac_address": "fa:16:3e:b0:d9:cf"
            },
            {
                "status": "ACTIVE",
                "allowed_address_pairs": [],
                "extra_dhcp_opts": [],
                "device_owner": "compute:az3.dc1",
                "port_security_enabled":true,
                "fixed_ips": [
                    {
                        "subnet_id": "b3ac1347-63f2-4e82-b853-3d86416a0db5",
                        "ip_address": "10.1.0.37"
                    }
                ],
                "dns_assignment": [
                    {
                        "hostname": "ip-10-1-0-37",
                        "ip_address": "10.1.0.37",
                        "fqdn": "ip-10-1-0-37.xxx.compute.internal."//xxx为区域名称。
                     }  
                ],
                "dns_name": "ip-10-1-0-37",
                "id": "7bb64706-6e46-4f94-a28a-4bc7caaab87d",
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ],
                "device_id": "e6c05704-c907-4cc1-8106-69b0996c43b9",
                "name": "port_vm_50_3",
                "admin_state_up": true,
                "network_id": "a54e1b19-ce78-4b7e-b28b-d2d716cdc161",
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "3e4a1816927f405cacbc3dca1e05111e",
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41",
                 "binding:vnic_type": "normal", 
                "binding:vnic_type": "normal",
                "mac_address": "fa:16:3e:f1:0b:09"
            }
        ]
    }
    ```


## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

