# 查询VPC资源实例<a name="vpc_tag_0005"></a>

## 功能介绍<a name="section046482318191"></a>

使用标签过滤实例。

## URI<a name="section204655230197"></a>

POST /v2.0/\{project\_id\}/vpcs/resource\_instances/action

参数说明请参见[表1](#table27380479)。

**表 1**  参数说明

<a name="table27380479"></a>
<table><thead align="left"><tr id="row28751554"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p47174532"><a name="p47174532"></a><a name="p47174532"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p63040734"><a name="p63040734"></a><a name="p63040734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p6025849"><a name="p6025849"></a><a name="p6025849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18331773"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p8478608"><a name="p8478608"></a><a name="p8478608"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p15678685"><a name="p15678685"></a><a name="p15678685"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section747562331920"></a>

请求参数

**表 2**  请求参数

<a name="table45111823181914"></a>
<table><thead align="left"><tr id="row88521623101920"><th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.1"><p id="p168521123141913"><a name="p168521123141913"></a><a name="p168521123141913"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="10.891089108910892%" id="mcps1.2.5.1.2"><p id="p68525234198"><a name="p68525234198"></a><a name="p68525234198"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.2.5.1.3"><p id="p68524237196"><a name="p68524237196"></a><a name="p68524237196"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="57.42574257425742%" id="mcps1.2.5.1.4"><p id="p1785232391916"><a name="p1785232391916"></a><a name="p1785232391916"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row9852172316195"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p38521123191911"><a name="p38521123191911"></a><a name="p38521123191911"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p10424324181820"><a name="p10424324181820"></a><a name="p10424324181820"></a>Array of <a href="#table1548032316199">tag</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p15852102341915"><a name="p15852102341915"></a><a name="p15852102341915"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="p1885242381910"><a name="p1885242381910"></a><a name="p1885242381910"></a>包含标签，最多包含10个key，每个key下面的value最多10个，结构体不能缺失，key不能为空或者空字符串。Key不能重复，同一个key中values不能重复。</p>
</td>
</tr>
<tr id="row485202331911"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p08523237195"><a name="p08523237195"></a><a name="p08523237195"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p1285218232197"><a name="p1285218232197"></a><a name="p1285218232197"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p1985292314197"><a name="p1985292314197"></a><a name="p1985292314197"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="p13852152341914"><a name="p13852152341914"></a><a name="p13852152341914"></a>查询记录数（action为count时无此参数）如果action为filter默认为1000，limit最多为1000,不能为负数，最小值为1</p>
</td>
</tr>
<tr id="row14852423111914"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p885219237198"><a name="p885219237198"></a><a name="p885219237198"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p1985218237191"><a name="p1985218237191"></a><a name="p1985218237191"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p5852132317199"><a name="p5852132317199"></a><a name="p5852132317199"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="p1785342311917"><a name="p1785342311917"></a><a name="p1785342311917"></a>（索引位置）， 从offset指定的下一条数据开始查询。 查询第一页数据时，不需要传入此参数，查询后续页码数据时，将查询前一页数据时响应体中的值带入此参数（action为count时无此参数）如果action为filter默认为0,必须为数字，不能为负数</p>
</td>
</tr>
<tr id="row28531123181913"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p1853123121912"><a name="p1853123121912"></a><a name="p1853123121912"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p14853122371914"><a name="p14853122371914"></a><a name="p14853122371914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p17853152331919"><a name="p17853152331919"></a><a name="p17853152331919"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="p6853182320190"><a name="p6853182320190"></a><a name="p6853182320190"></a>操作标识（仅限于filter，count）：filter（过滤），count(查询总条数)</p>
<p id="p1185332315194"><a name="p1185332315194"></a><a name="p1185332315194"></a>如果是filter就是分页查询，如果是count只需按照条件将总条数返回即可。</p>
</td>
</tr>
<tr id="row1885318232195"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p085315232194"><a name="p085315232194"></a><a name="p085315232194"></a>matches</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p12177957181019"><a name="p12177957181019"></a><a name="p12177957181019"></a>Array of <a href="#table104959232192">match</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p18853102313197"><a name="p18853102313197"></a><a name="p18853102313197"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="p128537230197"><a name="p128537230197"></a><a name="p128537230197"></a>搜索字段，key为要匹配的字段，当前仅支持resource_name。value为匹配的值。此字段为固定字典值。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  tag字段数据结构说明

<a name="table1548032316199"></a>
<table><thead align="left"><tr id="row1785310237196"><th class="cellrowborder" valign="top" width="31.626837316268368%" id="mcps1.2.5.1.1"><p id="p185312312192"><a name="p185312312192"></a><a name="p185312312192"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.2"><p id="p208531923101913"><a name="p208531923101913"></a><a name="p208531923101913"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.3"><p id="p685312311196"><a name="p685312311196"></a><a name="p685312311196"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.7960203979602%" id="mcps1.2.5.1.4"><p id="p4853122311199"><a name="p4853122311199"></a><a name="p4853122311199"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row08532238197"><td class="cellrowborder" valign="top" width="31.626837316268368%" headers="mcps1.2.5.1.1 "><p id="p16854122312191"><a name="p16854122312191"></a><a name="p16854122312191"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="p10854102317195"><a name="p10854102317195"></a><a name="p10854102317195"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="p5854122371919"><a name="p5854122371919"></a><a name="p5854122371919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.7960203979602%" headers="mcps1.2.5.1.4 "><p id="p085432316193"><a name="p085432316193"></a><a name="p085432316193"></a>键。最大长度127个unicode字符。 key不能为空。(搜索时不对此参数做校验)</p>
</td>
</tr>
<tr id="row15854623141911"><td class="cellrowborder" valign="top" width="31.626837316268368%" headers="mcps1.2.5.1.1 "><p id="p68541223141919"><a name="p68541223141919"></a><a name="p68541223141919"></a>values</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="p17854223161918"><a name="p17854223161918"></a><a name="p17854223161918"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="p188541423181914"><a name="p188541423181914"></a><a name="p188541423181914"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="39.7960203979602%" headers="mcps1.2.5.1.4 "><p id="p198541623121914"><a name="p198541623121914"></a><a name="p198541623121914"></a>值列表。每个值最大长度255个unicode字符，如果values为空列表，则表示any_value。value之间为或的关系。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  match字段数据结构说明

<a name="table104959232192"></a>
<table><thead align="left"><tr id="row208541423191917"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.5.1.1"><p id="p1385417236194"><a name="p1385417236194"></a><a name="p1385417236194"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.13131313131313%" id="mcps1.2.5.1.2"><p id="p1485442313195"><a name="p1485442313195"></a><a name="p1485442313195"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.3"><p id="p4854182361910"><a name="p4854182361910"></a><a name="p4854182361910"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.39393939393939%" id="mcps1.2.5.1.4"><p id="p685472317197"><a name="p685472317197"></a><a name="p685472317197"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row12854323201911"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.5.1.1 "><p id="p285482316198"><a name="p285482316198"></a><a name="p285482316198"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="13.13131313131313%" headers="mcps1.2.5.1.2 "><p id="p4854723121918"><a name="p4854723121918"></a><a name="p4854723121918"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p385422301919"><a name="p385422301919"></a><a name="p385422301919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.2.5.1.4 "><p id="p185514232197"><a name="p185514232197"></a><a name="p185514232197"></a>键。当前仅限定为resource_name</p>
</td>
</tr>
<tr id="row28552023131919"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.5.1.1 "><p id="p485514231195"><a name="p485514231195"></a><a name="p485514231195"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13.13131313131313%" headers="mcps1.2.5.1.2 "><p id="p58551523191914"><a name="p58551523191914"></a><a name="p58551523191914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="p128551235194"><a name="p128551235194"></a><a name="p128551235194"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.2.5.1.4 "><p id="p128551023151916"><a name="p128551023151916"></a><a name="p128551023151916"></a>值。每个值最大长度255个unicode字符。</p>
</td>
</tr>
</tbody>
</table>

请求样例1：action为filter

```
POST https://{Endpoint}/v2.0/{project_id}/vpcs/resource_instances/action

{
    "offset": "0",
    "limit": "100",
    "action": "filter",
    "matches": [
        {
            "key": "resource_name",
            "value": "resource1"
        }
    ],
    "tags": [
        {
            "key": "key1",
            "values": [
                "*value1",
                "value2"
            ]
        }
    ]
}
```

请求样例2：action为count

```
POST https://{Endpoint}/v2.0/{project_id}/vpcs/resource_instances/action

{
    "action": "count",
    "tags": [
        {
            "key": "key1",
            "values": [
                "value1",
                "value2"
            ]
        },
        {
            "key": "key2",
            "values": [
                "value1",
                "value2"
            ]
        }
    ],
    "matches": [
        {
            "key": "resource_name",
            "value": "resource1"
        }
    ]
}
```

## 响应消息<a name="section95436234191"></a>

响应参数

**表 5**  响应参数

<a name="table25631238196"></a>
<table><thead align="left"><tr id="row285515239199"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.1"><p id="p1385512317198"><a name="p1385512317198"></a><a name="p1385512317198"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="37.330000000000005%" id="mcps1.2.4.1.2"><p id="p158555239198"><a name="p158555239198"></a><a name="p158555239198"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.67%" id="mcps1.2.4.1.3"><p id="p2855102313199"><a name="p2855102313199"></a><a name="p2855102313199"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2855172320193"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="p685502321914"><a name="p685502321914"></a><a name="p685502321914"></a>resources</p>
</td>
<td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="p8347412111010"><a name="p8347412111010"></a><a name="p8347412111010"></a>Array of <a href="#table1454542331912">resource</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="p68562235195"><a name="p68562235195"></a><a name="p68562235195"></a>resource对象列表，请参见<a href="#table1454542331912">表6</a>。</p>
</td>
</tr>
<tr id="row16856223111912"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="p285620239197"><a name="p285620239197"></a><a name="p285620239197"></a>total_count</p>
</td>
<td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="p168562234194"><a name="p168562234194"></a><a name="p168562234194"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="p58561323181910"><a name="p58561323181910"></a><a name="p58561323181910"></a>总记录数</p>
</td>
</tr>
</tbody>
</table>

**表 6**  resource对象

<a name="table1454542331912"></a>
<table><thead align="left"><tr id="row385622315195"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.1"><p id="p1785610232193"><a name="p1785610232193"></a><a name="p1785610232193"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="37.330000000000005%" id="mcps1.2.4.1.2"><p id="p16856132351913"><a name="p16856132351913"></a><a name="p16856132351913"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.67%" id="mcps1.2.4.1.3"><p id="p1285622318195"><a name="p1285622318195"></a><a name="p1285622318195"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row185662311194"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="p1385611238195"><a name="p1385611238195"></a><a name="p1385611238195"></a>resource_id</p>
</td>
<td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="p6856152314195"><a name="p6856152314195"></a><a name="p6856152314195"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="p128561823141910"><a name="p128561823141910"></a><a name="p128561823141910"></a>资源ID</p>
</td>
</tr>
<tr id="row5856162316198"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="p985642311196"><a name="p985642311196"></a><a name="p985642311196"></a>resouce_detail</p>
</td>
<td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="p1285742310190"><a name="p1285742310190"></a><a name="p1285742310190"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="p8857523191910"><a name="p8857523191910"></a><a name="p8857523191910"></a>资源详情。 资源对象，用于扩展。默认为空</p>
</td>
</tr>
<tr id="row1859132311911"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="p0859423151913"><a name="p0859423151913"></a><a name="p0859423151913"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="p18794152718455"><a name="p18794152718455"></a><a name="p18794152718455"></a>Array of <a href="#table1353515016272">tag</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="p1985922316199"><a name="p1985922316199"></a><a name="p1985922316199"></a>标签列表，没有标签默认为空数组，参见<a href="#table1353515016272">表7</a></p>
</td>
</tr>
<tr id="row13859102317194"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="p1785919234197"><a name="p1785919234197"></a><a name="p1785919234197"></a>resource_name</p>
</td>
<td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="p138591823191919"><a name="p138591823191919"></a><a name="p138591823191919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="p68591823131919"><a name="p68591823131919"></a><a name="p68591823131919"></a>资源名称，没有默认为空字符串</p>
</td>
</tr>
</tbody>
</table>

**表 7**  tag字段数据结构说明

<a name="table1353515016272"></a>
<table><thead align="left"><tr id="row12536145015270"><th class="cellrowborder" valign="top" width="31.626837316268368%" id="mcps1.2.5.1.1"><p id="p153615010278"><a name="p153615010278"></a><a name="p153615010278"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.2"><p id="p205361850152712"><a name="p205361850152712"></a><a name="p205361850152712"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.3"><p id="p155361850162716"><a name="p155361850162716"></a><a name="p155361850162716"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.7960203979602%" id="mcps1.2.5.1.4"><p id="p105361150132714"><a name="p105361150132714"></a><a name="p105361150132714"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row653695012712"><td class="cellrowborder" valign="top" width="31.626837316268368%" headers="mcps1.2.5.1.1 "><p id="p155361650192714"><a name="p155361650192714"></a><a name="p155361650192714"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="p1853675017273"><a name="p1853675017273"></a><a name="p1853675017273"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="p3536250152718"><a name="p3536250152718"></a><a name="p3536250152718"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.7960203979602%" headers="mcps1.2.5.1.4 "><p id="p4536105010277"><a name="p4536105010277"></a><a name="p4536105010277"></a>键。最大长度127个unicode字符。 key不能为空。(搜索时不对此参数做校验)</p>
</td>
</tr>
<tr id="row11536165042716"><td class="cellrowborder" valign="top" width="31.626837316268368%" headers="mcps1.2.5.1.1 "><p id="p175361650142718"><a name="p175361650142718"></a><a name="p175361650142718"></a>values</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="p9536175042714"><a name="p9536175042714"></a><a name="p9536175042714"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="p13536155052713"><a name="p13536155052713"></a><a name="p13536155052713"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="39.7960203979602%" headers="mcps1.2.5.1.4 "><p id="p153645062719"><a name="p153645062719"></a><a name="p153645062719"></a>值列表。每个值最大长度255个unicode字符，如果values为空列表，则表示any_value。value之间为或的关系。</p>
</td>
</tr>
</tbody>
</table>

响应样例1：action为filter

```
{ 
      "resources": [
         {
            "resource_detail": null, 
            "resource_id": "cdfs_cefs_wesas_12_dsad", 
            "resource_name": "resouece1", 
            "tags": [
                {
                   "key": "key1"，
                   "value": "value1"
                },
                {
                   "key": "key2"，
                   "value": "value1"
                }
             ]
         }
       ], 
      "total_count": 1000
}
 
```

响应样例2：action为count

```
{
       "total_count": 1000
}
```

## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

