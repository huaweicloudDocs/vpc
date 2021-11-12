# 更新子网<a name="vpc_subnet02_0004"></a>

## 功能介绍<a name="section10267951"></a>

更新子网。

接口约束：

更新allocation\_pools字段时范围不能包含网关和广播地址的所有IP。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=NeutronUpdateSubnet)中直接运行调试该接口。

## URI<a name="section25302698"></a>

PUT /v2.0/subnets/\{subnet\_id\}

## 请求消息<a name="section36252627"></a>

**表 1**  请求参数

<a name="table40701910"></a>
<table><thead align="left"><tr id="row5914937"><th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1"><p id="p9347893"><a name="p9347893"></a><a name="p9347893"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.16%" id="mcps1.2.5.1.2"><p id="p18981865"><a name="p18981865"></a><a name="p18981865"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.2%" id="mcps1.2.5.1.3"><p id="p61136126"><a name="p61136126"></a><a name="p61136126"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="67.35%" id="mcps1.2.5.1.4"><p id="p53079196"><a name="p53079196"></a><a name="p53079196"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4447594"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="p24710800"><a name="p24710800"></a><a name="p24710800"></a>subnet</p>
</td>
<td class="cellrowborder" valign="top" width="8.16%" headers="mcps1.2.5.1.2 "><p id="p55417783"><a name="p55417783"></a><a name="p55417783"></a><a href="#table12211980105515">subnet</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="10.2%" headers="mcps1.2.5.1.3 "><p id="p59655430"><a name="p59655430"></a><a name="p59655430"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.35%" headers="mcps1.2.5.1.4 "><p id="p37955333"><a name="p37955333"></a><a name="p37955333"></a>subnet对象列表，参见<a href="#table12211980105515">表2</a>。</p>
<p id="p2265180"><a name="p2265180"></a><a name="p2265180"></a>更新操作时至少指定一项属性</p>
</td>
</tr>
</tbody>
</table>

**表 2**  subnet对象

