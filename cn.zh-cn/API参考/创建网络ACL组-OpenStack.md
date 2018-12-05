# 创建网络ACL组<a name="ZH-CN_TOPIC_0060574391"></a>

## 功能介绍<a name="section28317954132753"></a>

创建网络ACL组。

## URI<a name="section55587849132753"></a>

POST /v2.0/fwaas/firewall\_groups

## 请求消息<a name="section28981251132753"></a>

**表 1**  请求参数

<a name="table23322114132753"></a>
<table><thead align="left"><tr id="row65935357132753"><th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.1"><p id="p47877448132753"><a name="p47877448132753"></a><a name="p47877448132753"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p52491337132753"><a name="p52491337132753"></a><a name="p52491337132753"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p45667362132753"><a name="p45667362132753"></a><a name="p45667362132753"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p17633266132753"><a name="p17633266132753"></a><a name="p17633266132753"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8939225132753"><td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.1 "><p id="p59896822132753"><a name="p59896822132753"></a><a name="p59896822132753"></a>firewall_group</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p49917547132753"><a name="p49917547132753"></a><a name="p49917547132753"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p64285015132753"><a name="p64285015132753"></a><a name="p64285015132753"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p48871362132652"><a name="p48871362132652"></a><a name="p48871362132652"></a>firewall group对象列表，参见<a href="网络ACL简介-OpenStack.md#table31629250121127">表3</a>。</p>
<p id="p59212630132753"><a name="p59212630132753"></a><a name="p59212630132753"></a>必选字段：无</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section47249684132753"></a>

**表 2**  响应参数

<a name="table22528036132753"></a>
<table><thead align="left"><tr id="row54420002132753"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p43836262132753"><a name="p43836262132753"></a><a name="p43836262132753"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p57315890132753"><a name="p57315890132753"></a><a name="p57315890132753"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p55101661132753"><a name="p55101661132753"></a><a name="p55101661132753"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row23789310132753"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p30981925132753"><a name="p30981925132753"></a><a name="p30981925132753"></a>firewall_group</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p1451635132753"><a name="p1451635132753"></a><a name="p1451635132753"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p47442693132753"><a name="p47442693132753"></a><a name="p47442693132753"></a>firewall group对象列表，参见<a href="网络ACL简介-OpenStack.md#table31629250121127">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section59424075132753"></a>

请求样例

```
POST /v2.0/fwaas/firewall_groups
{
    "firewall_group": {
        "ingress_firewall_policy_id": "afc52ce9-5305-4ec9-9feb-44feb8330341", 
        "ports": [
            "c133f2bf-6937-4416-bb17-012e1be5cd2d"
        ]
    }
}
```

响应样例

```
{
    "firewall_group": {
        "status": "PENDING_CREATE", 
        "public": false, 
        "egress_firewall_policy_id": null, 
        "name": "", 
        "admin_state_up": true, 
        "ports": [
            "c133f2bf-6937-4416-bb17-012e1be5cd2d"
        ], 
        "tenant_id": "23c8a121505047b6869edf39f3062712", 
        "id": "0415f554-26ed-44e7-a881-bdf4e6216e38", 
        "ingress_firewall_policy_id": "afc52ce9-5305-4ec9-9feb-44feb8330341", 
        "description": "",
        "project_id": "23c8a121505047b6869edf39f3062712"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

