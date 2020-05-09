# 查询安全组<a name="vpc_sg02_0001"></a>

## 功能介绍<a name="section1170323616037"></a>

查询提交请求的租户有权限操作的所有安全组。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section2797834416037"></a>

GET /v2.0/security-groups

分页查询样例：

```
GET https://{Endpoint}/v2.0/security-groups?limit=2&marker=0431c9c5-1660-42e0-8a00-134bec7f03e2&page_reverse=False
```

参数说明请参见[表1](#table1687161718223)。

**表 1**  参数说明

<a name="table1687161718223"></a>
<table><thead align="left"><tr id="row396316178224"><th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.2.5.1.1"><p id="p14963617122211"><a name="p14963617122211"></a><a name="p14963617122211"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.2"><p id="p19964161752210"><a name="p19964161752210"></a><a name="p19964161752210"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.54175417541754%" id="mcps1.2.5.1.3"><p id="p1396481772212"><a name="p1396481772212"></a><a name="p1396481772212"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="46.09460946094609%" id="mcps1.2.5.1.4"><p id="p796421711226"><a name="p796421711226"></a><a name="p796421711226"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17964117122212"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1396481719225"><a name="p1396481719225"></a><a name="p1396481719225"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p17964717142210"><a name="p17964717142210"></a><a name="p17964717142210"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.54175417541754%" headers="mcps1.2.5.1.3 "><p id="p8964417192215"><a name="p8964417192215"></a><a name="p8964417192215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.09460946094609%" headers="mcps1.2.5.1.4 "><p id="p169644177228"><a name="p169644177228"></a><a name="p169644177228"></a>按照安全组对应的ID过滤查询</p>
</td>
</tr>
<tr id="row69646172222"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p89647174229"><a name="p89647174229"></a><a name="p89647174229"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p6964111702216"><a name="p6964111702216"></a><a name="p6964111702216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.54175417541754%" headers="mcps1.2.5.1.3 "><p id="p296421782217"><a name="p296421782217"></a><a name="p296421782217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.09460946094609%" headers="mcps1.2.5.1.4 "><p id="p11964717192216"><a name="p11964717192216"></a><a name="p11964717192216"></a>按照安全组的名称过滤查询</p>
</td>
</tr>
<tr id="row1996419172225"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p2096413173223"><a name="p2096413173223"></a><a name="p2096413173223"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p596421732212"><a name="p596421732212"></a><a name="p596421732212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.54175417541754%" headers="mcps1.2.5.1.3 "><p id="p10964131710228"><a name="p10964131710228"></a><a name="p10964131710228"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.09460946094609%" headers="mcps1.2.5.1.4 "><p id="p2096421719225"><a name="p2096421719225"></a><a name="p2096421719225"></a>按照安全组的描述过滤查询</p>
</td>
</tr>
<tr id="row396451752217"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p179648172225"><a name="p179648172225"></a><a name="p179648172225"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p196411752220"><a name="p196411752220"></a><a name="p196411752220"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.54175417541754%" headers="mcps1.2.5.1.3 "><p id="p11964181772212"><a name="p11964181772212"></a><a name="p11964181772212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.09460946094609%" headers="mcps1.2.5.1.4 "><p id="p5964217162211"><a name="p5964217162211"></a><a name="p5964217162211"></a>按照安全组所属的项目ID过滤查询</p>
</td>
</tr>
<tr id="row39646172224"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p109641217162215"><a name="p109641217162215"></a><a name="p109641217162215"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p199641717112219"><a name="p199641717112219"></a><a name="p199641717112219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.54175417541754%" headers="mcps1.2.5.1.3 "><p id="p796412174223"><a name="p796412174223"></a><a name="p796412174223"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.09460946094609%" headers="mcps1.2.5.1.4 "><p id="p496412171223"><a name="p496412171223"></a><a name="p496412171223"></a>分页查询起始的资源ID，为空时为查询第一页</p>
</td>
</tr>
<tr id="row10964201702215"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p10964111722211"><a name="p10964111722211"></a><a name="p10964111722211"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p896421742213"><a name="p896421742213"></a><a name="p896421742213"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.54175417541754%" headers="mcps1.2.5.1.3 "><p id="p18965161732218"><a name="p18965161732218"></a><a name="p18965161732218"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="46.09460946094609%" headers="mcps1.2.5.1.4 "><p id="p96971524162214"><a name="p96971524162214"></a><a name="p96971524162214"></a>每页返回的个数</p>
<p id="p1496571772219"><a name="p1496571772219"></a><a name="p1496571772219"></a>取值范围：0~intmax</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section3834086716037"></a>

无。

## 响应消息<a name="section6006230416037"></a>

**表 2**  响应参数

<a name="table1547016516037"></a>
<table><thead align="left"><tr id="row2546099716037"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p3614026216037"><a name="p3614026216037"></a><a name="p3614026216037"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p3446060616037"><a name="p3446060616037"></a><a name="p3446060616037"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p3726817816037"><a name="p3726817816037"></a><a name="p3726817816037"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row841863916037"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p5631571516037"><a name="p5631571516037"></a><a name="p5631571516037"></a>security_groups</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p86066502616"><a name="p86066502616"></a><a name="p86066502616"></a>Array of <a href="#table513726041607">Security Group</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p6079210416037"><a name="p6079210416037"></a><a name="p6079210416037"></a>security group对象列表。请参见<a href="#table513726041607">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  Security Group对象

<a name="table513726041607"></a>
<table><thead align="left"><tr id="row72893461607"><th class="cellrowborder" valign="top" width="26.669999999999998%" id="mcps1.2.4.1.1"><p id="p647825491607"><a name="p647825491607"></a><a name="p647825491607"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.2"><p id="p245230881607"><a name="p245230881607"></a><a name="p245230881607"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="p4542071607"><a name="p4542071607"></a><a name="p4542071607"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row284118681607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p6322881607"><a name="p6322881607"></a><a name="p6322881607"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p206339641607"><a name="p206339641607"></a><a name="p206339641607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p538811831607"><a name="p538811831607"></a><a name="p538811831607"></a>安全组的id</p>
<p id="p7631141813810"><a name="p7631141813810"></a><a name="p7631141813810"></a>使用说明：查询安全组列表非必选</p>
</td>
</tr>
<tr id="row487759591607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p499705331607"><a name="p499705331607"></a><a name="p499705331607"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p26621541607"><a name="p26621541607"></a><a name="p26621541607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row356666781607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p270644691607"><a name="p270644691607"></a><a name="p270644691607"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p426717071607"><a name="p426717071607"></a><a name="p426717071607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p29740751607"><a name="p29740751607"></a><a name="p29740751607"></a>安全组名称</p>
</td>
</tr>
<tr id="row5261561607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p76095411607"><a name="p76095411607"></a><a name="p76095411607"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p597100051607"><a name="p597100051607"></a><a name="p597100051607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p40269061607"><a name="p40269061607"></a><a name="p40269061607"></a>安全组描述</p>
</td>
</tr>
<tr id="row141788771607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p574773991607"><a name="p574773991607"></a><a name="p574773991607"></a>security_group_rules</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p263715271607"><a name="p263715271607"></a><a name="p263715271607"></a>Array of <a href="#table655457801607">Security Group Rule</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p577222241607"><a name="p577222241607"></a><a name="p577222241607"></a>security_group_rule列表，参见<a href="#table655457801607">表4</a></p>
</td>
</tr>
<tr id="row19560720141817"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p15700614790"><a name="p15700614790"></a><a name="p15700614790"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p8746620183014"><a name="p8746620183014"></a><a name="p8746620183014"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row5768162761818"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间，UTC时间</p>
<p id="p65980291419"><a name="p65980291419"></a><a name="p65980291419"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row4242824111816"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间，UTC时间</p>
<p id="p15297192516128"><a name="p15297192516128"></a><a name="p15297192516128"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

**表 4**  Security Group Rule对象

<a name="table655457801607"></a>
<table><thead align="left"><tr id="vpc_sg02_0006_row54478641607"><th class="cellrowborder" valign="top" width="26.669999999999998%" id="mcps1.2.4.1.1"><p id="vpc_sg02_0006_p389969021607"><a name="vpc_sg02_0006_p389969021607"></a><a name="vpc_sg02_0006_p389969021607"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.2"><p id="vpc_sg02_0006_p36789391607"><a name="vpc_sg02_0006_p36789391607"></a><a name="vpc_sg02_0006_p36789391607"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="vpc_sg02_0006_p433861031607"><a name="vpc_sg02_0006_p433861031607"></a><a name="vpc_sg02_0006_p433861031607"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_sg02_0006_row134774871607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p269083981607"><a name="vpc_sg02_0006_p269083981607"></a><a name="vpc_sg02_0006_p269083981607"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p630670281607"><a name="vpc_sg02_0006_p630670281607"></a><a name="vpc_sg02_0006_p630670281607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p334792201607"><a name="vpc_sg02_0006_p334792201607"></a><a name="vpc_sg02_0006_p334792201607"></a>安全组规则id</p>
<p id="vpc_sg02_0006_p529374054010"><a name="vpc_sg02_0006_p529374054010"></a><a name="vpc_sg02_0006_p529374054010"></a>使用说明：查询安全组规则非必选</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row250554771607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p254411021607"><a name="vpc_sg02_0006_p254411021607"></a><a name="vpc_sg02_0006_p254411021607"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p505368621607"><a name="vpc_sg02_0006_p505368621607"></a><a name="vpc_sg02_0006_p505368621607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p480145951607"><a name="vpc_sg02_0006_p480145951607"></a><a name="vpc_sg02_0006_p480145951607"></a>安全组规则描述</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row569401671607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p115724181607"><a name="vpc_sg02_0006_p115724181607"></a><a name="vpc_sg02_0006_p115724181607"></a>security_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p615991711607"><a name="vpc_sg02_0006_p615991711607"></a><a name="vpc_sg02_0006_p615991711607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p587796621607"><a name="vpc_sg02_0006_p587796621607"></a><a name="vpc_sg02_0006_p587796621607"></a>所属安全组id</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row654332091607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p113008931607"><a name="vpc_sg02_0006_p113008931607"></a><a name="vpc_sg02_0006_p113008931607"></a>remote_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p170542961607"><a name="vpc_sg02_0006_p170542961607"></a><a name="vpc_sg02_0006_p170542961607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p141218971607"><a name="vpc_sg02_0006_p141218971607"></a><a name="vpc_sg02_0006_p141218971607"></a>所属安全组的对端id</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row9932071607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p657989401607"><a name="vpc_sg02_0006_p657989401607"></a><a name="vpc_sg02_0006_p657989401607"></a>direction</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p507988391607"><a name="vpc_sg02_0006_p507988391607"></a><a name="vpc_sg02_0006_p507988391607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p570991491607"><a name="vpc_sg02_0006_p570991491607"></a><a name="vpc_sg02_0006_p570991491607"></a>规则方向</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row97529031607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p478834691607"><a name="vpc_sg02_0006_p478834691607"></a><a name="vpc_sg02_0006_p478834691607"></a>remote_ip_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p622759951607"><a name="vpc_sg02_0006_p622759951607"></a><a name="vpc_sg02_0006_p622759951607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p146708701607"><a name="vpc_sg02_0006_p146708701607"></a><a name="vpc_sg02_0006_p146708701607"></a>对端ip网段</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row315033981607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p163656291607"><a name="vpc_sg02_0006_p163656291607"></a><a name="vpc_sg02_0006_p163656291607"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p628340441607"><a name="vpc_sg02_0006_p628340441607"></a><a name="vpc_sg02_0006_p628340441607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p99902671607"><a name="vpc_sg02_0006_p99902671607"></a><a name="vpc_sg02_0006_p99902671607"></a>协议类型或直接指定IP协议号</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row551583771607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p97886331607"><a name="vpc_sg02_0006_p97886331607"></a><a name="vpc_sg02_0006_p97886331607"></a>port_range_max</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p343603851607"><a name="vpc_sg02_0006_p343603851607"></a><a name="vpc_sg02_0006_p343603851607"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p188144701607"><a name="vpc_sg02_0006_p188144701607"></a><a name="vpc_sg02_0006_p188144701607"></a>最大端口，当协议类型为ICMP时，该值表示ICMP的code</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row456604071607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p630384091607"><a name="vpc_sg02_0006_p630384091607"></a><a name="vpc_sg02_0006_p630384091607"></a>port_range_min</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p337362901607"><a name="vpc_sg02_0006_p337362901607"></a><a name="vpc_sg02_0006_p337362901607"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p258562691607"><a name="vpc_sg02_0006_p258562691607"></a><a name="vpc_sg02_0006_p258562691607"></a>最小端口，当协议类型为ICMP时，该值表示ICMP的type。</p>
<p id="vpc_sg02_0006_p5690808615417"><a name="vpc_sg02_0006_p5690808615417"></a><a name="vpc_sg02_0006_p5690808615417"></a>protocol为tcp和udp时，port_range_max和port_range_min必须同时输入，且port_range_max应大于等于port_range_min。</p>
<p id="vpc_sg02_0006_p4241072615417"><a name="vpc_sg02_0006_p4241072615417"></a><a name="vpc_sg02_0006_p4241072615417"></a>protocol为icmp时，指定ICMP code（port_range_max）时，必须同时指定ICMP type（port_range_min）。</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row360773491607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p364292801607"><a name="vpc_sg02_0006_p364292801607"></a><a name="vpc_sg02_0006_p364292801607"></a>ethertype</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p339523071607"><a name="vpc_sg02_0006_p339523071607"></a><a name="vpc_sg02_0006_p339523071607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p34728681607"><a name="vpc_sg02_0006_p34728681607"></a><a name="vpc_sg02_0006_p34728681607"></a>网络类型</p>
<p id="vpc_sg02_0006_p568898621607"><a name="vpc_sg02_0006_p568898621607"></a><a name="vpc_sg02_0006_p568898621607"></a>仅支持IPv4</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row532124261607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p593368391607"><a name="vpc_sg02_0006_p593368391607"></a><a name="vpc_sg02_0006_p593368391607"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p130282191607"><a name="vpc_sg02_0006_p130282191607"></a><a name="vpc_sg02_0006_p130282191607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p10487112"><a name="vpc_sg02_0006_p10487112"></a><a name="vpc_sg02_0006_p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row11992111863317"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p169261732143314"><a name="vpc_sg02_0006_p169261732143314"></a><a name="vpc_sg02_0006_p169261732143314"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p69311132153317"><a name="vpc_sg02_0006_p69311132153317"></a><a name="vpc_sg02_0006_p69311132153317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p13646103310"><a name="vpc_sg02_0006_p13646103310"></a><a name="vpc_sg02_0006_p13646103310"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row10903153923318"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p6634195714335"><a name="vpc_sg02_0006_p6634195714335"></a><a name="vpc_sg02_0006_p6634195714335"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p12638157153319"><a name="vpc_sg02_0006_p12638157153319"></a><a name="vpc_sg02_0006_p12638157153319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p1364635713332"><a name="vpc_sg02_0006_p1364635713332"></a><a name="vpc_sg02_0006_p1364635713332"></a>资源创建时间，UTC时间</p>
<p id="vpc_sg02_0006_p65980291419"><a name="vpc_sg02_0006_p65980291419"></a><a name="vpc_sg02_0006_p65980291419"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="vpc_sg02_0006_row1797311427338"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="vpc_sg02_0006_p1725445103416"><a name="vpc_sg02_0006_p1725445103416"></a><a name="vpc_sg02_0006_p1725445103416"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="vpc_sg02_0006_p192601514345"><a name="vpc_sg02_0006_p192601514345"></a><a name="vpc_sg02_0006_p192601514345"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="vpc_sg02_0006_p1127018513343"><a name="vpc_sg02_0006_p1127018513343"></a><a name="vpc_sg02_0006_p1127018513343"></a>资源更新时间，UTC时间</p>
<p id="vpc_sg02_0006_p19850105451210"><a name="vpc_sg02_0006_p19850105451210"></a><a name="vpc_sg02_0006_p19850105451210"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section2440368716037"></a>

请求样例

```
GET https://{Endpoint}/v2.0/security-groups?limit=1
```

响应样例

```
{
    "security_groups": [
        {
            "id": "0431c9c5-1660-42e0-8a00-134bec7f03e2",
            "name": "sg-ad3f",
            "description": "",
            "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
            "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
            "security_group_rules": [
                {
                    "id": "d90e55ba-23bd-4d97-b722-8cb6fb485d69",
                    "direction": "ingress",
                    "protocol": null,
                    "ethertype": "IPv4",
                    "description": null,
                    "remote_group_id": "0431c9c5-1660-42e0-8a00-134bec7f03e2",
                    "remote_ip_prefix": null,
                    "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
                    "port_range_max": null,
                    "port_range_min": null,
                    "security_group_id": "0431c9c5-1660-42e0-8a00-134bec7f03e2"
                    
                },
                {
                    "id": "aecff4d4-9ce9-489c-86a3-803aedec65f7",
                    "direction": "egress",
                    "protocol": null,
                    "ethertype": "IPv4",
                    "description": null,
                    "remote_group_id": null,
                    "remote_ip_prefix": null,
                    "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
                    "port_range_max": null,
                    "port_range_min": null,
                    "security_group_id": "0431c9c5-1660-42e0-8a00-134bec7f03e2"
                }
            ],
            "created_at": "2018-09-12T08:24:14",
            "updated_at": "2018-09-12T08:24:14"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

