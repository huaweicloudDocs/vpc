# 创建网络ACL策略<a name="ZH-CN_TOPIC_0060574384"></a>

## 功能介绍<a name="section1113556013250"></a>

创建网络ACL策略。

## URI<a name="section6172185713250"></a>

POST /v2.0/fwaas/firewall\_policies

## 请求消息<a name="section1463374013250"></a>

**表 1**  请求参数

<a name="table2714868513250"></a>
<table><thead align="left"><tr id="row1539465113250"><th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.1"><p id="p1243776013250"><a name="p1243776013250"></a><a name="p1243776013250"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p3819060413250"><a name="p3819060413250"></a><a name="p3819060413250"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p4282563113250"><a name="p4282563113250"></a><a name="p4282563113250"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p3747093813250"><a name="p3747093813250"></a><a name="p3747093813250"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4731925913250"><td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.1 "><p id="p3852256313250"><a name="p3852256313250"></a><a name="p3852256313250"></a>firewall_policy</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p5375326713250"><a name="p5375326713250"></a><a name="p5375326713250"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p5311559313250"><a name="p5311559313250"></a><a name="p5311559313250"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p3083242213250"><a name="p3083242213250"></a><a name="p3083242213250"></a>firewall policy对象列表，参见<a href="网络ACL简介-OpenStack.md#table17002720121127">表2</a>。</p>
<p id="p6151169713250"><a name="p6151169713250"></a><a name="p6151169713250"></a>必选字段：无</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section3860887413250"></a>

**表 2**  响应参数

<a name="table1500933413250"></a>
<table><thead align="left"><tr id="row4729303413250"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p3920364913250"><a name="p3920364913250"></a><a name="p3920364913250"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p2638548713250"><a name="p2638548713250"></a><a name="p2638548713250"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p3350107113250"><a name="p3350107113250"></a><a name="p3350107113250"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2328883413250"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p1575454013250"><a name="p1575454013250"></a><a name="p1575454013250"></a>firewall_policy</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p4446263713250"><a name="p4446263713250"></a><a name="p4446263713250"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p4558033913250"><a name="p4558033913250"></a><a name="p4558033913250"></a>firewall policy对象列表，参见<a href="网络ACL简介-OpenStack.md#table17002720121127">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section5030474113250"></a>

请求样例

```
POST /v2.0/fwaas/firewall_policies
{
    "firewall_policy": {
        "name": "test-policy", 
        "firewall_rules": [
            "b8243448-cb3c-496e-851c-dadade4c161b"
        ]
    }
}
```

响应样例

```
{
    "firewall_policy": {
        "description": "", 
        "firewall_rules": [
            "b8243448-cb3c-496e-851c-dadade4c161b"
        ], 
        "tenant_id": "23c8a121505047b6869edf39f3062712", 
        "public": false, 
        "id": "2fb0e81f-9f63-44b2-9894-c13a3284594a", 
        "audited": false, 
        "name": "test-policy",
        "project_id": "23c8a121505047b6869edf39f3062712"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

