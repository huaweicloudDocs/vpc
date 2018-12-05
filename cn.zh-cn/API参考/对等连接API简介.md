# 对等连接API简介<a name="ZH-CN_TOPIC_0075677482"></a>

## 对象简介<a name="section1225418341442"></a>

管理和操作对等连接（vpc peering）资源，包括查询对等连接列表、创建对等连接、查询对等连接、删除对等连接以及更新对等连接等接口。

## 对象模型<a name="section11260153417417"></a>

**表 1**  peering对象

<a name="table1026243410414"></a>
<table><thead align="left"><tr id="row145386341548"><th class="cellrowborder" valign="top" width="21.65%" id="mcps1.2.7.1.1"><p id="p553843415417"><a name="p553843415417"></a><a name="p553843415417"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.7.1.2"><p id="p453814344418"><a name="p453814344418"></a><a name="p453814344418"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.28%" id="mcps1.2.7.1.3"><p id="p125382034242"><a name="p125382034242"></a><a name="p125382034242"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="11.34%" id="mcps1.2.7.1.4"><p id="p205391034141"><a name="p205391034141"></a><a name="p205391034141"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="13.4%" id="mcps1.2.7.1.5"><p id="p18539193413415"><a name="p18539193413415"></a><a name="p18539193413415"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="28.87%" id="mcps1.2.7.1.6"><p id="p13539183410412"><a name="p13539183410412"></a><a name="p13539183410412"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row195391034944"><td class="cellrowborder" valign="top" width="21.65%" headers="mcps1.2.7.1.1 "><p id="p1053943410414"><a name="p1053943410414"></a><a name="p1053943410414"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.7.1.2 "><p id="p753963414417"><a name="p753963414417"></a><a name="p753963414417"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.28%" headers="mcps1.2.7.1.3 "><p id="p105391834249"><a name="p105391834249"></a><a name="p105391834249"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.4 "><p id="p6539113418414"><a name="p6539113418414"></a><a name="p6539113418414"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.2.7.1.5 "><p id="p135391134342"><a name="p135391134342"></a><a name="p135391134342"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.87%" headers="mcps1.2.7.1.6 "><p id="p17539123411413"><a name="p17539123411413"></a><a name="p17539123411413"></a>对等连接id</p>
</td>
</tr>
<tr id="row185391134449"><td class="cellrowborder" valign="top" width="21.65%" headers="mcps1.2.7.1.1 "><p id="p15540123413417"><a name="p15540123413417"></a><a name="p15540123413417"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.7.1.2 "><p id="p85405341547"><a name="p85405341547"></a><a name="p85405341547"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.28%" headers="mcps1.2.7.1.3 "><p id="p35405341344"><a name="p35405341344"></a><a name="p35405341344"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.4 "><p id="p85401834040"><a name="p85401834040"></a><a name="p85401834040"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.2.7.1.5 "><p id="p354063411417"><a name="p354063411417"></a><a name="p354063411417"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.87%" headers="mcps1.2.7.1.6 "><p id="p1654017341747"><a name="p1654017341747"></a><a name="p1654017341747"></a>对等连接的名称，支持长度为1-64</p>
</td>
</tr>
<tr id="row45401734847"><td class="cellrowborder" valign="top" width="21.65%" headers="mcps1.2.7.1.1 "><p id="p354083416417"><a name="p354083416417"></a><a name="p354083416417"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.7.1.2 "><p id="p11540034946"><a name="p11540034946"></a><a name="p11540034946"></a>String(16)</p>
</td>
<td class="cellrowborder" valign="top" width="9.28%" headers="mcps1.2.7.1.3 "><p id="p1654117343415"><a name="p1654117343415"></a><a name="p1654117343415"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.4 "><p id="p954116340410"><a name="p954116340410"></a><a name="p954116340410"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.2.7.1.5 "><p id="p15541434345"><a name="p15541434345"></a><a name="p15541434345"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.87%" headers="mcps1.2.7.1.6 "><p id="p5541534142"><a name="p5541534142"></a><a name="p5541534142"></a>状态位，可以为PENDING_ACCEPTANCE、REJECTED、EXPIRED、DELETED、ACTIVE</p>
</td>
</tr>
<tr id="row155415343411"><td class="cellrowborder" valign="top" width="21.65%" headers="mcps1.2.7.1.1 "><p id="p185411334349"><a name="p185411334349"></a><a name="p185411334349"></a>request_vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.7.1.2 "><p id="p1854183414414"><a name="p1854183414414"></a><a name="p1854183414414"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="9.28%" headers="mcps1.2.7.1.3 "><p id="p115413341340"><a name="p115413341340"></a><a name="p115413341340"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.4 "><p id="p18541193415415"><a name="p18541193415415"></a><a name="p18541193415415"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.2.7.1.5 "><p id="p16541834349"><a name="p16541834349"></a><a name="p16541834349"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.87%" headers="mcps1.2.7.1.6 "><p id="p155422348412"><a name="p155422348412"></a><a name="p155422348412"></a>对等连接发起端vpc信息，参见<a href="#ZH-CN_TOPIC_0075677482__table1132310347417">表2</a></p>
</td>
</tr>
<tr id="row145425341249"><td class="cellrowborder" valign="top" width="21.65%" headers="mcps1.2.7.1.1 "><p id="p25421834641"><a name="p25421834641"></a><a name="p25421834641"></a>accept_vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.7.1.2 "><p id="p354211341141"><a name="p354211341141"></a><a name="p354211341141"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="9.28%" headers="mcps1.2.7.1.3 "><p id="p8542153415419"><a name="p8542153415419"></a><a name="p8542153415419"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.4 "><p id="p1354217347416"><a name="p1354217347416"></a><a name="p1354217347416"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.2.7.1.5 "><p id="p7542434242"><a name="p7542434242"></a><a name="p7542434242"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.87%" headers="mcps1.2.7.1.6 "><p id="p3542143419414"><a name="p3542143419414"></a><a name="p3542143419414"></a>对等连接接受端vpc信息，参见<a href="#ZH-CN_TOPIC_0075677482__table1132310347417">表2</a></p>
</td>
</tr>
</tbody>
</table>

