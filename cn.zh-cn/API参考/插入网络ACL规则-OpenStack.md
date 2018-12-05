# 插入网络ACL规则<a name="ZH-CN_TOPIC_0060574387"></a>

## 功能介绍<a name="section29654898132610"></a>

插入一条网络ACL规则到某一网络ACL策略中。

## URI<a name="section17120978132610"></a>

PUT /v2.0/fwaas/firewall\_policies/\{firewall\_policy\_id\}/insert\_rule

## 请求消息<a name="section22829642132610"></a>

**表 1**  请求参数

<a name="table57910527132610"></a>
<table><thead align="left"><tr id="row56750671132610"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="p7811312132610"><a name="p7811312132610"></a><a name="p7811312132610"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p18875016132610"><a name="p18875016132610"></a><a name="p18875016132610"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p27149878132610"><a name="p27149878132610"></a><a name="p27149878132610"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p59520796132610"><a name="p59520796132610"></a><a name="p59520796132610"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13167705132610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p30726413132610"><a name="p30726413132610"></a><a name="p30726413132610"></a>firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p27151448132610"><a name="p27151448132610"></a><a name="p27151448132610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p12448089132610"><a name="p12448089132610"></a><a name="p12448089132610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p35868466132610"><a name="p35868466132610"></a><a name="p35868466132610"></a>网络ACL策略唯一标识</p>
</td>
</tr>
<tr id="row26604881132610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p12663304132610"><a name="p12663304132610"></a><a name="p12663304132610"></a>firewall_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p32486375132610"><a name="p32486375132610"></a><a name="p32486375132610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p18635788132610"><a name="p18635788132610"></a><a name="p18635788132610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p109701641488"><a name="p109701641488"></a><a name="p109701641488"></a>网络ACL规则唯一标识</p>
</td>
</tr>
<tr id="row8034919132610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p55542506132610"><a name="p55542506132610"></a><a name="p55542506132610"></a>insert_after</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p15787556132610"><a name="p15787556132610"></a><a name="p15787556132610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p63384372132610"><a name="p63384372132610"></a><a name="p63384372132610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p38128195114117"><a name="p38128195114117"></a><a name="p38128195114117"></a>insert_after参数表示已经和某个policy关联的rule，新的rule将会直接被插入到insert_after参数指定的rule后面。</p>
<p id="p25644931114113"><a name="p25644931114113"></a><a name="p25644931114113"></a>如果insert_after和insert_before都被指定了，insert_after参数值将被忽略。</p>
</td>
</tr>
<tr id="row20668351132610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p42122069132610"><a name="p42122069132610"></a><a name="p42122069132610"></a>insert_before</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p46267954132610"><a name="p46267954132610"></a><a name="p46267954132610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p36183414132610"><a name="p36183414132610"></a><a name="p36183414132610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p24247215114125"><a name="p24247215114125"></a><a name="p24247215114125"></a>insert_before参数表示已经和某个policy关联的rule，新的firewall rule将会直接被插入到insert_ before参数指定的firewall rule前面。</p>
<p id="p48605762132610"><a name="p48605762132610"></a><a name="p48605762132610"></a>如果insert_after和insert_before都被指定了，insert_after参数值将被忽略。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section56633148132610"></a>

**表 2**  响应参数

<a name="table50663598132610"></a>
<table><thead align="left"><tr id="row38032515132610"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p37452312132610"><a name="p37452312132610"></a><a name="p37452312132610"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p10818837132610"><a name="p10818837132610"></a><a name="p10818837132610"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p58166210132610"><a name="p58166210132610"></a><a name="p58166210132610"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row30547380132610"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p22778252132610"><a name="p22778252132610"></a><a name="p22778252132610"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p5687403132610"><a name="p5687403132610"></a><a name="p5687403132610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p28250047132610"><a name="p28250047132610"></a><a name="p28250047132610"></a>对policy的描述信息</p>
</td>
</tr>
<tr id="row38138722132610"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p51429622132610"><a name="p51429622132610"></a><a name="p51429622132610"></a>audited</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p44611873132610"><a name="p44611873132610"></a><a name="p44611873132610"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p64467387132610"><a name="p64467387132610"></a><a name="p64467387132610"></a>每次policy或者它相关的rule有变动，该参数将会被置为False</p>
</td>
</tr>
<tr id="row37057482132610"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p2394977132610"><a name="p2394977132610"></a><a name="p2394977132610"></a>firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p46939168132610"><a name="p46939168132610"></a><a name="p46939168132610"></a>List</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p41445777132610"><a name="p41445777132610"></a><a name="p41445777132610"></a>与当前policy相关联的rule的ID列表</p>
</td>
</tr>
<tr id="row52861264132610"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p4531891132610"><a name="p4531891132610"></a><a name="p4531891132610"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p19878605132610"><a name="p19878605132610"></a><a name="p19878605132610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p37584805132610"><a name="p37584805132610"></a><a name="p37584805132610"></a>policy ID</p>
</td>
</tr>
<tr id="row19224600132610"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p61803150132610"><a name="p61803150132610"></a><a name="p61803150132610"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p31295563132610"><a name="p31295563132610"></a><a name="p31295563132610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p19158555132610"><a name="p19158555132610"></a><a name="p19158555132610"></a>Policy 名称</p>
</td>
</tr>
<tr id="row17433093132610"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p3069015132610"><a name="p3069015132610"></a><a name="p3069015132610"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p63788416132610"><a name="p63788416132610"></a><a name="p63788416132610"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p17812694132610"><a name="p17812694132610"></a><a name="p17812694132610"></a>如果为True, 该policy对于其他项目网络ACL策略可见， 默认不可见</p>
</td>
</tr>
<tr id="row66677436132610"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p61139761132610"><a name="p61139761132610"></a><a name="p61139761132610"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p16205070132610"><a name="p16205070132610"></a><a name="p16205070132610"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p45507963132610"><a name="p45507963132610"></a><a name="p45507963132610"></a>当前项目ID</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section42126241132610"></a>

请求样例

```
PUT /v2.0/fwaas/firewall_policies/afc52ce9-5305-4ec9-9feb-44feb8330341/insert_rule 
{
    "insert_after": "b8243448-cb3c-496e-851c-dadade4c161b", 
    "firewall_rule_id": "0f82b221-8cd6-44bd-9dfc-0e118fa7b6b1", 
    "insert_before": ""
}
```

响应样例

```
{
    "description": "", 
    "firewall_rules": [
        "b8243448-cb3c-496e-851c-dadade4c161b", 
        "0f82b221-8cd6-44bd-9dfc-0e118fa7b6b1"
    ], 
    "tenant_id": "23c8a121505047b6869edf39f3062712", 
    "public": false, 
    "id": "afc52ce9-5305-4ec9-9feb-44feb8330341", 
    "audited": false, 
    "name": "test-policy",
    "project_id": "23c8a121505047b6869edf39f3062712"
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

