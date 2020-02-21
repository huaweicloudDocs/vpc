# API概览<a name="zh-cn_topic_0173364207"></a>

虚拟私有云所提供的接口分为VPC接口与OpenStack原生接口。

通过配合使用VPC接口和OpenStack原生接口，您可以完整的使用虚拟私有云的所有功能。同一功能既有原生OpenStack接口，还有VPC接口时，建议您优先使用VPC接口。

对于企业项目用户，只能使用VPC接口，各接口对应的权限说明请参见[权限策略和授权项](权限策略和授权项.md)。

**表 1**  接口说明

<a name="te9c2c27af3ef410ca49687211136fc68"></a>
<table><thead align="left"><tr id="r3268e8c4605e4c56b76fed80d3d7179b"><th class="cellrowborder" valign="top" width="19.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0121588224_p487811268290"><a name="zh-cn_topic_0121588224_p487811268290"></a><a name="zh-cn_topic_0121588224_p487811268290"></a><strong id="a897e0013dd5c4147b76411fb246b5cbf"><a name="a897e0013dd5c4147b76411fb246b5cbf"></a><a name="a897e0013dd5c4147b76411fb246b5cbf"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.82%" id="mcps1.2.4.1.2"><p id="a4d42a930985f4adfba2e1b3b2f7c1e5c"><a name="a4d42a930985f4adfba2e1b3b2f7c1e5c"></a><a name="a4d42a930985f4adfba2e1b3b2f7c1e5c"></a><strong id="a59202d4115294047bf1b1c771c0c15b7"><a name="a59202d4115294047bf1b1c771c0c15b7"></a><a name="a59202d4115294047bf1b1c771c0c15b7"></a>子类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="64%" id="mcps1.2.4.1.3"><p id="a7db882c6ed8e41649d1e0dd885f2cb24"><a name="a7db882c6ed8e41649d1e0dd885f2cb24"></a><a name="a7db882c6ed8e41649d1e0dd885f2cb24"></a><strong id="zh-cn_topic_0121588224_b15203449370"><a name="zh-cn_topic_0121588224_b15203449370"></a><a name="zh-cn_topic_0121588224_b15203449370"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="rd94c9e7d68744d848886418dcb53fbda"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="a4f6636d87d70493dbd6dac0bd57d6270"><a name="a4f6636d87d70493dbd6dac0bd57d6270"></a><a name="a4f6636d87d70493dbd6dac0bd57d6270"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p1711832215426"><a name="p1711832215426"></a><a name="p1711832215426"></a>VPC</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p73450100260"><a name="p73450100260"></a><a name="p73450100260"></a>VPC的创建、查询、更新、删除等接口。</p>
</td>
</tr>
<tr id="r2604299b19044ff6af7fd4523d60ff65"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p16731133115311"><a name="p16731133115311"></a><a name="p16731133115311"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p7116152254218"><a name="p7116152254218"></a><a name="p7116152254218"></a>子网</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p1345191072617"><a name="p1345191072617"></a><a name="p1345191072617"></a>子网的创建、查询、更新、删除等接口。</p>
</td>
</tr>
<tr id="r17ca8f0b934b457db191fe04fbf3af42"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p14725635135317"><a name="p14725635135317"></a><a name="p14725635135317"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p156231184496"><a name="p156231184496"></a><a name="p156231184496"></a>弹性公网IP</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p18104638134916"><a name="p18104638134916"></a><a name="p18104638134916"></a>弹性公网IP的申请、查询、更新、删除等接口。</p>
</td>
</tr>
<tr id="rdb0b6d1fb04c4ba891d163308b28fdde"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p12904162035316"><a name="p12904162035316"></a><a name="p12904162035316"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p11657401016"><a name="p11657401016"></a><a name="p11657401016"></a>带宽</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p96141701010"><a name="p96141701010"></a><a name="p96141701010"></a>带宽的查询、更新等接口。</p>
</td>
</tr>
<tr id="row13156184812615"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p12904162075319"><a name="p12904162075319"></a><a name="p12904162075319"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p1109722204210"><a name="p1109722204210"></a><a name="p1109722204210"></a>带宽（V2.0）</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><a name="ul74921813024"></a><a name="ul74921813024"></a><ul id="ul74921813024"><li>共享带宽的创建、删除等接口。</li><li>共享带宽插入/移出弹性公网IP操作。</li></ul>
</td>
</tr>
<tr id="row81561948102618"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p199041120105315"><a name="p199041120105315"></a><a name="p199041120105315"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p7106132215425"><a name="p7106132215425"></a><a name="p7106132215425"></a>配额</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p1481210321626"><a name="p1481210321626"></a><a name="p1481210321626"></a>配额查询接口。</p>
</td>
</tr>
<tr id="row4156748122612"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p190411208536"><a name="p190411208536"></a><a name="p190411208536"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p69917222421"><a name="p69917222421"></a><a name="p69917222421"></a>私有IP</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p14232421943"><a name="p14232421943"></a><a name="p14232421943"></a>私有IP的申请、查询、删除等接口。</p>
</td>
</tr>
<tr id="row1515624817263"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p1090482035314"><a name="p1090482035314"></a><a name="p1090482035314"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p14978229427"><a name="p14978229427"></a><a name="p14978229427"></a>安全组</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><a name="ul1566113391077"></a><a name="ul1566113391077"></a><ul id="ul1566113391077"><li>安全组创建、查询、删除等接口。</li><li>安全组规则创建、查询、删除等接口。</li></ul>
</td>
</tr>
<tr id="row15179102714516"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p317282010517"><a name="p317282010517"></a><a name="p317282010517"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p09317384610"><a name="p09317384610"></a><a name="p09317384610"></a>端口</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p23226335812"><a name="p23226335812"></a><a name="p23226335812"></a>端口创建、查询、更新、删除等接口。</p>
</td>
</tr>
<tr id="rf96c4401effa42a7b2d356f84070b98d"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p1994111517517"><a name="p1994111517517"></a><a name="p1994111517517"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p169013114616"><a name="p169013114616"></a><a name="p169013114616"></a>对等连接</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><a name="ul8905105114294"></a><a name="ul8905105114294"></a><ul id="ul8905105114294"><li>对等连接查询、创建、更新、删除等接口。</li><li>接受、拒绝对等连接请求接口。</li></ul>
</td>
</tr>
<tr id="r3b08984b52674cfc82aa586eaecac189"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p0941615259"><a name="p0941615259"></a><a name="p0941615259"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p109083164612"><a name="p109083164612"></a><a name="p109083164612"></a>VPC路由</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p732941010260"><a name="p732941010260"></a><a name="p732941010260"></a>VPC路由查询、创建、删除等接口。</p>
</td>
</tr>
<tr id="r80fc7a1aace64381b9567ab0906aed71"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p1941615657"><a name="p1941615657"></a><a name="p1941615657"></a>VPC接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p11888313467"><a name="p11888313467"></a><a name="p11888313467"></a>标签管理</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><a name="ul20558104818291"></a><a name="ul20558104818291"></a><ul id="ul20558104818291"><li>VPC资源标签的创建、查询、删除等接口。</li><li>子网资源标签的创建、查询、删除等接口。</li><li>弹性公网IP的创建、查询、删除等接口。</li></ul>
<p id="p10341154735217"><a name="p10341154735217"></a><a name="p10341154735217"></a>该类型接口目前仅在“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”区域开放。</p>
</td>
</tr>
<tr id="rccad5501787d4e4f81d9f8dbd1e47c20"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="a774fff5f4ccd40c4b3c74cc2ab894056"><a name="a774fff5f4ccd40c4b3c74cc2ab894056"></a><a name="a774fff5f4ccd40c4b3c74cc2ab894056"></a>OpenStack Neutron接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p386430466"><a name="p386430466"></a><a name="p386430466"></a>端口</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p15578141203420"><a name="p15578141203420"></a><a name="p15578141203420"></a>端口的查询、创建、更新、删除等接口。</p>
</td>
</tr>
<tr id="row24921665291"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p844712442361"><a name="p844712442361"></a><a name="p844712442361"></a>OpenStack Neutron接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p885163134617"><a name="p885163134617"></a><a name="p885163134617"></a>网络</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p10577512153412"><a name="p10577512153412"></a><a name="p10577512153412"></a>网络的查询、创建、更新、删除等接口。</p>
</td>
</tr>
<tr id="row8574134782719"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p74661155123820"><a name="p74661155123820"></a><a name="p74661155123820"></a>OpenStack Neutron接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p168453194610"><a name="p168453194610"></a><a name="p168453194610"></a>子网</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p15576151263411"><a name="p15576151263411"></a><a name="p15576151263411"></a>子网的查询、创建、更新、删除等接口。</p>
</td>
</tr>
<tr id="row185741475274"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p2971949173613"><a name="p2971949173613"></a><a name="p2971949173613"></a>OpenStack Neutron接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p6824312469"><a name="p6824312469"></a><a name="p6824312469"></a>路由器</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p205741012183413"><a name="p205741012183413"></a><a name="p205741012183413"></a>路由器的查询、创建、更新、删除等接口。</p>
</td>
</tr>
<tr id="row857418479278"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p207591550183610"><a name="p207591550183610"></a><a name="p207591550183610"></a>OpenStack Neutron接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p1480933469"><a name="p1480933469"></a><a name="p1480933469"></a>浮动IP</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><p id="p8573612133411"><a name="p8573612133411"></a><a name="p8573612133411"></a>浮动IP的查询、创建、更新、删除等接口。</p>
</td>
</tr>
<tr id="row4735122842911"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p1314417262396"><a name="p1314417262396"></a><a name="p1314417262396"></a>OpenStack Neutron接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p38013314461"><a name="p38013314461"></a><a name="p38013314461"></a>网络ACL</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><a name="ul161021536144811"></a><a name="ul161021536144811"></a><ul id="ul161021536144811"><li>网络ACL的创建、更新、删除等接口。</li><li>网络ACL规则的创建、更新、删除、查询等接口。</li><li>网络ACL策略的创建、更新、删除、查询等接口。</li></ul>
</td>
</tr>
<tr id="row5574124712717"><td class="cellrowborder" valign="top" width="19.18%" headers="mcps1.2.4.1.1 "><p id="p10579102918396"><a name="p10579102918396"></a><a name="p10579102918396"></a>OpenStack Neutron接口</p>
</td>
<td class="cellrowborder" valign="top" width="16.82%" headers="mcps1.2.4.1.2 "><p id="p1077193104617"><a name="p1077193104617"></a><a name="p1077193104617"></a>安全组</p>
</td>
<td class="cellrowborder" valign="top" width="64%" headers="mcps1.2.4.1.3 "><a name="ul1064148164919"></a><a name="ul1064148164919"></a><ul id="ul1064148164919"><li>安全组创建、查询、删除、更新等接口。</li><li>安全组规则创建、查询、删除等接口。</li></ul>
</td>
</tr>
</tbody>
</table>

