# API概览<a name="zh-cn_topic_0173364207"></a>

虚拟私有云所提供的接口分为VPC接口与OpenStack原生接口。

通过配合使用VPC接口和OpenStack原生接口，您可以完整的使用虚拟私有云的所有功能。同一功能既有原生OpenStack接口，还有VPC接口时，建议您优先使用VPC接口。

对于企业项目用户，只能使用VPC接口，各接口对应的权限说明请参见[权限策略和授权项](权限策略和授权项.md)。

## VPC接口说明<a name="section14330125184315"></a>

**表 1**  VPC接口说明

<a name="table1336185894518"></a>
<table><thead align="left"><tr id="row3362058124511"><th class="cellrowborder" valign="top" width="20.810000000000002%" id="mcps1.2.3.1.1"><p id="p336219586450"><a name="p336219586450"></a><a name="p336219586450"></a><strong id="b10362175817458"><a name="b10362175817458"></a><a name="b10362175817458"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="79.19%" id="mcps1.2.3.1.2"><p id="p1636275810454"><a name="p1636275810454"></a><a name="p1636275810454"></a><strong id="b236225874512"><a name="b236225874512"></a><a name="b236225874512"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row14362205884514"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p2362858134510"><a name="p2362858134510"></a><a name="p2362858134510"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0000.html" target="_blank" rel="noopener noreferrer">VPC</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p17362125884520"><a name="p17362125884520"></a><a name="p17362125884520"></a>VPC的创建、查询、更新、删除等接口。</p>
</td>
</tr>
<tr id="row1936211585453"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p1836213587450"><a name="p1836213587450"></a><a name="p1836213587450"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0000.html" target="_blank" rel="noopener noreferrer">子网</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p2036295817452"><a name="p2036295817452"></a><a name="p2036295817452"></a>子网的创建、查询、更新、删除等接口。</p>
</td>
</tr>
<tr id="row103631858124512"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p153634581457"><a name="p153634581457"></a><a name="p153634581457"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_quota_0000.html" target="_blank" rel="noopener noreferrer">配额</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p9363145811453"><a name="p9363145811453"></a><a name="p9363145811453"></a>配额查询接口。</p>
</td>
</tr>
<tr id="row736325817457"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p736315894514"><a name="p736315894514"></a><a name="p736315894514"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0000.html" target="_blank" rel="noopener noreferrer">私有IP</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p936355816451"><a name="p936355816451"></a><a name="p936355816451"></a>私有IP的申请、查询、删除等接口。</p>
</td>
</tr>
<tr id="row53631958124513"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p1236305854511"><a name="p1236305854511"></a><a name="p1236305854511"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0000.html" target="_blank" rel="noopener noreferrer">安全组</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><a name="ul1136325812458"></a><a name="ul1136325812458"></a><ul id="ul1136325812458"><li>安全组创建、查询、删除等接口。</li><li>安全组规则创建、查询、删除等接口。</li></ul>
</td>
</tr>
<tr id="row1736416582452"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p236415582452"><a name="p236415582452"></a><a name="p236415582452"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0000.html" target="_blank" rel="noopener noreferrer">端口</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p836435874518"><a name="p836435874518"></a><a name="p836435874518"></a>端口创建、查询、更新、删除等接口。</p>
</td>
</tr>
<tr id="row143648588454"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p536412589453"><a name="p536412589453"></a><a name="p536412589453"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_peering_0000.html" target="_blank" rel="noopener noreferrer">对等连接</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><a name="ul1836415584453"></a><a name="ul1836415584453"></a><ul id="ul1836415584453"><li>对等连接查询、创建、更新、删除等接口。</li><li>接受、拒绝对等连接请求接口。</li></ul>
</td>
</tr>
<tr id="row13364195817451"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p143647589456"><a name="p143647589456"></a><a name="p143647589456"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_route_0000.html" target="_blank" rel="noopener noreferrer">VPC路由</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p136411583451"><a name="p136411583451"></a><a name="p136411583451"></a>VPC路由查询、创建、删除等接口。</p>
</td>
</tr>
<tr id="row836417588454"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p036414581456"><a name="p036414581456"></a><a name="p036414581456"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_tag_0000.html" target="_blank" rel="noopener noreferrer">标签管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><a name="ul136485854520"></a><a name="ul136485854520"></a><ul id="ul136485854520"><li>VPC资源标签的创建、查询、删除等接口。</li><li>子网资源标签的创建、查询、删除等接口。</li></ul>
<p id="p103659580457"><a name="p103659580457"></a><a name="p103659580457"></a>该类型接口目前在“华北-北京一”“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”“华南-广州”、“亚太-香港”区域开放。</p>
</td>
</tr>
<tr id="row636520586451"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p13654589453"><a name="p13654589453"></a><a name="p13654589453"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_natworkip_0000.html" target="_blank" rel="noopener noreferrer">查询网络IP使用情况</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p103651958184513"><a name="p103651958184513"></a><a name="p103651958184513"></a>查询一个指定网络中的IP地址使用情况，包括网络中的IP总数以及已用IP总数。</p>
</td>
</tr>
</tbody>
</table>

