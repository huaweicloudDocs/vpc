# 查询网络<a name="ZH-CN_TOPIC_0060495802"></a>

## 功能介绍<a name="section58515065204939"></a>

查询网络详情。

## URI<a name="section43354202204939"></a>

GET /v2.0/networks/\{network\_id\}

## 请求消息<a name="section29238419204939"></a>

无。

## 响应消息<a name="section41298168204939"></a>

**表 1**  响应参数

<a name="table56817282204939"></a>
<table><thead align="left"><tr id="row35431593204939"><th class="cellrowborder" valign="top" width="21.59%" id="mcps1.2.4.1.1"><p id="p51386807204939"><a name="p51386807204939"></a><a name="p51386807204939"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.63%" id="mcps1.2.4.1.2"><p id="p1581813204939"><a name="p1581813204939"></a><a name="p1581813204939"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="64.78%" id="mcps1.2.4.1.3"><p id="p43510562204939"><a name="p43510562204939"></a><a name="p43510562204939"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row34694625204939"><td class="cellrowborder" valign="top" width="21.59%" headers="mcps1.2.4.1.1 "><p id="p58801265204939"><a name="p58801265204939"></a><a name="p58801265204939"></a>network</p>
</td>
<td class="cellrowborder" valign="top" width="13.63%" headers="mcps1.2.4.1.2 "><p id="p65282042204939"><a name="p65282042204939"></a><a name="p65282042204939"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="64.78%" headers="mcps1.2.4.1.3 "><p id="p26708244204939"><a name="p26708244204939"></a><a name="p26708244204939"></a>network对象列表，参见<a href="网络API简介-OpenStack.md#table49902238182444">表1</a>。。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section39047607204939"></a>

请求样例

```
GET /v2.0/networks/0133cd73-34d4-4d4c-bf1f-e65b24603206
```

响应样例

```
{
    "network": {
        "id": "0133cd73-34d4-4d4c-bf1f-e65b24603206",
        "name": "3804f26c-7862-43b6-ad3c-48445f42de89",
        "status": "ACTIVE",
        "shared": false,
        "subnets": [
            "423796f5-e02f-476f-bf02-2b88c8ddac8b"
        ],
        "availability_zone_hints": [],
        "availability_zones": [
            "az2.dc2",
            "az5.dc5"
        ],
        "admin_state_up": true,
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "provider:network_type": "vxlan",
        "router:external": false,
        "port_security_enabled": true,
        "created_at": "2018-03-23T03:51:58",
        "updated_at": "2018-03-23T03:51:58"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