<a name="table12211980105515"></a>
<table><thead align="left"><tr id="row32722637105515"><th class="cellrowborder" valign="top" width="24.93%" id="mcps1.2.5.1.1"><p id="p60075710105815"><a name="p60075710105815"></a><a name="p60075710105815"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="12.02%" id="mcps1.2.5.1.2"><p id="p194182022104514"><a name="p194182022104514"></a><a name="p194182022104514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="24.93%" id="mcps1.2.5.1.3"><p id="p34294369105815"><a name="p34294369105815"></a><a name="p34294369105815"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.12%" id="mcps1.2.5.1.4"><p id="p25203839105815"><a name="p25203839105815"></a><a name="p25203839105815"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row43081158105515"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.1 "><p id="p54833166105624"><a name="p54833166105624"></a><a name="p54833166105624"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="12.02%" headers="mcps1.2.5.1.2 "><p id="p11418162219452"><a name="p11418162219452"></a><a name="p11418162219452"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.3 "><p id="p12301465105624"><a name="p12301465105624"></a><a name="p12301465105624"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.12%" headers="mcps1.2.5.1.4 "><p id="p14797472105624"><a name="p14797472105624"></a><a name="p14797472105624"></a>子网的名称</p>
</td>
</tr>
<tr id="row2545218105647"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.1 "><p id="p1395064410577"><a name="p1395064410577"></a><a name="p1395064410577"></a>allocation_pools</p>
</td>
<td class="cellrowborder" valign="top" width="12.02%" headers="mcps1.2.5.1.2 "><p id="p19418122284515"><a name="p19418122284515"></a><a name="p19418122284515"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.3 "><p id="p5626034310577"><a name="p5626034310577"></a><a name="p5626034310577"></a>Array of <a href="#table24611730">allocation_pool</a> objects</p>
<p id="p3658104710577"><a name="p3658104710577"></a><a name="p3658104710577"></a></p>
</td>
<td class="cellrowborder" valign="top" width="38.12%" headers="mcps1.2.5.1.4 "><p id="p2390980910577"><a name="p2390980910577"></a><a name="p2390980910577"></a>可用的IP池，allocation_pool对象参见<a href="#table24611730">表3</a></p>
<p id="p1386169010577"><a name="p1386169010577"></a><a name="p1386169010577"></a>例如：[ { "start": "10.0.0.2", "end": "10.0.0.251"} ]</p>
<p id="p1961191927"><a name="p1961191927"></a><a name="p1961191927"></a>每个子网的第1个和最后3个IP地址为系统保留地址。以192.168.1.0/24为例，192.168.1.0、 192.168.1.253、192.168.1.254和192.168.1.255这些地址是系统保留地址。系统预留地址默认不在allocation_pool范围内。</p>
<p id="p5764635410577"><a name="p5764635410577"></a><a name="p5764635410577"></a>约束：更新时allocation_pool范围不能包含网关和广播地址的所有IP。</p>
</td>
</tr>
<tr id="row22360302105653"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.1 "><p id="p1404384110577"><a name="p1404384110577"></a><a name="p1404384110577"></a>dns_nameservers</p>
</td>
<td class="cellrowborder" valign="top" width="12.02%" headers="mcps1.2.5.1.2 "><p id="p2418922154512"><a name="p2418922154512"></a><a name="p2418922154512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.3 "><p id="p6380932110577"><a name="p6380932110577"></a><a name="p6380932110577"></a>Array&nbsp;of&nbsp;strings</p>
</td>
<td class="cellrowborder" valign="top" width="38.12%" headers="mcps1.2.5.1.4 "><p id="p324929310577"><a name="p324929310577"></a><a name="p324929310577"></a>dns服务器</p>
<p id="p1218711851714"><a name="p1218711851714"></a><a name="p1218711851714"></a>【使用说明】</p>
<p id="p2924364410577"><a name="p2924364410577"></a><a name="p2924364410577"></a>例如："dns_nameservers": ["8.xx.xx.8","8.xx.xx.4"]</p>
<p id="p1294111141716"><a name="p1294111141716"></a><a name="p1294111141716"></a>最大为5个</p>
</td>
</tr>
<tr id="row17847900105653"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.1 "><p id="p4510693110577"><a name="p4510693110577"></a><a name="p4510693110577"></a>host_routes</p>
</td>
<td class="cellrowborder" valign="top" width="12.02%" headers="mcps1.2.5.1.2 "><p id="p3418112264518"><a name="p3418112264518"></a><a name="p3418112264518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.3 "><p id="p166911588244"><a name="p166911588244"></a><a name="p166911588244"></a>Array of <a href="#table5232330">host_route</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="38.12%" headers="mcps1.2.5.1.4 "><p id="p2002497710577"><a name="p2002497710577"></a><a name="p2002497710577"></a>虚拟机静态路由，参见<a href="#table5232330">表4</a></p>
<p id="p4600706610577"><a name="p4600706610577"></a><a name="p4600706610577"></a>【使用说明】不支持，忽略输入信息</p>
</td>
</tr>
<tr id="row21625046105653"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.1 "><p id="p4495318510577"><a name="p4495318510577"></a><a name="p4495318510577"></a>enable_dhcp</p>
</td>
<td class="cellrowborder" valign="top" width="12.02%" headers="mcps1.2.5.1.2 "><p id="p1041812214516"><a name="p1041812214516"></a><a name="p1041812214516"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.5.1.3 "><p id="p1732939410577"><a name="p1732939410577"></a><a name="p1732939410577"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="38.12%" headers="mcps1.2.5.1.4 "><p id="p2100438810577"><a name="p2100438810577"></a><a name="p2100438810577"></a>是否启动dhcp，false表示不提供dhcp服务的能力</p>
<p id="p5482176910577"><a name="p5482176910577"></a><a name="p5482176910577"></a>【使用说明】只支持true</p>
</td>
</tr>
</tbody>
</table>

**表 3**  allocation\_pool对象