## OpenStack原生接口说明<a name="section3102202117447"></a>

**表 2**  OpenStack原生接口说明

<a name="table101761398465"></a>
<table><thead align="left"><tr id="row1617633924619"><th class="cellrowborder" valign="top" width="20.810000000000002%" id="mcps1.2.3.1.1"><p id="p2176153924610"><a name="p2176153924610"></a><a name="p2176153924610"></a><strong id="b2176183915460"><a name="b2176183915460"></a><a name="b2176183915460"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="79.19%" id="mcps1.2.3.1.2"><p id="p3176143954615"><a name="p3176143954615"></a><a name="p3176143954615"></a><strong id="b1917614397466"><a name="b1917614397466"></a><a name="b1917614397466"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row6185339124618"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p1918511393466"><a name="p1918511393466"></a><a name="p1918511393466"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_version_0000.html" target="_blank" rel="noopener noreferrer">API版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p1818519392464"><a name="p1818519392464"></a><a name="p1818519392464"></a>当前API所有可用版本的查询、分页查询。</p>
</td>
</tr>
<tr id="row2018603984619"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p42876425423"><a name="p42876425423"></a><a name="p42876425423"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0000.html" target="_blank" rel="noopener noreferrer">端口</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p618619393463"><a name="p618619393463"></a><a name="p618619393463"></a>端口的查询、创建、更新、删除等接口。</p>
</td>
</tr>
<tr id="row4186153914468"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p19186143919469"><a name="p19186143919469"></a><a name="p19186143919469"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0000.html" target="_blank" rel="noopener noreferrer">网络</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p1186143910460"><a name="p1186143910460"></a><a name="p1186143910460"></a>网络的查询、创建、更新、删除等接口。</p>
</td>
</tr>
<tr id="row81862039134620"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p111865394468"><a name="p111865394468"></a><a name="p111865394468"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0000.html" target="_blank" rel="noopener noreferrer">子网</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p161861139134613"><a name="p161861139134613"></a><a name="p161861139134613"></a>子网的查询、创建、更新、删除等接口。</p>
</td>
</tr>
<tr id="row15186193944619"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p141861639104615"><a name="p141861639104615"></a><a name="p141861639104615"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0000.html" target="_blank" rel="noopener noreferrer">路由器</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p16186163964611"><a name="p16186163964611"></a><a name="p16186163964611"></a>路由器的查询、创建、更新、删除等接口。</p>
</td>
</tr>
<tr id="row131871739124614"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p7187133911466"><a name="p7187133911466"></a><a name="p7187133911466"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_firewall_0000.html" target="_blank" rel="noopener noreferrer">网络ACL</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><a name="ul101871039184612"></a><a name="ul101871039184612"></a><ul id="ul101871039184612"><li><span id="text58621025101818"><a name="text58621025101818"></a><a name="text58621025101818"></a>网络ACL</span><span id="text19862142514185"><a name="text19862142514185"></a><a name="text19862142514185"></a></span>的创建、更新、删除等接口。</li><li><span id="text1986312701817"><a name="text1986312701817"></a><a name="text1986312701817"></a>网络ACL</span><span id="text10863122710185"><a name="text10863122710185"></a><a name="text10863122710185"></a></span>规则的创建、更新、删除、查询等接口。</li><li><span id="text07991229111811"><a name="text07991229111811"></a><a name="text07991229111811"></a>网络ACL</span><span id="text13799629141819"><a name="text13799629141819"></a><a name="text13799629141819"></a></span>策略的创建、更新、删除、查询等接口。</li></ul>
</td>
</tr>
<tr id="row3187439104619"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p01885397466"><a name="p01885397466"></a><a name="p01885397466"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0000.html" target="_blank" rel="noopener noreferrer">安全组</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><a name="ul19188239124618"></a><a name="ul19188239124618"></a><ul id="ul19188239124618"><li>安全组创建、查询、删除、更新等接口。</li><li>安全组规则创建、查询、删除等接口。</li></ul>
</td>
</tr>
</tbody>
</table>

