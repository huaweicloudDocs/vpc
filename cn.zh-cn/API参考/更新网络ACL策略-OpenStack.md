# 更新网络ACL策略<a name="ZH-CN_TOPIC_0060574385"></a>

## 功能介绍<a name="section19593265132522"></a>

更新网络ACL策略。

## URI<a name="section46147480132522"></a>

PUT /v2.0/fwaas/firewall\_policies/\{firewall\_policy\_id\}

## 请求消息<a name="section36048911132522"></a>

**表 1**  请求参数

<a name="table8852370132522"></a>
<table><thead align="left"><tr id="row32357095132522"><th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.1"><p id="p45580669132522"><a name="p45580669132522"></a><a name="p45580669132522"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p51498842132522"><a name="p51498842132522"></a><a name="p51498842132522"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p56072606132522"><a name="p56072606132522"></a><a name="p56072606132522"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p6648170132522"><a name="p6648170132522"></a><a name="p6648170132522"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row64881628132522"><td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.1 "><p id="p14588437132522"><a name="p14588437132522"></a><a name="p14588437132522"></a>firewall_policy</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p52664630132522"><a name="p52664630132522"></a><a name="p52664630132522"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p43844189132522"><a name="p43844189132522"></a><a name="p43844189132522"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p50197883132340"><a name="p50197883132340"></a><a name="p50197883132340"></a>firewall policy对象列表，参见<a href="网络ACL简介-OpenStack.md#table17002720121127">表2</a>。</p>
<p id="p62725571132522"><a name="p62725571132522"></a><a name="p62725571132522"></a>必选字段：无</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section41558848132522"></a>

**表 2**  响应参数

<a name="table35154237132522"></a>
<table><thead align="left"><tr id="row52261665132522"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p65769625132522"><a name="p65769625132522"></a><a name="p65769625132522"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p12018727132522"><a name="p12018727132522"></a><a name="p12018727132522"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p17036810132522"><a name="p17036810132522"></a><a name="p17036810132522"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row43204254132522"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p40260041132522"><a name="p40260041132522"></a><a name="p40260041132522"></a>firewall_policy</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p26565290132522"><a name="p26565290132522"></a><a name="p26565290132522"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p59164179132522"><a name="p59164179132522"></a><a name="p59164179132522"></a>firewall policy对象列表，参见<a href="网络ACL简介-OpenStack.md#table17002720121127">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section41774729132522"></a>

请求样例

```
PUT /v2.0/fwaas/firewall_policies/2fb0e81f-9f63-44b2-9894-c13a3284594a 
{
    "firewall_policy": {
        "firewall_rules": [
            "0f82b221-8cd6-44bd-9dfc-0e118fa7b6b1"
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
            "0f82b221-8cd6-44bd-9dfc-0e118fa7b6b1"
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