<a name="table24611730"></a>
<table><thead align="left"><tr id="row15154020"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.2.5.1.1"><p id="p19516075"><a name="p19516075"></a><a name="p19516075"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="14.7%" id="mcps1.2.5.1.2"><p id="p1327122842316"><a name="p1327122842316"></a><a name="p1327122842316"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.78%" id="mcps1.2.5.1.3"><p id="p37298263"><a name="p37298263"></a><a name="p37298263"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="46.339999999999996%" id="mcps1.2.5.1.4"><p id="p15727687"><a name="p15727687"></a><a name="p15727687"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7331458"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.5.1.1 "><p id="p56977217"><a name="p56977217"></a><a name="p56977217"></a>start</p>
</td>
<td class="cellrowborder" valign="top" width="14.7%" headers="mcps1.2.5.1.2 "><p id="p227112286236"><a name="p227112286236"></a><a name="p227112286236"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.78%" headers="mcps1.2.5.1.3 "><p id="p51751889"><a name="p51751889"></a><a name="p51751889"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.339999999999996%" headers="mcps1.2.5.1.4 "><p id="p51610228"><a name="p51610228"></a><a name="p51610228"></a>网络池起始IP</p>
</td>
</tr>
<tr id="row61838871"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.2.5.1.1 "><p id="p42892680"><a name="p42892680"></a><a name="p42892680"></a>end</p>
</td>
<td class="cellrowborder" valign="top" width="14.7%" headers="mcps1.2.5.1.2 "><p id="p1727314281237"><a name="p1727314281237"></a><a name="p1727314281237"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.78%" headers="mcps1.2.5.1.3 "><p id="p51755094"><a name="p51755094"></a><a name="p51755094"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.339999999999996%" headers="mcps1.2.5.1.4 "><p id="p10006650"><a name="p10006650"></a><a name="p10006650"></a>网络池结束IP</p>
</td>
</tr>
</tbody>
</table>

**表 4**  host\_route对象

<a name="table5232330"></a>
<table><thead align="left"><tr id="row65973637"><th class="cellrowborder" valign="top" width="21.55%" id="mcps1.2.5.1.1"><p id="p42264412"><a name="p42264412"></a><a name="p42264412"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="14.649999999999999%" id="mcps1.2.5.1.2"><p id="p197406419246"><a name="p197406419246"></a><a name="p197406419246"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.63%" id="mcps1.2.5.1.3"><p id="p865310"><a name="p865310"></a><a name="p865310"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="47.17%" id="mcps1.2.5.1.4"><p id="p31641985"><a name="p31641985"></a><a name="p31641985"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16342414"><td class="cellrowborder" valign="top" width="21.55%" headers="mcps1.2.5.1.1 "><p id="p48667192"><a name="p48667192"></a><a name="p48667192"></a>destination</p>
</td>
<td class="cellrowborder" valign="top" width="14.649999999999999%" headers="mcps1.2.5.1.2 "><p id="p181671451247"><a name="p181671451247"></a><a name="p181671451247"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="p49728507"><a name="p49728507"></a><a name="p49728507"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.17%" headers="mcps1.2.5.1.4 "><p id="p28535525"><a name="p28535525"></a><a name="p28535525"></a>路由目的子网</p>
</td>
</tr>
<tr id="row55493137"><td class="cellrowborder" valign="top" width="21.55%" headers="mcps1.2.5.1.1 "><p id="p65759080"><a name="p65759080"></a><a name="p65759080"></a>nexthop</p>
</td>
<td class="cellrowborder" valign="top" width="14.649999999999999%" headers="mcps1.2.5.1.2 "><p id="p174054102412"><a name="p174054102412"></a><a name="p174054102412"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="p24885284"><a name="p24885284"></a><a name="p24885284"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.17%" headers="mcps1.2.5.1.4 "><p id="p51086148"><a name="p51086148"></a><a name="p51086148"></a>路由下一跳IP</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section57838187"></a>

**表 5**  响应参数

<a name="table49261880"></a>
<table><thead align="left"><tr id="row31386613"><th class="cellrowborder" valign="top" width="31.7%" id="mcps1.2.4.1.1"><p id="p59287744"><a name="p59287744"></a><a name="p59287744"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.080000000000002%" id="mcps1.2.4.1.2"><p id="p37577972"><a name="p37577972"></a><a name="p37577972"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p58217140"><a name="p58217140"></a><a name="p58217140"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17967889"><td class="cellrowborder" valign="top" width="31.7%" headers="mcps1.2.4.1.1 "><p id="p46112886"><a name="p46112886"></a><a name="p46112886"></a>subnet</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.4.1.2 "><p id="p44156300"><a name="p44156300"></a><a name="p44156300"></a><a href="#table176735992713">subnet</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p522217"><a name="p522217"></a><a name="p522217"></a>subnet对象列表，参见<a href="#table176735992713">表6</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 6**  subnet对象

