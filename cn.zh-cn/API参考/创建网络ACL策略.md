# 创建网络ACL策略<a name="vpc_firewall_0008"></a>

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
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p5375326713250"><a name="p5375326713250"></a><a name="p5375326713250"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p5311559313250"><a name="p5311559313250"></a><a name="p5311559313250"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p3083242213250"><a name="p3083242213250"></a><a name="p3083242213250"></a>firewall policy对象列表。请参见<a href="#table17002720121127">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Firewall Policy对象

<a name="table17002720121127"></a>
<table><thead align="left"><tr id="row16929792121127"><th class="cellrowborder" valign="top" width="20.830000000000002%" id="mcps1.2.5.1.1"><p id="p18873879121127"><a name="p18873879121127"></a><a name="p18873879121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="16.35%" id="mcps1.2.5.1.2"><p id="p1558616214598"><a name="p1558616214598"></a><a name="p1558616214598"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.94%" id="mcps1.2.5.1.3"><p id="p12638309121127"><a name="p12638309121127"></a><a name="p12638309121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.88%" id="mcps1.2.5.1.4"><p id="p61199938121127"><a name="p61199938121127"></a><a name="p61199938121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row9858171121127"><td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.5.1.1 "><p id="p49865700121127"><a name="p49865700121127"></a><a name="p49865700121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.2 "><p id="p13586523597"><a name="p13586523597"></a><a name="p13586523597"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.94%" headers="mcps1.2.5.1.3 "><p id="p6225460121127"><a name="p6225460121127"></a><a name="p6225460121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.88%" headers="mcps1.2.5.1.4 "><p id="p40337147121127"><a name="p40337147121127"></a><a name="p40337147121127"></a>网络ACL策略名称。</p>
<p id="p078324045715"><a name="p078324045715"></a><a name="p078324045715"></a>使用说明：最长255个字符</p>
</td>
</tr>
<tr id="row61803802121127"><td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.5.1.1 "><p id="p39621949121127"><a name="p39621949121127"></a><a name="p39621949121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.2 "><p id="p9586132125919"><a name="p9586132125919"></a><a name="p9586132125919"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.94%" headers="mcps1.2.5.1.3 "><p id="p66053143121127"><a name="p66053143121127"></a><a name="p66053143121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.88%" headers="mcps1.2.5.1.4 "><p id="p15357220121127"><a name="p15357220121127"></a><a name="p15357220121127"></a>网络ACL策略描述。</p>
<p id="p9538853205712"><a name="p9538853205712"></a><a name="p9538853205712"></a>使用说明：最长255个字符</p>
</td>
</tr>
<tr id="row33369184121127"><td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.5.1.1 "><p id="p16940942121127"><a name="p16940942121127"></a><a name="p16940942121127"></a>firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.2 "><p id="p958617217599"><a name="p958617217599"></a><a name="p958617217599"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.94%" headers="mcps1.2.5.1.3 "><p id="p27024915121127"><a name="p27024915121127"></a><a name="p27024915121127"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="41.88%" headers="mcps1.2.5.1.4 "><p id="p53455884121127"><a name="p53455884121127"></a><a name="p53455884121127"></a>策略引用的网络ACL规则链。</p>
</td>
</tr>
<tr id="row717167121127"><td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.5.1.1 "><p id="p30704110121127"><a name="p30704110121127"></a><a name="p30704110121127"></a>audited</p>
</td>
<td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.2 "><p id="p1586172195914"><a name="p1586172195914"></a><a name="p1586172195914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.94%" headers="mcps1.2.5.1.3 "><p id="p10804884121127"><a name="p10804884121127"></a><a name="p10804884121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="41.88%" headers="mcps1.2.5.1.4 "><p id="p3925300121127"><a name="p3925300121127"></a><a name="p3925300121127"></a>审计标记。</p>
<p id="p04705516572"><a name="p04705516572"></a><a name="p04705516572"></a>取值范围：true/false</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section3860887413250"></a>

**表 3**  响应参数

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
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p4446263713250"><a name="p4446263713250"></a><a name="p4446263713250"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p4558033913250"><a name="p4558033913250"></a><a name="p4558033913250"></a>firewall policy对象列表。请参见<a href="#table6763048152111">表4</a>。</p>
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
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p127661248192113"><a name="p127661248192113"></a><a name="p127661248192113"></a>Array of strings</p>
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
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p1582585392819"><a name="p1582585392819"></a><a name="p1582585392819"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section5030474113250"></a>

请求样例

```
POST https://{Endpoint}/v2.0/fwaas/firewall_policies

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

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

