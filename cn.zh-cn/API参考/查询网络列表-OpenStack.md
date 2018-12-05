# 查询网络列表<a name="ZH-CN_TOPIC_0060495801"></a>

## 功能介绍<a name="section23215317204921"></a>

查询提交请求的租户的所有网络，单次查询最多返回2000条数据，超过2000后会返回分页标记分页。查询请参考[分页查询](分页查询.md)。

## URI<a name="section12532958204921"></a>

GET /v2.0/networks

样例：

```
/v2.0/networks?id={network_id}&status={network_status}&name={network_name}&admin_state_up={is_admin_status_up}&tenant_id={tenant_id}&shared={is_shared}&provider:network_type={geneve}
```

## 请求消息<a name="section24189635204921"></a>

无。

## 响应消息<a name="section51721924204921"></a>

**表 1**  响应参数

<a name="table28726301204921"></a>
<table><thead align="left"><tr id="row66095891204921"><th class="cellrowborder" valign="top" width="18.82%" id="mcps1.2.4.1.1"><p id="p52166951204921"><a name="p52166951204921"></a><a name="p52166951204921"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="24.709999999999997%" id="mcps1.2.4.1.2"><p id="p64773532204921"><a name="p64773532204921"></a><a name="p64773532204921"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.47%" id="mcps1.2.4.1.3"><p id="p45821640204921"><a name="p45821640204921"></a><a name="p45821640204921"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row20565326204921"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.2.4.1.1 "><p id="p55178709204921"><a name="p55178709204921"></a><a name="p55178709204921"></a>networks</p>
</td>
<td class="cellrowborder" valign="top" width="24.709999999999997%" headers="mcps1.2.4.1.2 "><p id="p40290436204921"><a name="p40290436204921"></a><a name="p40290436204921"></a>List（network）</p>
</td>
<td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.2.4.1.3 "><p id="p3740541204921"><a name="p3740541204921"></a><a name="p3740541204921"></a>network对象列表，参见<a href="网络API简介-OpenStack.md#table49902238182444">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section33664870204921"></a>

请求样例

```
GET /v2.0/networks?limit=1
```

响应样例

```
{
    "networks": [
        {
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
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

