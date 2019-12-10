# 创建安全组<a name="ZH-CN_TOPIC_0201534171"></a>

## 功能介绍<a name="section3720668916116"></a>

创建安全组。

## URI<a name="section745182516116"></a>

POST /v2.0/security-groups

## 请求消息<a name="section4818631316116"></a>

**表 1**  请求参数

<a name="table3697372616116"></a>
<table><thead align="left"><tr id="row2546787016116"><th class="cellrowborder" valign="top" width="14.44%" id="mcps1.2.5.1.1"><p id="p5679273516116"><a name="p5679273516116"></a><a name="p5679273516116"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="9.9%" id="mcps1.2.5.1.2"><p id="p1571843716116"><a name="p1571843716116"></a><a name="p1571843716116"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.549999999999999%" id="mcps1.2.5.1.3"><p id="p805282316116"><a name="p805282316116"></a><a name="p805282316116"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.11%" id="mcps1.2.5.1.4"><p id="p5322986716116"><a name="p5322986716116"></a><a name="p5322986716116"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1360551216116"><td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.1 "><p id="p5104828416116"><a name="p5104828416116"></a><a name="p5104828416116"></a>security_group</p>
</td>
<td class="cellrowborder" valign="top" width="9.9%" headers="mcps1.2.5.1.2 "><p id="p3558909616116"><a name="p3558909616116"></a><a name="p3558909616116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.549999999999999%" headers="mcps1.2.5.1.3 "><p id="p714515916116"><a name="p714515916116"></a><a name="p714515916116"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="61.11%" headers="mcps1.2.5.1.4 "><p id="p4305865716116"><a name="p4305865716116"></a><a name="p4305865716116"></a>security group对象列表。请参见<a href="#table513726041607">表2</a></p>
</td>
</tr>
</tbody>
</table>

**表 2**  Security Group对象

<a name="table513726041607"></a>
<table><thead align="left"><tr id="row72893461607"><th class="cellrowborder" valign="top" width="14.31%" id="mcps1.2.5.1.1"><p id="p647825491607"><a name="p647825491607"></a><a name="p647825491607"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="8.959999999999999%" id="mcps1.2.5.1.2"><p id="p1075015422371"><a name="p1075015422371"></a><a name="p1075015422371"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.66%" id="mcps1.2.5.1.3"><p id="p245230881607"><a name="p245230881607"></a><a name="p245230881607"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="62.07%" id="mcps1.2.5.1.4"><p id="p4542071607"><a name="p4542071607"></a><a name="p4542071607"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row356666781607"><td class="cellrowborder" valign="top" width="14.31%" headers="mcps1.2.5.1.1 "><p id="p270644691607"><a name="p270644691607"></a><a name="p270644691607"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="8.959999999999999%" headers="mcps1.2.5.1.2 "><p id="p87501142163712"><a name="p87501142163712"></a><a name="p87501142163712"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.5.1.3 "><p id="p426717071607"><a name="p426717071607"></a><a name="p426717071607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.5.1.4 "><p id="p29740751607"><a name="p29740751607"></a><a name="p29740751607"></a>安全组名称</p>
</td>
</tr>
<tr id="row5261561607"><td class="cellrowborder" valign="top" width="14.31%" headers="mcps1.2.5.1.1 "><p id="p76095411607"><a name="p76095411607"></a><a name="p76095411607"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="8.959999999999999%" headers="mcps1.2.5.1.2 "><p id="p11750124243714"><a name="p11750124243714"></a><a name="p11750124243714"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.5.1.3 "><p id="p597100051607"><a name="p597100051607"></a><a name="p597100051607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.07%" headers="mcps1.2.5.1.4 "><p id="p40269061607"><a name="p40269061607"></a><a name="p40269061607"></a>安全组描述</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section2285655116116"></a>

**表 3**  响应参数

<a name="table6597002216116"></a>
<table><thead align="left"><tr id="row3852245716116"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p5239237116116"><a name="p5239237116116"></a><a name="p5239237116116"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p5702934716116"><a name="p5702934716116"></a><a name="p5702934716116"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p5255764216116"><a name="p5255764216116"></a><a name="p5255764216116"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1989548816116"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p3843802816116"><a name="p3843802816116"></a><a name="p3843802816116"></a>security_group</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p4806907216116"><a name="p4806907216116"></a><a name="p4806907216116"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p944057316116"><a name="p944057316116"></a><a name="p944057316116"></a>security group对象列表。请参见<a href="#table32081555104215">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  Security Group对象