<a name="table176735992713"></a>
<table><thead align="left"><tr id="row176713593276"><th class="cellrowborder" valign="top" width="28.332833283328334%" id="mcps1.2.4.1.1"><p id="p136755912715"><a name="p136755912715"></a><a name="p136755912715"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="28.332833283328334%" id="mcps1.2.4.1.2"><p id="p667105912718"><a name="p667105912718"></a><a name="p667105912718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.33433343334334%" id="mcps1.2.4.1.3"><p id="p26855915275"><a name="p26855915275"></a><a name="p26855915275"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row28303131105515"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p2014344105614"><a name="p2014344105614"></a><a name="p2014344105614"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p28944191105614"><a name="p28944191105614"></a><a name="p28944191105614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p53796361105614"><a name="p53796361105614"></a><a name="p53796361105614"></a>子网的id</p>
<p id="p2677113954519"><a name="p2677113954519"></a><a name="p2677113954519"></a>【使用说明】在查询子网列表时非必选</p>
</td>
</tr>
<tr id="row1868135972719"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p37015595272"><a name="p37015595272"></a><a name="p37015595272"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p18706591271"><a name="p18706591271"></a><a name="p18706591271"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p1870259172715"><a name="p1870259172715"></a><a name="p1870259172715"></a>子网的名称</p>
</td>
</tr>
<tr id="row670165910271"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p187012596279"><a name="p187012596279"></a><a name="p187012596279"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p137095922720"><a name="p137095922720"></a><a name="p137095922720"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p870155932715"><a name="p870155932715"></a><a name="p870155932715"></a>IP版本</p>
<p id="p10708598273"><a name="p10708598273"></a><a name="p10708598273"></a>【使用说明】只支持IPv4</p>
</td>
</tr>
<tr id="row1270135915274"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p1770105919271"><a name="p1770105919271"></a><a name="p1770105919271"></a>ipv6_address_mode</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p1370205912279"><a name="p1370205912279"></a><a name="p1370205912279"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p5701759142713"><a name="p5701759142713"></a><a name="p5701759142713"></a>IPv6寻址模式</p>
</td>
</tr>
<tr id="row57075913279"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p070195972715"><a name="p070195972715"></a><a name="p070195972715"></a>ipv6_ra_mode</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p1970559102716"><a name="p1970559102716"></a><a name="p1970559102716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p19701959152712"><a name="p19701959152712"></a><a name="p19701959152712"></a>IPv6路由广播模式</p>
</td>
</tr>
<tr id="row970185911274"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p5719599271"><a name="p5719599271"></a><a name="p5719599271"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p1671105982710"><a name="p1671105982710"></a><a name="p1671105982710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p1071259102716"><a name="p1071259102716"></a><a name="p1071259102716"></a>所属网络的id</p>
</td>
</tr>
<tr id="row9711659142718"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p1471155922712"><a name="p1471155922712"></a><a name="p1471155922712"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p1871155912279"><a name="p1871155912279"></a><a name="p1871155912279"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p471115972720"><a name="p471115972720"></a><a name="p471115972720"></a>CIDR格式</p>
<p id="p171105952717"><a name="p171105952717"></a><a name="p171105952717"></a>【使用说明】只支持10.0.0.0/8,172.16.0.0/12,192.168.0.0/16三个网段内的地址，掩码长度不能大于28。</p>
</td>
</tr>
<tr id="row373659122718"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p173195914274"><a name="p173195914274"></a><a name="p173195914274"></a>gateway_ip</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p16733594272"><a name="p16733594272"></a><a name="p16733594272"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p167319597276"><a name="p167319597276"></a><a name="p167319597276"></a>网关IP不允许和allocation_pools地址块冲突。</p>
<p id="p1773175918271"><a name="p1773175918271"></a><a name="p1773175918271"></a>【使用说明】不支持修改。</p>
</td>
</tr>
<tr id="row6733598278"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p37325918273"><a name="p37325918273"></a><a name="p37325918273"></a>allocation_pools</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p974125918276"><a name="p974125918276"></a><a name="p974125918276"></a>Array of <a href="#table1777145918276">allocation_pool</a> objects</p>
<p id="p107495982715"><a name="p107495982715"></a><a name="p107495982715"></a></p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p13740597271"><a name="p13740597271"></a><a name="p13740597271"></a>可用的IP池，allocation_pool对象参见</p>
<p id="p8891441195814"><a name="p8891441195814"></a><a name="p8891441195814"></a><a href="#table1777145918276">表7</a></p>
<p id="p137415915279"><a name="p137415915279"></a><a name="p137415915279"></a>例如：[ { "start": "10.0.0.2", "end": "10.0.0.251"} ]</p>
<p id="p167414592279"><a name="p167414592279"></a><a name="p167414592279"></a>每个子网的第1个和最后3个IP地址为系统保留地址。以192.168.1.0/24为例，192.168.1.0、 192.168.1.253、192.168.1.254和192.168.1.255这些地址是系统保留地址。系统预留地址默认不在allocation_pool范围内。</p>
<p id="p074359192720"><a name="p074359192720"></a><a name="p074359192720"></a>约束：更新时allocation_pool范围不能包含网关和广播地址的所有IP。</p>
</td>
</tr>
<tr id="row474205911270"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p774105972720"><a name="p774105972720"></a><a name="p774105972720"></a>dns_nameservers</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p1474155952710"><a name="p1474155952710"></a><a name="p1474155952710"></a>Array&nbsp;of&nbsp;strings</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p10743593273"><a name="p10743593273"></a><a name="p10743593273"></a>dns服务器</p>
<p id="p97485912712"><a name="p97485912712"></a><a name="p97485912712"></a>例如："dns_nameservers": ["8.xx.xx.8","8.xx.xx.4"]</p>
</td>
</tr>
<tr id="row6741659182714"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p574959122713"><a name="p574959122713"></a><a name="p574959122713"></a>host_routes</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p3169174310293"><a name="p3169174310293"></a><a name="p3169174310293"></a>Array of <a href="#table177865912715">host_route</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p2074459132712"><a name="p2074459132712"></a><a name="p2074459132712"></a>虚拟机静态路由，参见<a href="#table177865912715">表8</a></p>
<p id="p1674359172717"><a name="p1674359172717"></a><a name="p1674359172717"></a>【使用说明】不支持，忽略输入信息</p>
</td>
</tr>
<tr id="row42017779105653"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p5182838910577"><a name="p5182838910577"></a><a name="p5182838910577"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p3734998010577"><a name="p3734998010577"></a><a name="p3734998010577"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row97535914274"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p475959202718"><a name="p475959202718"></a><a name="p475959202718"></a>enable_dhcp</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p2755596279"><a name="p2755596279"></a><a name="p2755596279"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p47595962710"><a name="p47595962710"></a><a name="p47595962710"></a>是否启动dhcp，false表示不提供dhcp服务的能力</p>
<p id="p57535914276"><a name="p57535914276"></a><a name="p57535914276"></a>【使用说明】只支持true</p>
</td>
</tr>
<tr id="row63315321123"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p45641422124917"><a name="p45641422124917"></a><a name="p45641422124917"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p16855104462516"><a name="p16855104462516"></a><a name="p16855104462516"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row126291040191211"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间，UTC时间</p>
<p id="p65980291419"><a name="p65980291419"></a><a name="p65980291419"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row1084513362123"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.2 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.33433343334334%" headers="mcps1.2.4.1.3 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间，UTC时间</p>
<p id="p173172815471"><a name="p173172815471"></a><a name="p173172815471"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

