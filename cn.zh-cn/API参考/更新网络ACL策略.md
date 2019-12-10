# 更新网络ACL策略<a name="ZH-CN_TOPIC_0201534069"></a>

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
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p52664630132522"><a name="p52664630132522"></a><a name="p52664630132522"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p43844189132522"><a name="p43844189132522"></a><a name="p43844189132522"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p50197883132340"><a name="p50197883132340"></a><a name="p50197883132340"></a>firewall policy对象。请参见<a href="#table17002720121127">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Firewall Policy对象

<a name="table17002720121127"></a>
<table><thead align="left"><tr id="row16929792121127"><th class="cellrowborder" valign="top" width="23.21%" id="mcps1.2.5.1.1"><p id="p18873879121127"><a name="p18873879121127"></a><a name="p18873879121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="13.98%" id="mcps1.2.5.1.2"><p id="p1187191018576"><a name="p1187191018576"></a><a name="p1187191018576"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.93%" id="mcps1.2.5.1.3"><p id="p12638309121127"><a name="p12638309121127"></a><a name="p12638309121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.88%" id="mcps1.2.5.1.4"><p id="p61199938121127"><a name="p61199938121127"></a><a name="p61199938121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row9858171121127"><td class="cellrowborder" valign="top" width="23.21%" headers="mcps1.2.5.1.1 "><p id="p49865700121127"><a name="p49865700121127"></a><a name="p49865700121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.98%" headers="mcps1.2.5.1.2 "><p id="p287210165719"><a name="p287210165719"></a><a name="p287210165719"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.93%" headers="mcps1.2.5.1.3 "><p id="p6225460121127"><a name="p6225460121127"></a><a name="p6225460121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.88%" headers="mcps1.2.5.1.4 "><p id="p40337147121127"><a name="p40337147121127"></a><a name="p40337147121127"></a>网络ACL策略名称。</p>
<p id="p1606122895617"><a name="p1606122895617"></a><a name="p1606122895617"></a>使用说明：最长255个字符</p>
</td>
</tr>
<tr id="row61803802121127"><td class="cellrowborder" valign="top" width="23.21%" headers="mcps1.2.5.1.1 "><p id="p39621949121127"><a name="p39621949121127"></a><a name="p39621949121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13.98%" headers="mcps1.2.5.1.2 "><p id="p087191011575"><a name="p087191011575"></a><a name="p087191011575"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.93%" headers="mcps1.2.5.1.3 "><p id="p66053143121127"><a name="p66053143121127"></a><a name="p66053143121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.88%" headers="mcps1.2.5.1.4 "><p id="p15357220121127"><a name="p15357220121127"></a><a name="p15357220121127"></a>网络ACL策略描述。</p>
<p id="p1267612575565"><a name="p1267612575565"></a><a name="p1267612575565"></a>使用说明：最长255个字符</p>
</td>
</tr>
<tr id="row33369184121127"><td class="cellrowborder" valign="top" width="23.21%" headers="mcps1.2.5.1.1 "><p id="p16940942121127"><a name="p16940942121127"></a><a name="p16940942121127"></a>firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="13.98%" headers="mcps1.2.5.1.2 "><p id="p7871410165711"><a name="p7871410165711"></a><a name="p7871410165711"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.93%" headers="mcps1.2.5.1.3 "><p id="p27024915121127"><a name="p27024915121127"></a><a name="p27024915121127"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="41.88%" headers="mcps1.2.5.1.4 "><p id="p53455884121127"><a name="p53455884121127"></a><a name="p53455884121127"></a>策略引用的网络ACL规则链。</p>
</td>
</tr>
<tr id="row717167121127"><td class="cellrowborder" valign="top" width="23.21%" headers="mcps1.2.5.1.1 "><p id="p30704110121127"><a name="p30704110121127"></a><a name="p30704110121127"></a>audited</p>
</td>
<td class="cellrowborder" valign="top" width="13.98%" headers="mcps1.2.5.1.2 "><p id="p17871310145717"><a name="p17871310145717"></a><a name="p17871310145717"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.93%" headers="mcps1.2.5.1.3 "><p id="p10804884121127"><a name="p10804884121127"></a><a name="p10804884121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="41.88%" headers="mcps1.2.5.1.4 "><p id="p3925300121127"><a name="p3925300121127"></a><a name="p3925300121127"></a>审计标记。</p>
<p id="p172123197567"><a name="p172123197567"></a><a name="p172123197567"></a>取值范围：true/false</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section41558848132522"></a>

**表 3**  响应参数

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
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p26565290132522"><a name="p26565290132522"></a><a name="p26565290132522"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p59164179132522"><a name="p59164179132522"></a><a name="p59164179132522"></a>firewall policy对象。请参见<a href="#table6763048152111">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  Firewall Policy对象

<a name="table6763048152111"></a>
<table><thead align="left"><tr id="row18764194892115"><th class="cellrowborder" valign="top" width="32.083208320832085%" id="mcps1.2.4.1.1"><p id="p3764194815213"><a name="p3764194815213"></a><a name="p3764194815213"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="22.632263226322635%" id="mcps1.2.4.1.2"><p id="p876474817212"><a name="p876474817212"></a><a name="p876474817212"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="45.28452845284529%" id="mcps1.2.4.1.3"><p id="p1876484815214"><a name="p1876484815214"></a><a name="p1876484815214"></a>说明</p>
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
<tr id="row376464814211"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p19764204872112"><a name="p19764204872112"></a><a name="p19764204872112"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p2764154815210"><a name="p2764154815210"></a><a name="p2764154815210"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p676474842118"><a name="p676474842118"></a><a name="p676474842118"></a>网络ACL策略名称。</p>
</td>
</tr>
<tr id="row5764144892115"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p476424842118"><a name="p476424842118"></a><a name="p476424842118"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p147654481219"><a name="p147654481219"></a><a name="p147654481219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p18765204812117"><a name="p18765204812117"></a><a name="p18765204812117"></a>网络ACL策略描述。</p>
</td>
</tr>
<tr id="row3765184815214"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p11765848162113"><a name="p11765848162113"></a><a name="p11765848162113"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p4765548162116"><a name="p4765548162116"></a><a name="p4765548162116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row7766248182119"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p376624822116"><a name="p376624822116"></a><a name="p376624822116"></a>firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p2070691313818"><a name="p2070691313818"></a><a name="p2070691313818"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p076694811218"><a name="p076694811218"></a><a name="p076694811218"></a>策略引用的网络ACL规则链。</p>
</td>
</tr>
<tr id="row376664817218"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p1376624892119"><a name="p1376624892119"></a><a name="p1376624892119"></a>audited</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p197661748132118"><a name="p197661748132118"></a><a name="p197661748132118"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p1676694811214"><a name="p1676694811214"></a><a name="p1676694811214"></a>审计标记。</p>
</td>
</tr>
<tr id="row1976619489210"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p1376694818214"><a name="p1376694818214"></a><a name="p1376694818214"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p576634816213"><a name="p576634816213"></a><a name="p576634816213"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p19766748192115"><a name="p19766748192115"></a><a name="p19766748192115"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row109594223354"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p17700201411911"><a name="p17700201411911"></a><a name="p17700201411911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p28021558142812"><a name="p28021558142812"></a><a name="p28021558142812"></a>项目ID</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section41774729132522"></a>

请求样例

```
PUT https://{Endpoint}/v2.0/fwaas/firewall_policies/2fb0e81f-9f63-44b2-9894-c13a3284594a 

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

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