<a name="table32081555104215"></a>
<table><thead align="left"><tr id="row11209155574211"><th class="cellrowborder" valign="top" width="26.669999999999998%" id="mcps1.2.4.1.1"><p id="p8209855204216"><a name="p8209855204216"></a><a name="p8209855204216"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.2"><p id="p6209455164212"><a name="p6209455164212"></a><a name="p6209455164212"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="p220935519423"><a name="p220935519423"></a><a name="p220935519423"></a>说明</p>
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
<tr id="row202102055194211"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p0210165544220"><a name="p0210165544220"></a><a name="p0210165544220"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p9210155544212"><a name="p9210155544212"></a><a name="p9210155544212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p921095512423"><a name="p921095512423"></a><a name="p921095512423"></a>安全组名称</p>
</td>
</tr>
<tr id="row20210455144220"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p121012559426"><a name="p121012559426"></a><a name="p121012559426"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p1221011557421"><a name="p1221011557421"></a><a name="p1221011557421"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p521018559423"><a name="p521018559423"></a><a name="p521018559423"></a>安全组描述</p>
</td>
</tr>
<tr id="row141788771607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p574773991607"><a name="p574773991607"></a><a name="p574773991607"></a>security_group_rules</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p263715271607"><a name="p263715271607"></a><a name="p263715271607"></a>Array of <a href="#table655457801607">Security Group Rule</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p577222241607"><a name="p577222241607"></a><a name="p577222241607"></a>security_group_rule列表，参见<a href="#table655457801607">表5</a></p>
</td>
</tr>
<tr id="row19560720141817"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p15700614790"><a name="p15700614790"></a><a name="p15700614790"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p13953143814304"><a name="p13953143814304"></a><a name="p13953143814304"></a>项目ID</p>
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
<p id="p48631659131118"><a name="p48631659131118"></a><a name="p48631659131118"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

**表 5**  Security Group Rule对象

