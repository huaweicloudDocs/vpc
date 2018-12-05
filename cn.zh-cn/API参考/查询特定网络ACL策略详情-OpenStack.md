# 查询特定网络ACL策略详情<a name="ZH-CN_TOPIC_0060574383"></a>

## 功能介绍<a name="section915947313242"></a>

查询特定网络ACL策略详情。

## URI<a name="section2518841213242"></a>

GET /v2.0/fwaas/firewall\_policies/\{firewall\_policy\_id\}

**表 1**  参数说明

<a name="table18880184689"></a>
<table><thead align="left"><tr id="row13968641385"><th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.2.5.1.1"><p id="p209684410817"><a name="p209684410817"></a><a name="p209684410817"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.2"><p id="p69681441386"><a name="p69681441386"></a><a name="p69681441386"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="27.27272727272727%" id="mcps1.2.5.1.3"><p id="p1096813412811"><a name="p1096813412811"></a><a name="p1096813412811"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.36363636363636%" id="mcps1.2.5.1.4"><p id="p139686416813"><a name="p139686416813"></a><a name="p139686416813"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19681041189"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1682422682817"><a name="p1682422682817"></a><a name="p1682422682817"></a>firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p1797015416817"><a name="p1797015416817"></a><a name="p1797015416817"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p19701411813"><a name="p19701411813"></a><a name="p19701411813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p109701641488"><a name="p109701641488"></a><a name="p109701641488"></a>网络ACL策略唯一标识，按照firewall_policy_id查询</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section5030939813242"></a>

无

## 响应消息<a name="section2488003713242"></a>

**表 2**  响应参数

<a name="table6694832013242"></a>
<table><thead align="left"><tr id="row6068200913242"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p963376713242"><a name="p963376713242"></a><a name="p963376713242"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.11%" id="mcps1.2.4.1.2"><p id="p303129213242"><a name="p303129213242"></a><a name="p303129213242"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.540000000000006%" id="mcps1.2.4.1.3"><p id="p1024114813242"><a name="p1024114813242"></a><a name="p1024114813242"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4115792613242"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p1605288813242"><a name="p1605288813242"></a><a name="p1605288813242"></a>firewall_policy</p>
</td>
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p2885681613242"><a name="p2885681613242"></a><a name="p2885681613242"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p6121237313242"><a name="p6121237313242"></a><a name="p6121237313242"></a>firewall policy对象列表，参见<a href="网络ACL简介-OpenStack.md#table17002720121127">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section478525713242"></a>

请求样例

```
GET /v2.0/fwaas/firewall_policies/fed2d88f-d0e7-4cc5-bd7e-c495f67037b6
```

响应样例

```
{
    "firewall_policy": {
        "description": "", 
        "firewall_rules": [
            "3c0e6267-73df-4d9a-87a6-e226f2db2036"
        ], 
        "tenant_id": "23c8a121505047b6869edf39f3062712", 
        "public": false, 
        "id": "fed2d88f-d0e7-4cc5-bd7e-c495f67037b6", 
        "audited": false, 
        "name": "bobby_fwp1",
        "project_id": "23c8a121505047b6869edf39f3062712"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

