# 更新网络ACL组<a name="ZH-CN_TOPIC_0060574392"></a>

## 功能介绍<a name="section61945363132813"></a>

更新网络ACL组。

## URI<a name="section27354345132813"></a>

PUT /v2.0/fwaas/firewall\_groups/\{firewall\_group\_id\}

## 请求消息<a name="section27893714132813"></a>

**表 1**  请求参数

<a name="table28101199132813"></a>
<table><thead align="left"><tr id="row55825911132813"><th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.1"><p id="p10707943132813"><a name="p10707943132813"></a><a name="p10707943132813"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p28975582132813"><a name="p28975582132813"></a><a name="p28975582132813"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p18050301132813"><a name="p18050301132813"></a><a name="p18050301132813"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p32456290132813"><a name="p32456290132813"></a><a name="p32456290132813"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row37137198132813"><td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.1 "><p id="p13657217132813"><a name="p13657217132813"></a><a name="p13657217132813"></a>firewall_group</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p40187772132813"><a name="p40187772132813"></a><a name="p40187772132813"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p43289917132813"><a name="p43289917132813"></a><a name="p43289917132813"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p5159094411463"><a name="p5159094411463"></a><a name="p5159094411463"></a>firewall group对象列表，参见<a href="网络ACL简介-OpenStack.md#table31629250121127">表3</a></p>
<p id="p41922418132813"><a name="p41922418132813"></a><a name="p41922418132813"></a>必选字段：无</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section39612821132813"></a>

**表 2**  响应参数

<a name="table16604779132813"></a>
<table><thead align="left"><tr id="row54692786132813"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p37352036132813"><a name="p37352036132813"></a><a name="p37352036132813"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p5454829132813"><a name="p5454829132813"></a><a name="p5454829132813"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p31055875132813"><a name="p31055875132813"></a><a name="p31055875132813"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row6198481132813"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p27058422132813"><a name="p27058422132813"></a><a name="p27058422132813"></a>firewall_group</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p32561041132813"><a name="p32561041132813"></a><a name="p32561041132813"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p2612398132813"><a name="p2612398132813"></a><a name="p2612398132813"></a>firewall group对象列表，参见<a href="网络ACL简介-OpenStack.md#table31629250121127">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section26765578132813"></a>

请求样例

```
PUT /v2.0/fwaas/firewall_groups/2fb0e81f-9f63-44b2-9894-c13a3284594a 
{
    "firewall_group": {
        "egress_firewall_policy_id": "53f36c32-db25-4856-a0ba-e605fd88c5e9"
    }
}
```

响应样例

```
{
    "firewall_group": {
        "status": "PENDING_UPDATE", 
        "public": false, 
        "egress_firewall_policy_id": "53f36c32-db25-4856-a0ba-e605fd88c5e9", 
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