**表 7**  allocation\_pool对象

<a name="table1777145918276"></a>
<table><thead align="left"><tr id="row11772597275"><th class="cellrowborder" valign="top" width="23.65%" id="mcps1.2.4.1.1"><p id="p1477155962713"><a name="p1477155962713"></a><a name="p1477155962713"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="24.610000000000003%" id="mcps1.2.4.1.2"><p id="p1077859162717"><a name="p1077859162717"></a><a name="p1077859162717"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.739999999999995%" id="mcps1.2.4.1.3"><p id="p5771159182718"><a name="p5771159182718"></a><a name="p5771159182718"></a>备注</p>
</th>
</tr>
</thead>
<tbody><tr id="row167785982711"><td class="cellrowborder" valign="top" width="23.65%" headers="mcps1.2.4.1.1 "><p id="p1077159182720"><a name="p1077159182720"></a><a name="p1077159182720"></a>start</p>
</td>
<td class="cellrowborder" valign="top" width="24.610000000000003%" headers="mcps1.2.4.1.2 "><p id="p2077125912718"><a name="p2077125912718"></a><a name="p2077125912718"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.739999999999995%" headers="mcps1.2.4.1.3 "><p id="p2078205910275"><a name="p2078205910275"></a><a name="p2078205910275"></a>网络池起始IP</p>
</td>
</tr>
<tr id="row1782594271"><td class="cellrowborder" valign="top" width="23.65%" headers="mcps1.2.4.1.1 "><p id="p9781459162717"><a name="p9781459162717"></a><a name="p9781459162717"></a>end</p>
</td>
<td class="cellrowborder" valign="top" width="24.610000000000003%" headers="mcps1.2.4.1.2 "><p id="p1778115952719"><a name="p1778115952719"></a><a name="p1778115952719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.739999999999995%" headers="mcps1.2.4.1.3 "><p id="p187825911271"><a name="p187825911271"></a><a name="p187825911271"></a>网络池结束IP</p>
</td>
</tr>
</tbody>
</table>

