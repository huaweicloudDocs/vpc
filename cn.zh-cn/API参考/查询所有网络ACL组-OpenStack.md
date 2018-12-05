# 查询所有网络ACL组<a name="ZH-CN_TOPIC_0060574389"></a>

## 功能介绍<a name="section11380465132652"></a>

查询提交请求的租户有权限操作的所有网络ACL组信息。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section38164372132652"></a>

GET /v2.0/fwaas/firewall\_groups

## 请求消息<a name="section30244758132652"></a>

无。

## 响应消息<a name="section48852885132652"></a>

**表 1**  响应参数

<a name="table25605667132652"></a>
<table><thead align="left"><tr id="row26621002132652"><th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.1"><p id="p17188156132652"><a name="p17188156132652"></a><a name="p17188156132652"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.78%" id="mcps1.2.4.1.2"><p id="p29579284132652"><a name="p29579284132652"></a><a name="p29579284132652"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.89%" id="mcps1.2.4.1.3"><p id="p37495801132652"><a name="p37495801132652"></a><a name="p37495801132652"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row29258567132652"><td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.1 "><p id="p7598331132652"><a name="p7598331132652"></a><a name="p7598331132652"></a>firewall_groups</p>
</td>
<td class="cellrowborder" valign="top" width="17.78%" headers="mcps1.2.4.1.2 "><p id="p50785846132652"><a name="p50785846132652"></a><a name="p50785846132652"></a>List(firewall group)</p>
</td>
<td class="cellrowborder" valign="top" width="58.89%" headers="mcps1.2.4.1.3 "><p id="p48871362132652"><a name="p48871362132652"></a><a name="p48871362132652"></a>firewall group对象列表，参见<a href="网络ACL简介-OpenStack.md#table31629250121127">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section19537091132652"></a>

请求样例

```
GET /v2.0/fwaas/firewall_groups
```

响应样例

```
{
    "firewall_groups": [
        {
            "status": "INACTIVE", 
            "public": false, 
            "egress_firewall_policy_id": null, 
            "name": "", 
            "admin_state_up": true, 
            "ports": [ ], 
            "tenant_id": "23c8a121505047b6869edf39f3062712", 
            "id": "cd600d47-0045-483f-87a1-5041ae2f513b", 
            "ingress_firewall_policy_id": null, 
            "description": "",
            "project_id": "23c8a121505047b6869edf39f3062712"
        }, 
        {
            "status": "INACTIVE", 
            "public": false, 
            "egress_firewall_policy_id": "d939df29-fe76-4089-90c3-3778e4d53141", 
            "name": "fwg-1475475043", 
            "admin_state_up": true, 
            "ports": [ ], 
            "tenant_id": "0af57070695044ea9a70f04779e6aa1f", 
            "id": "ca971b45-70ce-4879-9734-b6cac1d00845", 
            "ingress_firewall_policy_id": "d939df29-fe76-4089-90c3-3778e4d53141", 
            "description": "",
            "project_id": "0af57070695044ea9a70f04779e6aa1f"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

