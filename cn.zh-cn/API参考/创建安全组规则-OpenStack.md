# 创建安全组规则<a name="vpc_sg02_0008"></a>

## 功能介绍<a name="section5958580616319"></a>

创建安全组规则。

## URI<a name="section6291358016319"></a>

POST /v2.0/security-group-rules

## 请求消息<a name="section3953869316319"></a>

**表 1**  请求参数

<a name="table981991416319"></a>
<table><thead align="left"><tr id="row191482716319"><th class="cellrowborder" valign="top" width="26.52734726527347%" id="mcps1.2.5.1.1"><p id="p2280026616319"><a name="p2280026616319"></a><a name="p2280026616319"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.5.1.2"><p id="p1835529716319"><a name="p1835529716319"></a><a name="p1835529716319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p3464228716319"><a name="p3464228716319"></a><a name="p3464228716319"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p3284526816319"><a name="p3284526816319"></a><a name="p3284526816319"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3793835116319"><td class="cellrowborder" valign="top" width="26.52734726527347%" headers="mcps1.2.5.1.1 "><p id="p4303593816319"><a name="p4303593816319"></a><a name="p4303593816319"></a>security_group_rule</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p3852346816319"><a name="p3852346816319"></a><a name="p3852346816319"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p6530542116319"><a name="p6530542116319"></a><a name="p6530542116319"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p732393116218"><a name="p732393116218"></a><a name="p732393116218"></a>security group rule对象列表。请参见<a href="#table655457801607">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Security Group Rule对象