**表 8**  host\_route对象

<a name="table177865912715"></a>
<table><thead align="left"><tr id="row1779145992719"><th class="cellrowborder" valign="top" width="23.712371237123715%" id="mcps1.2.4.1.1"><p id="p2794593271"><a name="p2794593271"></a><a name="p2794593271"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="24.4024402440244%" id="mcps1.2.4.1.2"><p id="p14791594271"><a name="p14791594271"></a><a name="p14791594271"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.88518851885189%" id="mcps1.2.4.1.3"><p id="p14791459172716"><a name="p14791459172716"></a><a name="p14791459172716"></a>备注</p>
</th>
</tr>
</thead>
<tbody><tr id="row1379165919277"><td class="cellrowborder" valign="top" width="23.712371237123715%" headers="mcps1.2.4.1.1 "><p id="p979165972710"><a name="p979165972710"></a><a name="p979165972710"></a>destination</p>
</td>
<td class="cellrowborder" valign="top" width="24.4024402440244%" headers="mcps1.2.4.1.2 "><p id="p37995952710"><a name="p37995952710"></a><a name="p37995952710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.88518851885189%" headers="mcps1.2.4.1.3 "><p id="p10791559172714"><a name="p10791559172714"></a><a name="p10791559172714"></a>路由目的子网</p>
</td>
</tr>
<tr id="row1779185915279"><td class="cellrowborder" valign="top" width="23.712371237123715%" headers="mcps1.2.4.1.1 "><p id="p6791359102719"><a name="p6791359102719"></a><a name="p6791359102719"></a>nexthop</p>
</td>
<td class="cellrowborder" valign="top" width="24.4024402440244%" headers="mcps1.2.4.1.2 "><p id="p107935942717"><a name="p107935942717"></a><a name="p107935942717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.88518851885189%" headers="mcps1.2.4.1.3 "><p id="p87975920278"><a name="p87975920278"></a><a name="p87975920278"></a>路由下一跳IP</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section5055526711495"></a>

请求样例

```
PUT https://{Endpoint}/v2.0/subnets/98bac90c-0ba7-4a63-8995-097da9bead1c  

{
  "subnet": {
    "name": "subnet-test"
  }
}
```

响应样例

```
{
    "subnet": {
        "name": "subnet-test",
        "cidr": "172.16.2.0/24",
        "id": "98bac90c-0ba7-4a63-8995-097da9bead1c",
        "enable_dhcp": true,
        "network_id": "0133cd73-34d4-4d4c-bf1f-e65b24603206",
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "dns_nameservers": [],
        "allocation_pools": [
            {
                "start": "172.16.2.2",
                "end": "172.16.2.251"
            }
        ],
        "host_routes": [],
        "ip_version": 4,
        "gateway_ip": "172.16.2.1",
        "created_at": "2018-09-20T02:02:16",
        "updated_at": "2018-09-20T02:03:03"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

