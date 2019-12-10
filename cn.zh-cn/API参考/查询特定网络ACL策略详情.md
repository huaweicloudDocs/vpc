# 查询特定网络ACL策略详情<a name="ZH-CN_TOPIC_0201534277"></a>

## 功能介绍<a name="section915947313242"></a>

查询特定网络ACL策略详情。

## URI<a name="section2518841213242"></a>

GET /v2.0/fwaas/firewall\_policies/\{firewall\_policy\_id\}

参数说明请参见[表1](#table18880184689)。

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
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p2885681613242"><a name="p2885681613242"></a><a name="p2885681613242"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p6121237313242"><a name="p6121237313242"></a><a name="p6121237313242"></a>firewall policy对象列表。请参见<a href="#table17002720121127">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  Firewall Policy对象

<a name="table17002720121127"></a>
<table><thead align="left"><tr id="row16929792121127"><th class="cellrowborder" valign="top" width="32.083208320832085%" id="mcps1.2.4.1.1"><p id="p18873879121127"><a name="p18873879121127"></a><a name="p18873879121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="22.632263226322635%" id="mcps1.2.4.1.2"><p id="p12638309121127"><a name="p12638309121127"></a><a name="p12638309121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="45.28452845284529%" id="mcps1.2.4.1.3"><p id="p61199938121127"><a name="p61199938121127"></a><a name="p61199938121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46402691121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p11805115121127"><a name="p11805115121127"></a><a name="p11805115121127"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p13006089121127"><a name="p13006089121127"></a><a name="p13006089121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p13152683121127"><a name="p13152683121127"></a><a name="p13152683121127"></a>网络ACL策略uuid标识。</p>
</td>
</tr>
<tr id="row9858171121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p49865700121127"><a name="p49865700121127"></a><a name="p49865700121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p6225460121127"><a name="p6225460121127"></a><a name="p6225460121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p40337147121127"><a name="p40337147121127"></a><a name="p40337147121127"></a>网络ACL策略名称。</p>
</td>
</tr>
<tr id="row61803802121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p39621949121127"><a name="p39621949121127"></a><a name="p39621949121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p66053143121127"><a name="p66053143121127"></a><a name="p66053143121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p15357220121127"><a name="p15357220121127"></a><a name="p15357220121127"></a>网络ACL策略描述。</p>
</td>
</tr>
<tr id="row57644277121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p9761241121127"><a name="p9761241121127"></a><a name="p9761241121127"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p20138053121127"><a name="p20138053121127"></a><a name="p20138053121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row33369184121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p16940942121127"><a name="p16940942121127"></a><a name="p16940942121127"></a>firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p1916011339370"><a name="p1916011339370"></a><a name="p1916011339370"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p53455884121127"><a name="p53455884121127"></a><a name="p53455884121127"></a>策略引用的网络ACL规则链。</p>
</td>
</tr>
<tr id="row717167121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p30704110121127"><a name="p30704110121127"></a><a name="p30704110121127"></a>audited</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p10804884121127"><a name="p10804884121127"></a><a name="p10804884121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p3925300121127"><a name="p3925300121127"></a><a name="p3925300121127"></a>审计标记。</p>
</td>
</tr>
<tr id="row40905717121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p16821838121127"><a name="p16821838121127"></a><a name="p16821838121127"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p49691806121127"><a name="p49691806121127"></a><a name="p49691806121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p31604739121127"><a name="p31604739121127"></a><a name="p31604739121127"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row109594223354"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p17700201411911"><a name="p17700201411911"></a><a name="p17700201411911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p20137347142815"><a name="p20137347142815"></a><a name="p20137347142815"></a>项目ID</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section478525713242"></a>

请求样例

```
GET https://{Endpoint}/v2.0/fwaas/firewall_policies/fed2d88f-d0e7-4cc5-bd7e-c495f67037b6
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

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