<a name="table655457801607"></a>
<table><thead align="left"><tr id="row54478641607"><th class="cellrowborder" valign="top" width="23.54%" id="mcps1.2.5.1.1"><p id="p389969021607"><a name="p389969021607"></a><a name="p389969021607"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="11.72%" id="mcps1.2.5.1.2"><p id="p07415175392"><a name="p07415175392"></a><a name="p07415175392"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.599999999999998%" id="mcps1.2.5.1.3"><p id="p36789391607"><a name="p36789391607"></a><a name="p36789391607"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.14%" id="mcps1.2.5.1.4"><p id="p433861031607"><a name="p433861031607"></a><a name="p433861031607"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row250554771607"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p254411021607"><a name="p254411021607"></a><a name="p254411021607"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="11.72%" headers="mcps1.2.5.1.2 "><p id="p27411717193910"><a name="p27411717193910"></a><a name="p27411717193910"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p505368621607"><a name="p505368621607"></a><a name="p505368621607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.14%" headers="mcps1.2.5.1.4 "><p id="p480145951607"><a name="p480145951607"></a><a name="p480145951607"></a>安全组规则描述</p>
</td>
</tr>
<tr id="row569401671607"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p115724181607"><a name="p115724181607"></a><a name="p115724181607"></a>security_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.72%" headers="mcps1.2.5.1.2 "><p id="p10741111717399"><a name="p10741111717399"></a><a name="p10741111717399"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p615991711607"><a name="p615991711607"></a><a name="p615991711607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.14%" headers="mcps1.2.5.1.4 "><p id="p587796621607"><a name="p587796621607"></a><a name="p587796621607"></a>所属安全组id</p>
</td>
</tr>
<tr id="row654332091607"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p113008931607"><a name="p113008931607"></a><a name="p113008931607"></a>remote_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.72%" headers="mcps1.2.5.1.2 "><p id="p374111793919"><a name="p374111793919"></a><a name="p374111793919"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p170542961607"><a name="p170542961607"></a><a name="p170542961607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.14%" headers="mcps1.2.5.1.4 "><p id="p141218971607"><a name="p141218971607"></a><a name="p141218971607"></a>所属安全组的对端id</p>
<p id="p1511685411396"><a name="p1511685411396"></a><a name="p1511685411396"></a>使用说明：和remote_ip_prefix参数二选一</p>
</td>
</tr>
<tr id="row9932071607"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p657989401607"><a name="p657989401607"></a><a name="p657989401607"></a>direction</p>
</td>
<td class="cellrowborder" valign="top" width="11.72%" headers="mcps1.2.5.1.2 "><p id="p19741111723910"><a name="p19741111723910"></a><a name="p19741111723910"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p507988391607"><a name="p507988391607"></a><a name="p507988391607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.14%" headers="mcps1.2.5.1.4 "><p id="p570991491607"><a name="p570991491607"></a><a name="p570991491607"></a>规则方向</p>
<p id="p13943922124015"><a name="p13943922124015"></a><a name="p13943922124015"></a>取值范围：ingress（入方向）/egress（出方向）</p>
</td>
</tr>
<tr id="row97529031607"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p478834691607"><a name="p478834691607"></a><a name="p478834691607"></a>remote_ip_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="11.72%" headers="mcps1.2.5.1.2 "><p id="p1574110175393"><a name="p1574110175393"></a><a name="p1574110175393"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p622759951607"><a name="p622759951607"></a><a name="p622759951607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.14%" headers="mcps1.2.5.1.4 "><p id="p146708701607"><a name="p146708701607"></a><a name="p146708701607"></a>对端ip网段</p>
<p id="p1238771033815"><a name="p1238771033815"></a><a name="p1238771033815"></a>使用说明：和remote_group_id参数二选一</p>
</td>
</tr>
<tr id="row315033981607"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p163656291607"><a name="p163656291607"></a><a name="p163656291607"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="11.72%" headers="mcps1.2.5.1.2 "><p id="p07411217183920"><a name="p07411217183920"></a><a name="p07411217183920"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p628340441607"><a name="p628340441607"></a><a name="p628340441607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.14%" headers="mcps1.2.5.1.4 "><p id="p99902671607"><a name="p99902671607"></a><a name="p99902671607"></a>协议类型或直接指定IP协议号</p>
<p id="p6125143124117"><a name="p6125143124117"></a><a name="p6125143124117"></a>取值范围：tcp/udp/icmp或IP协议号</p>
</td>
</tr>
<tr id="row551583771607"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p97886331607"><a name="p97886331607"></a><a name="p97886331607"></a>port_range_max</p>
</td>
<td class="cellrowborder" valign="top" width="11.72%" headers="mcps1.2.5.1.2 "><p id="p8741717103914"><a name="p8741717103914"></a><a name="p8741717103914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p343603851607"><a name="p343603851607"></a><a name="p343603851607"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.14%" headers="mcps1.2.5.1.4 "><p id="p188144701607"><a name="p188144701607"></a><a name="p188144701607"></a>最大端口，当协议类型为ICMP时，该值表示ICMP的code</p>
<p id="p1354926164118"><a name="p1354926164118"></a><a name="p1354926164118"></a>取值范围：1-65535（当表示code时为0-255）</p>
</td>
</tr>
<tr id="row456604071607"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p630384091607"><a name="p630384091607"></a><a name="p630384091607"></a>port_range_min</p>
</td>
<td class="cellrowborder" valign="top" width="11.72%" headers="mcps1.2.5.1.2 "><p id="p137411517143913"><a name="p137411517143913"></a><a name="p137411517143913"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p337362901607"><a name="p337362901607"></a><a name="p337362901607"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.14%" headers="mcps1.2.5.1.4 "><p id="p258562691607"><a name="p258562691607"></a><a name="p258562691607"></a>最小端口，当协议类型为ICMP时，该值表示ICMP的type。</p>
<p id="p5690808615417"><a name="p5690808615417"></a><a name="p5690808615417"></a>protocol为tcp和udp时，port_range_max和port_range_min必须同时输入，且port_range_max应大于等于port_range_min。</p>
<p id="p4241072615417"><a name="p4241072615417"></a><a name="p4241072615417"></a>protocol为icmp时，指定ICMP code（port_range_max）时，必须同时指定ICMP type（port_range_min）。</p>
<p id="p543313212446"><a name="p543313212446"></a><a name="p543313212446"></a>取值范围：1-65535（当表示code时为0-255）</p>
</td>
</tr>
<tr id="row360773491607"><td class="cellrowborder" valign="top" width="23.54%" headers="mcps1.2.5.1.1 "><p id="p364292801607"><a name="p364292801607"></a><a name="p364292801607"></a>ethertype</p>
</td>
<td class="cellrowborder" valign="top" width="11.72%" headers="mcps1.2.5.1.2 "><p id="p15741131719393"><a name="p15741131719393"></a><a name="p15741131719393"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.599999999999998%" headers="mcps1.2.5.1.3 "><p id="p339523071607"><a name="p339523071607"></a><a name="p339523071607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.14%" headers="mcps1.2.5.1.4 "><p id="p34728681607"><a name="p34728681607"></a><a name="p34728681607"></a>网络类型</p>
<p id="p668771714614"><a name="p668771714614"></a><a name="p668771714614"></a>取值范围：IPv4/IPv6</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section2023987716319"></a>