**表 2**  vpc\_info对象

<a name="table1132310347417"></a>
<table><thead align="left"><tr id="row65431034046"><th class="cellrowborder" valign="top" width="21.65%" id="mcps1.2.7.1.1"><p id="p14543173418413"><a name="p14543173418413"></a><a name="p14543173418413"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="15.459999999999999%" id="mcps1.2.7.1.2"><p id="p1354353413410"><a name="p1354353413410"></a><a name="p1354353413410"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.28%" id="mcps1.2.7.1.3"><p id="p1754312341043"><a name="p1754312341043"></a><a name="p1754312341043"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="11.34%" id="mcps1.2.7.1.4"><p id="p185431634947"><a name="p185431634947"></a><a name="p185431634947"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="13.4%" id="mcps1.2.7.1.5"><p id="p354343412418"><a name="p354343412418"></a><a name="p354343412418"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="28.87%" id="mcps1.2.7.1.6"><p id="p19543634641"><a name="p19543634641"></a><a name="p19543634641"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4543434247"><td class="cellrowborder" valign="top" width="21.65%" headers="mcps1.2.7.1.1 "><p id="p13544163416415"><a name="p13544163416415"></a><a name="p13544163416415"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.7.1.2 "><p id="p654410341549"><a name="p654410341549"></a><a name="p654410341549"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.28%" headers="mcps1.2.7.1.3 "><p id="p5544113416410"><a name="p5544113416410"></a><a name="p5544113416410"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.4 "><p id="p45449344412"><a name="p45449344412"></a><a name="p45449344412"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.2.7.1.5 "><p id="p1454411341145"><a name="p1454411341145"></a><a name="p1454411341145"></a>存在的vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.87%" headers="mcps1.2.7.1.6 "><p id="p55448348416"><a name="p55448348416"></a><a name="p55448348416"></a>对等连接其中一端vpc id</p>
</td>
</tr>
<tr id="row65441334646"><td class="cellrowborder" valign="top" width="21.65%" headers="mcps1.2.7.1.1 "><p id="p14544034945"><a name="p14544034945"></a><a name="p14544034945"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.459999999999999%" headers="mcps1.2.7.1.2 "><p id="p454413347419"><a name="p454413347419"></a><a name="p454413347419"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.28%" headers="mcps1.2.7.1.3 "><p id="p1254415342411"><a name="p1254415342411"></a><a name="p1254415342411"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.4 "><p id="p175441342413"><a name="p175441342413"></a><a name="p175441342413"></a>vpc对应的tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.4%" headers="mcps1.2.7.1.5 "><p id="p175442341549"><a name="p175442341549"></a><a name="p175442341549"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.87%" headers="mcps1.2.7.1.6 "><p id="p105449344410"><a name="p105449344410"></a><a name="p105449344410"></a>对等连接其中一端vpc所属的项目id</p>
</td>
</tr>
</tbody>
</table>

