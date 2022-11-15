# 管理IPv6<a name="eip_0001"></a>

## 简介<a name="section427419411848"></a>

弹性公网IP支持IPv4地址和IPv6地址，您可以申请一个全新的IPv6弹性公网IP，也可以通过IPv6转换功能将已有的IPv4弹性公网IP映射为公网IPv6地址。

开启IPv6转换后，将提供IPv4和IPv6弹性公网IP地址，原有IPv4业务可以快速为IPv6用户提供访问能力。

IPv4弹性公网IP收取费用，IPv6弹性公网IP当前暂不收费，后续将择时收费。

## IPv4/IPv6双栈网络应用场景<a name="section1227519146612"></a>

如果您的ECS规格支持IPv6网络，那么您可以使用IPv4/IPv6双栈网络，场景示例和资源规划如[表1](#zh-cn_topic_0000001374350697_table105590377292)所示。

**表 1**  IPv4/IPv6双栈网络的应用场景及资源规划

<a name="zh-cn_topic_0000001374350697_table105590377292"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001374350697_vpc_0002_row1455915377291"><th class="cellrowborder" valign="top" width="10.489999999999998%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0000001374350697_vpc_0002_p155591237112916"><a name="zh-cn_topic_0000001374350697_vpc_0002_p155591237112916"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p155591237112916"></a>应用场景</p>
</th>
<th class="cellrowborder" valign="top" width="17.59%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0000001374350697_vpc_0002_p255918376297"><a name="zh-cn_topic_0000001374350697_vpc_0002_p255918376297"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p255918376297"></a>场景示例</p>
</th>
<th class="cellrowborder" valign="top" width="40.38%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0000001374350697_p72488217461"><a name="zh-cn_topic_0000001374350697_p72488217461"></a><a name="zh-cn_topic_0000001374350697_p72488217461"></a>条件</p>
</th>
<th class="cellrowborder" valign="top" width="10.71%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0000001374350697_vpc_0002_p14559237132910"><a name="zh-cn_topic_0000001374350697_vpc_0002_p14559237132910"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p14559237132910"></a>子网网段类型</p>
</th>
<th class="cellrowborder" valign="top" width="20.830000000000002%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0000001374350697_vpc_0002_p105590375296"><a name="zh-cn_topic_0000001374350697_vpc_0002_p105590375296"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p105590375296"></a>ECS</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001374350697_row1623913713308"><td class="cellrowborder" valign="top" width="10.489999999999998%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0000001374350697_p2531102113011"><a name="zh-cn_topic_0000001374350697_p2531102113011"></a><a name="zh-cn_topic_0000001374350697_p2531102113011"></a>IPv4内网通信</p>
</td>
<td class="cellrowborder" valign="top" width="17.59%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0000001374350697_p823910763016"><a name="zh-cn_topic_0000001374350697_p823910763016"></a><a name="zh-cn_topic_0000001374350697_p823910763016"></a>在ECS上部署应用，需要与其他系统（比如数据库）之间使用<strong id="zh-cn_topic_0000001374350697_b3598102811426"><a name="zh-cn_topic_0000001374350697_b3598102811426"></a><a name="zh-cn_topic_0000001374350697_b3598102811426"></a>IPV4</strong>进行内网互访。</p>
</td>
<td class="cellrowborder" valign="top" width="40.38%" headers="mcps1.2.6.1.3 "><a name="zh-cn_topic_0000001374350697_ul2222123744117"></a><a name="zh-cn_topic_0000001374350697_ul2222123744117"></a><ul id="zh-cn_topic_0000001374350697_ul2222123744117"><li>VPC的子网未开启IPv6。</li><li>实例未绑定<span id="zh-cn_topic_0000001374350697_text371061683314"><a name="zh-cn_topic_0000001374350697_text371061683314"></a><a name="zh-cn_topic_0000001374350697_text371061683314"></a></span><span id="zh-cn_topic_0000001374350697_text0188181915330"><a name="zh-cn_topic_0000001374350697_text0188181915330"></a><a name="zh-cn_topic_0000001374350697_text0188181915330"></a>弹性公网IP</span>。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="10.71%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0000001374350697_p42391178307"><a name="zh-cn_topic_0000001374350697_p42391178307"></a><a name="zh-cn_topic_0000001374350697_p42391178307"></a>IPv4网段</p>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0000001374350697_p72391278305"><a name="zh-cn_topic_0000001374350697_p72391278305"></a><a name="zh-cn_topic_0000001374350697_p72391278305"></a><strong id="zh-cn_topic_0000001374350697_b157256983916"><a name="zh-cn_topic_0000001374350697_b157256983916"></a><a name="zh-cn_topic_0000001374350697_b157256983916"></a>IPv4私网地址：</strong>支持IPv4内网通信。</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001374350697_row335801012302"><td class="cellrowborder" valign="top" width="10.489999999999998%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0000001374350697_p1053217216303"><a name="zh-cn_topic_0000001374350697_p1053217216303"></a><a name="zh-cn_topic_0000001374350697_p1053217216303"></a>IPv4公网通信</p>
</td>
<td class="cellrowborder" valign="top" width="17.59%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0000001374350697_p10359910103013"><a name="zh-cn_topic_0000001374350697_p10359910103013"></a><a name="zh-cn_topic_0000001374350697_p10359910103013"></a>在ECS上部署应用，需要与其他系统（比如数据库）之间使用<strong id="zh-cn_topic_0000001374350697_b68551133174214"><a name="zh-cn_topic_0000001374350697_b68551133174214"></a><a name="zh-cn_topic_0000001374350697_b68551133174214"></a>IPV4</strong>进行公网互访。</p>
</td>
<td class="cellrowborder" valign="top" width="40.38%" headers="mcps1.2.6.1.3 "><a name="zh-cn_topic_0000001374350697_ul1917195612413"></a><a name="zh-cn_topic_0000001374350697_ul1917195612413"></a><ul id="zh-cn_topic_0000001374350697_ul1917195612413"><li>VPC的子网未开启IPv6。</li><li>实例绑定<span id="zh-cn_topic_0000001374350697_text0181856104113"><a name="zh-cn_topic_0000001374350697_text0181856104113"></a><a name="zh-cn_topic_0000001374350697_text0181856104113"></a></span><span id="zh-cn_topic_0000001374350697_text19181956164110"><a name="zh-cn_topic_0000001374350697_text19181956164110"></a><a name="zh-cn_topic_0000001374350697_text19181956164110"></a>弹性公网IP</span>。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="10.71%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0000001374350697_p18569197113411"><a name="zh-cn_topic_0000001374350697_p18569197113411"></a><a name="zh-cn_topic_0000001374350697_p18569197113411"></a>IPv4网段</p>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.6.1.5 "><a name="zh-cn_topic_0000001374350697_ul121841172514"></a><a name="zh-cn_topic_0000001374350697_ul121841172514"></a><ul id="zh-cn_topic_0000001374350697_ul121841172514"><li><strong id="zh-cn_topic_0000001374350697_b1299612141059"><a name="zh-cn_topic_0000001374350697_b1299612141059"></a><a name="zh-cn_topic_0000001374350697_b1299612141059"></a>IPv4私网地址：</strong>支持IPv4内网通信。</li><li><strong id="zh-cn_topic_0000001374350697_b13705131314398"><a name="zh-cn_topic_0000001374350697_b13705131314398"></a><a name="zh-cn_topic_0000001374350697_b13705131314398"></a>IPv4公网地址：</strong>支持IPv4公网通信。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0000001374350697_row19576052134216"><td class="cellrowborder" valign="top" width="10.489999999999998%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0000001374350697_p1957719529426"><a name="zh-cn_topic_0000001374350697_p1957719529426"></a><a name="zh-cn_topic_0000001374350697_p1957719529426"></a>IPv6内网通信</p>
</td>
<td class="cellrowborder" valign="top" width="17.59%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0000001374350697_p1657717526427"><a name="zh-cn_topic_0000001374350697_p1657717526427"></a><a name="zh-cn_topic_0000001374350697_p1657717526427"></a>在ECS上部署应用，需要与其他系统（比如数据库）之间使用<strong id="zh-cn_topic_0000001374350697_b9866154016423"><a name="zh-cn_topic_0000001374350697_b9866154016423"></a><a name="zh-cn_topic_0000001374350697_b9866154016423"></a>IPV6</strong>进行内网互访。</p>
</td>
<td class="cellrowborder" valign="top" width="40.38%" headers="mcps1.2.6.1.3 "><a name="zh-cn_topic_0000001374350697_ul588432014475"></a><a name="zh-cn_topic_0000001374350697_ul588432014475"></a><ul id="zh-cn_topic_0000001374350697_ul588432014475"><li>VPC的子网开启IPv6。</li><li>创建ECS时，网络配置如下：<a name="zh-cn_topic_0000001374350697_ul1757174118501"></a><a name="zh-cn_topic_0000001374350697_ul1757174118501"></a><ul id="zh-cn_topic_0000001374350697_ul1757174118501"><li><strong id="zh-cn_topic_0000001374350697_b1989219481537"><a name="zh-cn_topic_0000001374350697_b1989219481537"></a><a name="zh-cn_topic_0000001374350697_b1989219481537"></a>规格：</strong>选择支持IPv6网络的ECS规格。关于ECS哪些规格支持IPv6网络，请参见<a href="https://support.huaweicloud.com/productdesc-ecs/ecs_01_0019.html" target="_blank" rel="noopener noreferrer">《弹性云服务器用户指南》</a></li><li><strong id="zh-cn_topic_0000001374350697_b19667201414818"><a name="zh-cn_topic_0000001374350697_b19667201414818"></a><a name="zh-cn_topic_0000001374350697_b19667201414818"></a>VPC和子网：</strong>选择已开启IPv6的子网及子网所属的VPC。</li><li>选择“<strong id="zh-cn_topic_0000001374350697_b291301913813"><a name="zh-cn_topic_0000001374350697_b291301913813"></a><a name="zh-cn_topic_0000001374350697_b291301913813"></a>自动分配IPv6地址</strong>”。</li><li><strong id="zh-cn_topic_0000001374350697_b21401728282"><a name="zh-cn_topic_0000001374350697_b21401728282"></a><a name="zh-cn_topic_0000001374350697_b21401728282"></a>共享带宽：</strong>暂不配置。</li></ul>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="10.71%" headers="mcps1.2.6.1.4 "><a name="zh-cn_topic_0000001374350697_ul1075885351019"></a><a name="zh-cn_topic_0000001374350697_ul1075885351019"></a><ul id="zh-cn_topic_0000001374350697_ul1075885351019"><li>IPv4网段</li><li>IPv6网段</li></ul>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.6.1.5 "><a name="zh-cn_topic_0000001374350697_ul3341172910111"></a><a name="zh-cn_topic_0000001374350697_ul3341172910111"></a><ul id="zh-cn_topic_0000001374350697_ul3341172910111"><li><strong id="zh-cn_topic_0000001374350697_b139801430133718"><a name="zh-cn_topic_0000001374350697_b139801430133718"></a><a name="zh-cn_topic_0000001374350697_b139801430133718"></a>IPv4私网地址+IPv4 EIP：</strong>实例绑定IPv4 EIP，支持IPv4公网通信。</li><li><strong id="zh-cn_topic_0000001374350697_b23555252111"><a name="zh-cn_topic_0000001374350697_b23555252111"></a><a name="zh-cn_topic_0000001374350697_b23555252111"></a>IPv4私网地址：</strong>实例不绑定IPv4 EIP，支持IPv4内网通信。</li><li><strong id="zh-cn_topic_0000001374350697_b9812814195"><a name="zh-cn_topic_0000001374350697_b9812814195"></a><a name="zh-cn_topic_0000001374350697_b9812814195"></a>IPv6地址：</strong>IPv6地址不加入共享带宽，支持IPv6内网通信。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0000001374350697_vpc_0002_row14559183702918"><td class="cellrowborder" valign="top" width="10.489999999999998%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0000001374350697_vpc_0002_p1559103711297"><a name="zh-cn_topic_0000001374350697_vpc_0002_p1559103711297"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p1559103711297"></a>IPv6公网通信</p>
</td>
<td class="cellrowborder" valign="top" width="17.59%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0000001374350697_p16133835171413"><a name="zh-cn_topic_0000001374350697_p16133835171413"></a><a name="zh-cn_topic_0000001374350697_p16133835171413"></a>搭建IPv6网络，使ECS可以访问Internet上的<strong id="zh-cn_topic_0000001374350697_b4341449144214"><a name="zh-cn_topic_0000001374350697_b4341449144214"></a><a name="zh-cn_topic_0000001374350697_b4341449144214"></a>IPv6</strong>服务。</p>
</td>
<td class="cellrowborder" valign="top" width="40.38%" headers="mcps1.2.6.1.3 "><a name="zh-cn_topic_0000001374350697_ul139761521161417"></a><a name="zh-cn_topic_0000001374350697_ul139761521161417"></a><ul id="zh-cn_topic_0000001374350697_ul139761521161417"><li>VPC的子网开启IPv6。</li><li>创建ECS时，网络配置如下：<a name="zh-cn_topic_0000001374350697_ul1942019095714"></a><a name="zh-cn_topic_0000001374350697_ul1942019095714"></a><ul id="zh-cn_topic_0000001374350697_ul1942019095714"><li><strong id="zh-cn_topic_0000001374350697_b197762131413"><a name="zh-cn_topic_0000001374350697_b197762131413"></a><a name="zh-cn_topic_0000001374350697_b197762131413"></a>规格：</strong>选择支持IPv6网络的ECS规格。关于ECS哪些规格支持IPv6网络，请参见<a href="https://support.huaweicloud.com/productdesc-ecs/ecs_01_0019.html" target="_blank" rel="noopener noreferrer">《弹性云服务器用户指南》</a></li><li><strong id="zh-cn_topic_0000001374350697_b19771921161410"><a name="zh-cn_topic_0000001374350697_b19771921161410"></a><a name="zh-cn_topic_0000001374350697_b19771921161410"></a>VPC和子网：</strong>选择已开启IPv6的子网及子网所属的VPC。</li><li>选择“<strong id="zh-cn_topic_0000001374350697_b1197722161420"><a name="zh-cn_topic_0000001374350697_b1197722161420"></a><a name="zh-cn_topic_0000001374350697_b1197722161420"></a>自动分配IPv6地址</strong>”。</li><li><strong id="zh-cn_topic_0000001374350697_b1797752121414"><a name="zh-cn_topic_0000001374350697_b1797752121414"></a><a name="zh-cn_topic_0000001374350697_b1797752121414"></a>共享带宽：</strong>选择一个共享带宽。</li></ul>
</li></ul>
<div class="note" id="zh-cn_topic_0000001374350697_note18818202845720"><a name="zh-cn_topic_0000001374350697_note18818202845720"></a><a name="zh-cn_topic_0000001374350697_note18818202845720"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0000001374350697_p13818728135720"><a name="zh-cn_topic_0000001374350697_p13818728135720"></a><a name="zh-cn_topic_0000001374350697_p13818728135720"></a>该场景的具体实现请参见<a href="https://support.huaweicloud.com/qs-vpc/qs_ipv6.html" target="_blank" rel="noopener noreferrer">搭建IPv6网络</a>。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="10.71%" headers="mcps1.2.6.1.4 "><a name="zh-cn_topic_0000001374350697_ul1358217161183"></a><a name="zh-cn_topic_0000001374350697_ul1358217161183"></a><ul id="zh-cn_topic_0000001374350697_ul1358217161183"><li>IPv4网段</li><li>IPv6网段</li></ul>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.6.1.5 "><a name="zh-cn_topic_0000001374350697_ul2841104394015"></a><a name="zh-cn_topic_0000001374350697_ul2841104394015"></a><ul id="zh-cn_topic_0000001374350697_ul2841104394015"><li><strong id="zh-cn_topic_0000001374350697_b084194317408"><a name="zh-cn_topic_0000001374350697_b084194317408"></a><a name="zh-cn_topic_0000001374350697_b084194317408"></a>IPv4私网地址+IPv4 EIP：</strong>实例绑定IPv4 EIP，支持IPv4公网通信。</li><li><strong id="zh-cn_topic_0000001374350697_b18411431404"><a name="zh-cn_topic_0000001374350697_b18411431404"></a><a name="zh-cn_topic_0000001374350697_b18411431404"></a>IPv4私网地址：</strong>实例不绑定IPv4 EIP，支持IPv4内网通信。</li></ul>
<a name="zh-cn_topic_0000001374350697_ul1522674132211"></a><a name="zh-cn_topic_0000001374350697_ul1522674132211"></a><ul id="zh-cn_topic_0000001374350697_ul1522674132211"><li><strong id="zh-cn_topic_0000001374350697_b9226341162217"><a name="zh-cn_topic_0000001374350697_b9226341162217"></a><a name="zh-cn_topic_0000001374350697_b9226341162217"></a>IPv6地址+共享带宽：</strong>同时支持IPv6公网通信和IPv6内网通信。</li></ul>
</td>
</tr>
</tbody>
</table>

使用IPv4/IPv6双栈网络请参考[IPv4/IPv6双栈网络](https://support.huaweicloud.com/usermanual-vpc/vpc_0002.html)。

## **IPv6转换**功能应用场景<a name="section172321632117"></a>

如果您想使部署应用的ECS面向Internet客户端提供IPv6服务，但您的ECS规格不支持IPv6网络，或者您不想通过搭建IPv6网络来实现该需求，那么您可以通过弹性公网IP的IPv6转换功能快速实现该能力。场景示例和资源规划如[表2](#zh-cn_topic_0000001374350697_table104846201827)。

**表 2**  IPv6 EIP（开启IPv6转换）网络的应用场景及资源规划

<a name="zh-cn_topic_0000001374350697_table104846201827"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001374350697_vpc_0002_row10563044205914"><th class="cellrowborder" valign="top" width="11.28%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0000001374350697_vpc_0002_p1756315441597"><a name="zh-cn_topic_0000001374350697_vpc_0002_p1756315441597"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p1756315441597"></a>应用场景</p>
</th>
<th class="cellrowborder" valign="top" width="22.63%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0000001374350697_vpc_0002_p1456364475911"><a name="zh-cn_topic_0000001374350697_vpc_0002_p1456364475911"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p1456364475911"></a>场景示例</p>
</th>
<th class="cellrowborder" valign="top" width="20.54%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0000001374350697_p239913024617"><a name="zh-cn_topic_0000001374350697_p239913024617"></a><a name="zh-cn_topic_0000001374350697_p239913024617"></a>条件</p>
</th>
<th class="cellrowborder" valign="top" width="13.389999999999999%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0000001374350697_vpc_0002_p856374416599"><a name="zh-cn_topic_0000001374350697_vpc_0002_p856374416599"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p856374416599"></a>子网网段类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.16%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0000001374350697_vpc_0002_p71425413219"><a name="zh-cn_topic_0000001374350697_vpc_0002_p71425413219"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p71425413219"></a>ECS</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001374350697_vpc_0002_row1956304410594"><td class="cellrowborder" valign="top" width="11.28%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0000001374350697_vpc_0002_p55632448596"><a name="zh-cn_topic_0000001374350697_vpc_0002_p55632448596"></a><a name="zh-cn_topic_0000001374350697_vpc_0002_p55632448596"></a>IPv6公网通信</p>
</td>
<td class="cellrowborder" valign="top" width="22.63%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0000001374350697_p14719514615"><a name="zh-cn_topic_0000001374350697_p14719514615"></a><a name="zh-cn_topic_0000001374350697_p14719514615"></a>不搭建IPv6网络，使ECS为Internet上的客户端提供IPv6服务。</p>
</td>
<td class="cellrowborder" valign="top" width="20.54%" headers="mcps1.2.6.1.3 "><a name="zh-cn_topic_0000001374350697_ul184717564611"></a><a name="zh-cn_topic_0000001374350697_ul184717564611"></a><ul id="zh-cn_topic_0000001374350697_ul184717564611"><li>实例绑定<span id="zh-cn_topic_0000001374350697_text44601156144811"><a name="zh-cn_topic_0000001374350697_text44601156144811"></a><a name="zh-cn_topic_0000001374350697_text44601156144811"></a></span><span id="zh-cn_topic_0000001374350697_text25101758154816"><a name="zh-cn_topic_0000001374350697_text25101758154816"></a><a name="zh-cn_topic_0000001374350697_text25101758154816"></a>弹性公网IP</span>。</li><li>开启IPv6转换。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="13.389999999999999%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0000001374350697_p6782192011211"><a name="zh-cn_topic_0000001374350697_p6782192011211"></a><a name="zh-cn_topic_0000001374350697_p6782192011211"></a>IPv4网段</p>
</td>
<td class="cellrowborder" valign="top" width="32.16%" headers="mcps1.2.6.1.5 "><a name="zh-cn_topic_0000001374350697_ul19807846241"></a><a name="zh-cn_topic_0000001374350697_ul19807846241"></a><ul id="zh-cn_topic_0000001374350697_ul19807846241"><li><strong id="zh-cn_topic_0000001374350697_b163617451972"><a name="zh-cn_topic_0000001374350697_b163617451972"></a><a name="zh-cn_topic_0000001374350697_b163617451972"></a>IPv4私网地址：</strong>支持IPv4内网通信。</li><li><strong id="zh-cn_topic_0000001374350697_b1273120509711"><a name="zh-cn_topic_0000001374350697_b1273120509711"></a><a name="zh-cn_topic_0000001374350697_b1273120509711"></a>IPv4 EIP地址（开启IPv6转换）：</strong>同时支持IPv4公网通信和IPv6公网通信。</li></ul>
</td>
</tr>
</tbody>
</table>

## IPv6网络应用场景及资源规划<a name="section11683111196"></a>

**图 1**  IPv6网络应用场景及资源规划<a name="zh-cn_topic_0000001374350697_fig18359258135814"></a>  
![](figures/IPv6网络应用场景及资源规划-5.png "IPv6网络应用场景及资源规划-5")

## 开启IPv6转换（申请IPv6弹性公网IP）<a name="section1372725019183"></a>

-   方法一：

    参考[为云主机弹性云服务器申请和绑定弹性IP弹性公网IP](为弹性云服务器申请和绑定弹性公网IP.md)申请弹性公网IP，在申请页面配置参数时，请将“IPv6转换”设置为“开启”，就可以在申请IPv4地址的同时申请一个IPv6弹性公网IP。

    开启IPv6转换后，该弹性公网IP将同时拥有IPv4和IPv6地址，原有IPv4业务可以快速为IPv6用户提供访问能力。

-   方法二：

    当已有的IPv4地址的弹性公网IP需要增加IPv6地址时，可以在弹性公网IP列表页面，找到想转换的IPv4弹性公网IP ，单击操作列“更多”下的“开启IPv6转换”，即可将已有的IPv4弹性公网IP转换为IPv6的。

    开启IPv6转换后，该弹性公网IP将同时拥有IPv4和IPv6地址，原有IPv4业务可以快速为IPv6用户提供访问能力。


>![](public_sys-resources/icon-note.gif) **说明：** 
>开启IPv6转换后，对原有绑定资源的使用无影响。
>目前，支持开启IPv6转换的区域有：华北-北京一、华北-北京四、华东-上海一、华东-上海二、华南-广州。

## 配置安全组<a name="section8240144922017"></a>

开启弹性公网IP的IPv6转换后，请务必在安全组的出方向和入方向中放通198.19.0.0/16网段的IP地址，如[表3](#zh-cn_topic_0000001323190700_eip_0001_table854766319358)所示。因为IPv6 弹性公网IP采用NAT64技术，入方向的源IP地址经过NAT64转换后，会将IPv6地址转换为198.19.0.0/16之间的某个IPv4地址，源端口随机，目的IP为本机的内部私有IPv4地址，目的端口不变。

配置安全组操作请参考[《虚拟私有云用户指南》](https://support.huaweicloud.com/usermanual-vpc/zh-cn_topic_0030969470.html)。

**表 3**  安全组规则

<a name="zh-cn_topic_0000001323190700_eip_0001_table854766319358"></a>
<table><thead align="left"><tr id="zh-cn_topic_0000001323190700_eip_0001_row2051403019358"><th class="cellrowborder" valign="top" width="19.681968196819682%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0000001323190700_eip_0001_p5102371419358"><a name="zh-cn_topic_0000001323190700_eip_0001_p5102371419358"></a><a name="zh-cn_topic_0000001323190700_eip_0001_p5102371419358"></a>方向</p>
</th>
<th class="cellrowborder" valign="top" width="20.782078207820785%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0000001323190700_eip_0001_p3928016319358"><a name="zh-cn_topic_0000001323190700_eip_0001_p3928016319358"></a><a name="zh-cn_topic_0000001323190700_eip_0001_p3928016319358"></a>协议</p>
</th>
<th class="cellrowborder" valign="top" width="59.53595359535954%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0000001323190700_eip_0001_p2415644494621"><a name="zh-cn_topic_0000001323190700_eip_0001_p2415644494621"></a><a name="zh-cn_topic_0000001323190700_eip_0001_p2415644494621"></a>端口和地址</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0000001323190700_eip_0001_row3779122419358"><td class="cellrowborder" valign="top" width="19.681968196819682%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001323190700_eip_0001_p4119033619358"><a name="zh-cn_topic_0000001323190700_eip_0001_p4119033619358"></a><a name="zh-cn_topic_0000001323190700_eip_0001_p4119033619358"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="20.782078207820785%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001323190700_eip_0001_p4808290419358"><a name="zh-cn_topic_0000001323190700_eip_0001_p4808290419358"></a><a name="zh-cn_topic_0000001323190700_eip_0001_p4808290419358"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="59.53595359535954%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001323190700_eip_0001_p4640703694621"><a name="zh-cn_topic_0000001323190700_eip_0001_p4640703694621"></a><a name="zh-cn_topic_0000001323190700_eip_0001_p4640703694621"></a>源地址：198.19.0.0/16</p>
</td>
</tr>
<tr id="zh-cn_topic_0000001323190700_eip_0001_row22818581398"><td class="cellrowborder" valign="top" width="19.681968196819682%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0000001323190700_eip_0001_p6301958495"><a name="zh-cn_topic_0000001323190700_eip_0001_p6301958495"></a><a name="zh-cn_topic_0000001323190700_eip_0001_p6301958495"></a>出方向</p>
</td>
<td class="cellrowborder" valign="top" width="20.782078207820785%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0000001323190700_eip_0001_p730158994"><a name="zh-cn_topic_0000001323190700_eip_0001_p730158994"></a><a name="zh-cn_topic_0000001323190700_eip_0001_p730158994"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="59.53595359535954%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0000001323190700_eip_0001_p7825131612103"><a name="zh-cn_topic_0000001323190700_eip_0001_p7825131612103"></a><a name="zh-cn_topic_0000001323190700_eip_0001_p7825131612103"></a>目的地址：198.19.0.0/16</p>
</td>
</tr>
</tbody>
</table>

## 关闭IPv6转换（释放IPv6弹性公网IP）<a name="section16592348142114"></a>

当弹性公网IP不再需要IPv6地址时，可以在弹性公网IP列表页面，找到想关闭IPv6地址的弹性公网IP ，单击“操作”列的“关闭IPv6转换”，即可删除IPv6地址。删除后，该弹性公网IP仅保留IPv4地址。