**表 3**  响应参数

<a name="table676552316319"></a>
<table><thead align="left"><tr id="row5032047016319"><th class="cellrowborder" valign="top" width="31.7%" id="mcps1.2.4.1.1"><p id="p4182747116319"><a name="p4182747116319"></a><a name="p4182747116319"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.080000000000002%" id="mcps1.2.4.1.2"><p id="p4264467116319"><a name="p4264467116319"></a><a name="p4264467116319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p4267558716319"><a name="p4267558716319"></a><a name="p4267558716319"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row60629616319"><td class="cellrowborder" valign="top" width="31.7%" headers="mcps1.2.4.1.1 "><p id="p2428304416319"><a name="p2428304416319"></a><a name="p2428304416319"></a>security_group_rule</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.4.1.2 "><p id="p2724314316319"><a name="p2724314316319"></a><a name="p2724314316319"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p5745755316319"><a name="p5745755316319"></a><a name="p5745755316319"></a>security group rule对象列表。请参见<a href="#table1794215178501">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  Security Group Rule对象

<a name="table1794215178501"></a>
<table><thead align="left"><tr id="row594401765012"><th class="cellrowborder" valign="top" width="26.669999999999998%" id="mcps1.2.4.1.1"><p id="p79441917145016"><a name="p79441917145016"></a><a name="p79441917145016"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.2"><p id="p189449173501"><a name="p189449173501"></a><a name="p189449173501"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="p14944151714502"><a name="p14944151714502"></a><a name="p14944151714502"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row134774871607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p269083981607"><a name="p269083981607"></a><a name="p269083981607"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p630670281607"><a name="p630670281607"></a><a name="p630670281607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p334792201607"><a name="p334792201607"></a><a name="p334792201607"></a>安全组规则id</p>
<p id="p529374054010"><a name="p529374054010"></a><a name="p529374054010"></a>使用说明：查询安全组规则非必选</p>
</td>
</tr>
<tr id="row15944617165015"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p149461217195012"><a name="p149461217195012"></a><a name="p149461217195012"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p294641745013"><a name="p294641745013"></a><a name="p294641745013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p19946917105019"><a name="p19946917105019"></a><a name="p19946917105019"></a>安全组规则描述</p>
</td>
</tr>
<tr id="row894618172509"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p149461917175015"><a name="p149461917175015"></a><a name="p149461917175015"></a>security_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p179460179503"><a name="p179460179503"></a><a name="p179460179503"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p59471117115010"><a name="p59471117115010"></a><a name="p59471117115010"></a>所属安全组id</p>
</td>
</tr>
<tr id="row494711765015"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p5947517135014"><a name="p5947517135014"></a><a name="p5947517135014"></a>remote_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p18947817175013"><a name="p18947817175013"></a><a name="p18947817175013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p194821775015"><a name="p194821775015"></a><a name="p194821775015"></a>所属安全组的对端id</p>
</td>
</tr>
<tr id="row1394891775017"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p189481171504"><a name="p189481171504"></a><a name="p189481171504"></a>direction</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p99481417185012"><a name="p99481417185012"></a><a name="p99481417185012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1694851720506"><a name="p1694851720506"></a><a name="p1694851720506"></a>规则方向</p>
</td>
</tr>
<tr id="row1994812173503"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p1294831745014"><a name="p1294831745014"></a><a name="p1294831745014"></a>remote_ip_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p19948171725018"><a name="p19948171725018"></a><a name="p19948171725018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p694881717507"><a name="p694881717507"></a><a name="p694881717507"></a>对端ip网段</p>
</td>
</tr>
<tr id="row3948181714504"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p59488172505"><a name="p59488172505"></a><a name="p59488172505"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p69481317155019"><a name="p69481317155019"></a><a name="p69481317155019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1094871718506"><a name="p1094871718506"></a><a name="p1094871718506"></a>协议类型或直接指定IP协议号</p>
</td>
</tr>
<tr id="row189481317185015"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p14948417155013"><a name="p14948417155013"></a><a name="p14948417155013"></a>port_range_max</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p29484172505"><a name="p29484172505"></a><a name="p29484172505"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p8948417135013"><a name="p8948417135013"></a><a name="p8948417135013"></a>最大端口，当协议类型为ICMP时，该值表示ICMP的code</p>
</td>
</tr>
<tr id="row10948131795018"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p13948191705018"><a name="p13948191705018"></a><a name="p13948191705018"></a>port_range_min</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p89497176506"><a name="p89497176506"></a><a name="p89497176506"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p4949191713509"><a name="p4949191713509"></a><a name="p4949191713509"></a>最小端口，当协议类型为ICMP时，该值表示ICMP的type。</p>
<p id="p594916176501"><a name="p594916176501"></a><a name="p594916176501"></a>protocol为tcp和udp时，port_range_max和port_range_min必须同时输入，且port_range_max应大于等于port_range_min。</p>
<p id="p189494172509"><a name="p189494172509"></a><a name="p189494172509"></a>protocol为icmp时，指定ICMP code（port_range_max）时，必须同时指定ICMP type（port_range_min）。</p>
</td>
</tr>
<tr id="row159491817195016"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p89491817165011"><a name="p89491817165011"></a><a name="p89491817165011"></a>ethertype</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p5949617125012"><a name="p5949617125012"></a><a name="p5949617125012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1894915178504"><a name="p1894915178504"></a><a name="p1894915178504"></a>网络类型</p>
<p id="p1594961712508"><a name="p1594961712508"></a><a name="p1594961712508"></a>仅支持IPv4</p>
</td>
</tr>
<tr id="row532124261607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p593368391607"><a name="p593368391607"></a><a name="p593368391607"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p130282191607"><a name="p130282191607"></a><a name="p130282191607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row11992111863317"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p169261732143314"><a name="p169261732143314"></a><a name="p169261732143314"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p69311132153317"><a name="p69311132153317"></a><a name="p69311132153317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p103844191312"><a name="p103844191312"></a><a name="p103844191312"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row10903153923318"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p6634195714335"><a name="p6634195714335"></a><a name="p6634195714335"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p12638157153319"><a name="p12638157153319"></a><a name="p12638157153319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1364635713332"><a name="p1364635713332"></a><a name="p1364635713332"></a>资源创建时间，UTC时间</p>
<p id="p65980291419"><a name="p65980291419"></a><a name="p65980291419"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row1797311427338"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p1725445103416"><a name="p1725445103416"></a><a name="p1725445103416"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p192601514345"><a name="p192601514345"></a><a name="p192601514345"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1127018513343"><a name="p1127018513343"></a><a name="p1127018513343"></a>资源更新时间，UTC时间</p>
<p id="p11481521141510"><a name="p11481521141510"></a><a name="p11481521141510"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section5025263616319"></a>

请求样例

```
POST https://{Endpoint}/v2.0/security-group-rules

{
    "security_group_rule": {
        "security_group_id": "5cb9c1ee-00e0-4d0f-9623-55463cd26ff8", 
        "direction": "egress", 
        "protocol": "tcp", 
        "remote_ip_prefix": "10.10.0.0/24"
    }
}
```

响应样例

```
{
    "security_group_rule": {
        "remote_group_id": null, 
        "direction": "egress", 
        "remote_ip_prefix": "10.10.0.0/24", 
        "protocol": "tcp", 
        "tenant_id": "6fbe9263116a4b68818cf1edce16bc4f", 
        "port_range_max": null, 
        "security_group_id": "5cb9c1ee-00e0-4d0f-9623-55463cd26ff8", 
        "port_range_min": null, 
        "ethertype": "IPv4", 
        "description": null, 
        "id": "7c336b04-1603-4911-a6f4-f2af1d9a0488",
        "project_id": "6fbe9263116a4b68818cf1edce16bc4f", 
        "created_at": "2018-09-20T02:15:34",
        "updated_at": "2018-09-20T02:15:34"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