<a name="table655457801607"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534086_row54478641607"><th class="cellrowborder" valign="top" width="26.669999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534086_p389969021607"><a name="zh-cn_topic_0201534086_p389969021607"></a><a name="zh-cn_topic_0201534086_p389969021607"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534086_p36789391607"><a name="zh-cn_topic_0201534086_p36789391607"></a><a name="zh-cn_topic_0201534086_p36789391607"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534086_p433861031607"><a name="zh-cn_topic_0201534086_p433861031607"></a><a name="zh-cn_topic_0201534086_p433861031607"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534086_row134774871607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p269083981607"><a name="zh-cn_topic_0201534086_p269083981607"></a><a name="zh-cn_topic_0201534086_p269083981607"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p630670281607"><a name="zh-cn_topic_0201534086_p630670281607"></a><a name="zh-cn_topic_0201534086_p630670281607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p334792201607"><a name="zh-cn_topic_0201534086_p334792201607"></a><a name="zh-cn_topic_0201534086_p334792201607"></a>安全组规则id</p>
<p id="zh-cn_topic_0201534086_p529374054010"><a name="zh-cn_topic_0201534086_p529374054010"></a><a name="zh-cn_topic_0201534086_p529374054010"></a>使用说明：查询安全组规则非必选</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row250554771607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p254411021607"><a name="zh-cn_topic_0201534086_p254411021607"></a><a name="zh-cn_topic_0201534086_p254411021607"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p505368621607"><a name="zh-cn_topic_0201534086_p505368621607"></a><a name="zh-cn_topic_0201534086_p505368621607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p480145951607"><a name="zh-cn_topic_0201534086_p480145951607"></a><a name="zh-cn_topic_0201534086_p480145951607"></a>安全组规则描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row569401671607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p115724181607"><a name="zh-cn_topic_0201534086_p115724181607"></a><a name="zh-cn_topic_0201534086_p115724181607"></a>security_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p615991711607"><a name="zh-cn_topic_0201534086_p615991711607"></a><a name="zh-cn_topic_0201534086_p615991711607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p587796621607"><a name="zh-cn_topic_0201534086_p587796621607"></a><a name="zh-cn_topic_0201534086_p587796621607"></a>所属安全组id</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row654332091607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p113008931607"><a name="zh-cn_topic_0201534086_p113008931607"></a><a name="zh-cn_topic_0201534086_p113008931607"></a>remote_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p170542961607"><a name="zh-cn_topic_0201534086_p170542961607"></a><a name="zh-cn_topic_0201534086_p170542961607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p141218971607"><a name="zh-cn_topic_0201534086_p141218971607"></a><a name="zh-cn_topic_0201534086_p141218971607"></a>所属安全组的对端id</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row9932071607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p657989401607"><a name="zh-cn_topic_0201534086_p657989401607"></a><a name="zh-cn_topic_0201534086_p657989401607"></a>direction</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p507988391607"><a name="zh-cn_topic_0201534086_p507988391607"></a><a name="zh-cn_topic_0201534086_p507988391607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p570991491607"><a name="zh-cn_topic_0201534086_p570991491607"></a><a name="zh-cn_topic_0201534086_p570991491607"></a>规则方向</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row97529031607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p478834691607"><a name="zh-cn_topic_0201534086_p478834691607"></a><a name="zh-cn_topic_0201534086_p478834691607"></a>remote_ip_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p622759951607"><a name="zh-cn_topic_0201534086_p622759951607"></a><a name="zh-cn_topic_0201534086_p622759951607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p146708701607"><a name="zh-cn_topic_0201534086_p146708701607"></a><a name="zh-cn_topic_0201534086_p146708701607"></a>对端ip网段</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row315033981607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p163656291607"><a name="zh-cn_topic_0201534086_p163656291607"></a><a name="zh-cn_topic_0201534086_p163656291607"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p628340441607"><a name="zh-cn_topic_0201534086_p628340441607"></a><a name="zh-cn_topic_0201534086_p628340441607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p99902671607"><a name="zh-cn_topic_0201534086_p99902671607"></a><a name="zh-cn_topic_0201534086_p99902671607"></a>协议类型或直接指定IP协议号</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row551583771607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p97886331607"><a name="zh-cn_topic_0201534086_p97886331607"></a><a name="zh-cn_topic_0201534086_p97886331607"></a>port_range_max</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p343603851607"><a name="zh-cn_topic_0201534086_p343603851607"></a><a name="zh-cn_topic_0201534086_p343603851607"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p188144701607"><a name="zh-cn_topic_0201534086_p188144701607"></a><a name="zh-cn_topic_0201534086_p188144701607"></a>最大端口，当协议类型为ICMP时，该值表示ICMP的code</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row456604071607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p630384091607"><a name="zh-cn_topic_0201534086_p630384091607"></a><a name="zh-cn_topic_0201534086_p630384091607"></a>port_range_min</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p337362901607"><a name="zh-cn_topic_0201534086_p337362901607"></a><a name="zh-cn_topic_0201534086_p337362901607"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p258562691607"><a name="zh-cn_topic_0201534086_p258562691607"></a><a name="zh-cn_topic_0201534086_p258562691607"></a>最小端口，当协议类型为ICMP时，该值表示ICMP的type。</p>
<p id="zh-cn_topic_0201534086_p5690808615417"><a name="zh-cn_topic_0201534086_p5690808615417"></a><a name="zh-cn_topic_0201534086_p5690808615417"></a>protocol为tcp和udp时，port_range_max和port_range_min必须同时输入，且port_range_max应大于等于port_range_min。</p>
<p id="zh-cn_topic_0201534086_p4241072615417"><a name="zh-cn_topic_0201534086_p4241072615417"></a><a name="zh-cn_topic_0201534086_p4241072615417"></a>protocol为icmp时，指定ICMP code（port_range_max）时，必须同时指定ICMP type（port_range_min）。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row360773491607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p364292801607"><a name="zh-cn_topic_0201534086_p364292801607"></a><a name="zh-cn_topic_0201534086_p364292801607"></a>ethertype</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p339523071607"><a name="zh-cn_topic_0201534086_p339523071607"></a><a name="zh-cn_topic_0201534086_p339523071607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p34728681607"><a name="zh-cn_topic_0201534086_p34728681607"></a><a name="zh-cn_topic_0201534086_p34728681607"></a>网络类型</p>
<p id="zh-cn_topic_0201534086_p568898621607"><a name="zh-cn_topic_0201534086_p568898621607"></a><a name="zh-cn_topic_0201534086_p568898621607"></a>仅支持IPv4</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row532124261607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p593368391607"><a name="zh-cn_topic_0201534086_p593368391607"></a><a name="zh-cn_topic_0201534086_p593368391607"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p130282191607"><a name="zh-cn_topic_0201534086_p130282191607"></a><a name="zh-cn_topic_0201534086_p130282191607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p10487112"><a name="zh-cn_topic_0201534086_p10487112"></a><a name="zh-cn_topic_0201534086_p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row11992111863317"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p169261732143314"><a name="zh-cn_topic_0201534086_p169261732143314"></a><a name="zh-cn_topic_0201534086_p169261732143314"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p69311132153317"><a name="zh-cn_topic_0201534086_p69311132153317"></a><a name="zh-cn_topic_0201534086_p69311132153317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p13646103310"><a name="zh-cn_topic_0201534086_p13646103310"></a><a name="zh-cn_topic_0201534086_p13646103310"></a>项目ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row10903153923318"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p6634195714335"><a name="zh-cn_topic_0201534086_p6634195714335"></a><a name="zh-cn_topic_0201534086_p6634195714335"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p12638157153319"><a name="zh-cn_topic_0201534086_p12638157153319"></a><a name="zh-cn_topic_0201534086_p12638157153319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p1364635713332"><a name="zh-cn_topic_0201534086_p1364635713332"></a><a name="zh-cn_topic_0201534086_p1364635713332"></a>资源创建时间，UTC时间</p>
<p id="zh-cn_topic_0201534086_p65980291419"><a name="zh-cn_topic_0201534086_p65980291419"></a><a name="zh-cn_topic_0201534086_p65980291419"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534086_row1797311427338"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534086_p1725445103416"><a name="zh-cn_topic_0201534086_p1725445103416"></a><a name="zh-cn_topic_0201534086_p1725445103416"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534086_p192601514345"><a name="zh-cn_topic_0201534086_p192601514345"></a><a name="zh-cn_topic_0201534086_p192601514345"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534086_p1127018513343"><a name="zh-cn_topic_0201534086_p1127018513343"></a><a name="zh-cn_topic_0201534086_p1127018513343"></a>资源更新时间，UTC时间</p>
<p id="zh-cn_topic_0201534086_p19850105451210"><a name="zh-cn_topic_0201534086_p19850105451210"></a><a name="zh-cn_topic_0201534086_p19850105451210"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section6015182016116"></a>

请求样例

```
POST https://{Endpoint}/v2.0/security-groups 

{
    "security_group": {
           "name": "sg-test"
    }
}
```

响应样例

```
{
    "security_group": {
        "id": "d29ae17d-f355-4992-8747-1fb66cc9afd2",
        "name": "sg-test",
        "description": "",
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "security_group_rules": [
            {
                "id": "3f51e52c-0e85-40f7-a137-85927392e436",
                "direction": "egress",
                "protocol": null,
                "ethertype": "IPv4",
                "description": null,
                "remote_group_id": null,
                "remote_ip_prefix": null,
                "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
                "port_range_max": null,
                "port_range_min": null,
                "security_group_id": "d29ae17d-f355-4992-8747-1fb66cc9afd2"
            },
            {
                "id": "6332de3e-98fb-4f8c-b44a-fcb8ff09881e",
                "direction": "egress",
                "protocol": null,
                "ethertype": "IPv6",
                "description": null,
                "remote_group_id": null,
                "remote_ip_prefix": null,
                "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
                "port_range_max": null,
                "port_range_min": null,
                "security_group_id": "d29ae17d-f355-4992-8747-1fb66cc9afd2"
            }
        ],
        "created_at": "2018-09-20T02:15:34",
        "updated_at": "2018-09-20T02:15:34"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

