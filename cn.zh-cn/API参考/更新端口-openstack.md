# 更新端口<a name="vpc_port02_0004"></a>

## 功能介绍<a name="zh-cn_topic_0062207392_section23646388"></a>

更新端口。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=NeutronUpdatePort)中直接运行调试该接口。

## URI<a name="zh-cn_topic_0062207392_section11490904"></a>

PUT /v2.0/ports/\{port\_id\}

参数说明请参见[表1](#table1855162528)。

**表 1**  参数说明

<a name="table1855162528"></a>
<table><thead align="left"><tr id="vpc_port02_0002_row1394617591304"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="vpc_port02_0002_p159467591307"><a name="vpc_port02_0002_p159467591307"></a><a name="vpc_port02_0002_p159467591307"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="vpc_port02_0002_p1094612597019"><a name="vpc_port02_0002_p1094612597019"></a><a name="vpc_port02_0002_p1094612597019"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="vpc_port02_0002_p29466591203"><a name="vpc_port02_0002_p29466591203"></a><a name="vpc_port02_0002_p29466591203"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_port02_0002_row1494695918012"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="vpc_port02_0002_p9946159600"><a name="vpc_port02_0002_p9946159600"></a><a name="vpc_port02_0002_p9946159600"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="vpc_port02_0002_p09465594017"><a name="vpc_port02_0002_p09465594017"></a><a name="vpc_port02_0002_p09465594017"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="vpc_port02_0002_p394618591401"><a name="vpc_port02_0002_p394618591401"></a><a name="vpc_port02_0002_p394618591401"></a>端口唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0062207392_section55370462"></a>

**表 2**  请求参数

<a name="zh-cn_topic_0062207392_table10296933"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207392_row62640398"><th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0062207392_p40707460"><a name="zh-cn_topic_0062207392_p40707460"></a><a name="zh-cn_topic_0062207392_p40707460"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.16%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0062207392_p8970000"><a name="zh-cn_topic_0062207392_p8970000"></a><a name="zh-cn_topic_0062207392_p8970000"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0062207392_p55481367"><a name="zh-cn_topic_0062207392_p55481367"></a><a name="zh-cn_topic_0062207392_p55481367"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="65.31%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0062207392_p64805763"><a name="zh-cn_topic_0062207392_p64805763"></a><a name="zh-cn_topic_0062207392_p64805763"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207392_row14775484"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0062207392_p55963561"><a name="zh-cn_topic_0062207392_p55963561"></a><a name="zh-cn_topic_0062207392_p55963561"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="8.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0062207392_p36754611"><a name="zh-cn_topic_0062207392_p36754611"></a><a name="zh-cn_topic_0062207392_p36754611"></a><a href="#table17891153981819">port</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0062207392_p24333505"><a name="zh-cn_topic_0062207392_p24333505"></a><a name="zh-cn_topic_0062207392_p24333505"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="65.31%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0062207386_p50516929"><a name="zh-cn_topic_0062207386_p50516929"></a><a name="zh-cn_topic_0062207386_p50516929"></a>port对象，参见<a href="#table17891153981819">表3</a>。</p>
<p id="zh-cn_topic_0062207392_p22385437"><a name="zh-cn_topic_0062207392_p22385437"></a><a name="zh-cn_topic_0062207392_p22385437"></a>更新操作时至少指定一项属性。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  port对象

<a name="table17891153981819"></a>
<table><thead align="left"><tr id="row188929398187"><th class="cellrowborder" valign="top" width="26.35736426357364%" id="mcps1.2.5.1.1"><p id="p0892193917186"><a name="p0892193917186"></a><a name="p0892193917186"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="15.608439156084392%" id="mcps1.2.5.1.2"><p id="p18759144481919"><a name="p18759144481919"></a><a name="p18759144481919"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.50814918508149%" id="mcps1.2.5.1.3"><p id="p6892163916182"><a name="p6892163916182"></a><a name="p6892163916182"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.52604739526047%" id="mcps1.2.5.1.4"><p id="p1389210394189"><a name="p1389210394189"></a><a name="p1389210394189"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8892203921814"><td class="cellrowborder" valign="top" width="26.35736426357364%" headers="mcps1.2.5.1.1 "><p id="p8892143913188"><a name="p8892143913188"></a><a name="p8892143913188"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="15.608439156084392%" headers="mcps1.2.5.1.2 "><p id="p10759744131910"><a name="p10759744131910"></a><a name="p10759744131910"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.50814918508149%" headers="mcps1.2.5.1.3 "><p id="p168921639181817"><a name="p168921639181817"></a><a name="p168921639181817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p18892339201812"><a name="p18892339201812"></a><a name="p18892339201812"></a>端口的名称</p>
</td>
</tr>
<tr id="row689363918186"><td class="cellrowborder" valign="top" width="26.35736426357364%" headers="mcps1.2.5.1.1 "><p id="p128953395185"><a name="p128953395185"></a><a name="p128953395185"></a>security_groups</p>
</td>
<td class="cellrowborder" valign="top" width="15.608439156084392%" headers="mcps1.2.5.1.2 "><p id="p15759134419199"><a name="p15759134419199"></a><a name="p15759134419199"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.50814918508149%" headers="mcps1.2.5.1.3 "><p id="p448220335811"><a name="p448220335811"></a><a name="p448220335811"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p9895123951816"><a name="p9895123951816"></a><a name="p9895123951816"></a>扩展属性：安全组的UUID，例如："security_groups": ["a0608cbf-d047-4f54-8b28-cd7b59853fff"]</p>
<p id="p1389519392188"><a name="p1389519392188"></a><a name="p1389519392188"></a>【使用说明】不支持更新为空。</p>
</td>
</tr>
<tr id="row15895183961814"><td class="cellrowborder" valign="top" width="26.35736426357364%" headers="mcps1.2.5.1.1 "><p id="p18895039131819"><a name="p18895039131819"></a><a name="p18895039131819"></a>allowed_address_pairs</p>
</td>
<td class="cellrowborder" valign="top" width="15.608439156084392%" headers="mcps1.2.5.1.2 "><p id="p14761104411912"><a name="p14761104411912"></a><a name="p14761104411912"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.50814918508149%" headers="mcps1.2.5.1.3 "><p id="p5114142220534"><a name="p5114142220534"></a><a name="p5114142220534"></a>Array of <a href="#table1389733912184">allow_address_pair</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p1789510391184"><a name="p1789510391184"></a><a name="p1789510391184"></a>扩展属性：IP/Mac对列表，allow_address_pair参见<a href="#table1389733912184">表4</a></p>
<p id="p19895203921819"><a name="p19895203921819"></a><a name="p19895203921819"></a>【使用说明】</p>
<a name="ul14895163913188"></a><a name="ul14895163913188"></a><ul id="ul14895163913188"><li>IP地址不允许为 “0.0.0.0”</li><li>如果allowed_address_pairs配置地址池较大的CIDR（掩码小于24位），建议为该port配置一个单独的安全组</li><li>硬件SDN环境不支持ip_address属性配置为CIDR格式</li><li>为虚拟IP配置后端ECS场景，allowed_address_pairs中配置的IP地址，必须为ECS网卡已有的IP地址，否则可能会导致虚拟IP通信异常。</li></ul>
</td>
</tr>
<tr id="row1889513921812"><td class="cellrowborder" valign="top" width="26.35736426357364%" headers="mcps1.2.5.1.1 "><p id="p289516398183"><a name="p289516398183"></a><a name="p289516398183"></a>extra_dhcp_opts</p>
</td>
<td class="cellrowborder" valign="top" width="15.608439156084392%" headers="mcps1.2.5.1.2 "><p id="p5761174412193"><a name="p5761174412193"></a><a name="p5761174412193"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.50814918508149%" headers="mcps1.2.5.1.3 "><p id="p173831731195712"><a name="p173831731195712"></a><a name="p173831731195712"></a>Array of <a href="#table10898183911816">extra_dhcp_opt</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p1989543981819"><a name="p1989543981819"></a><a name="p1989543981819"></a>扩展属性：DHCP的扩展Option，参见<a href="#table10898183911816">表5</a></p>
</td>
</tr>
<tr id="row2895739131813"><td class="cellrowborder" valign="top" width="26.35736426357364%" headers="mcps1.2.5.1.1 "><p id="p4895123911810"><a name="p4895123911810"></a><a name="p4895123911810"></a>binding:profile</p>
</td>
<td class="cellrowborder" valign="top" width="15.608439156084392%" headers="mcps1.2.5.1.2 "><p id="p4761174416192"><a name="p4761174416192"></a><a name="p4761174416192"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.50814918508149%" headers="mcps1.2.5.1.3 "><p id="p489543912186"><a name="p489543912186"></a><a name="p489543912186"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p9895133913188"><a name="p9895133913188"></a><a name="p9895133913188"></a>扩展属性：提供用户设置自定义信息</p>
<p id="p158951395181"><a name="p158951395181"></a><a name="p158951395181"></a>【使用说明】</p>
<a name="ul198951339131813"></a><a name="ul198951339131813"></a><ul id="ul198951339131813"><li>internal_elb字段，布尔类型，普通租户可见。只有在创建内网ELB的虚拟IP的网卡时设置为true。普通租户没有权限更改该字段，由系统维护。<p id="p14895143901818"><a name="p14895143901818"></a><a name="p14895143901818"></a>举例：</p>
<p id="p1689593911185"><a name="p1689593911185"></a><a name="p1689593911185"></a>{"internal_elb": true}</p>
</li><li>disable_security_groups字段，布尔类型，普通租户可见。默认为false高性能通信场景下，允许指定为true普通租户可见。仅支持创建port和读取时指定。当前仅支持指定为true，不支持指定为false<p id="p489520395187"><a name="p489520395187"></a><a name="p489520395187"></a>举例：</p>
<p id="p1789513951810"><a name="p1789513951810"></a><a name="p1789513951810"></a>{"disable_security_groups"：true }，</p>
<p id="p9895539101812"><a name="p9895539101812"></a><a name="p9895539101812"></a>当前仅支持指定为true，不支持指定为false，指定为true时，FWaaS功能不生效。</p>
</li></ul>
<a name="ul181891610121218"></a><a name="ul181891610121218"></a><ul id="ul181891610121218"><li>仅对于“华北-北京二”：udp_srvports和tcp_srvports，字段，字符串类型，默认不设置udp_srvports和tcp_srvports字段。允许指定udp_srvports和tcp_srvports字段为端口号，表示这些端口的tcp报文和udp报文可支持高并发连接，但是此类报文不受ACL和安全组规则的限制。udp_srvports和tcp_srvports字段同时支持更新操作。<a name="vpc_port02_0001_ul119701359152919"></a><a name="vpc_port02_0001_ul119701359152919"></a><ul id="vpc_port02_0001_ul119701359152919"><li>格式：<p id="vpc_port02_0001_p7108830192916"><a name="vpc_port02_0001_p7108830192916"></a><a name="vpc_port02_0001_p7108830192916"></a>{"tcp_srvports": "port1 port2 port3", "udp_srvports": "port1 port2 port3"}</p>
<p id="vpc_port02_0001_p47335481297"><a name="vpc_port02_0001_p47335481297"></a><a name="vpc_port02_0001_p47335481297"></a>端口号之间以空格间隔，最多允许指定的端口号总共为15个，端口号范围是1到65535。</p>
</li><li>示例：<p id="vpc_port02_0001_p10852165018293"><a name="vpc_port02_0001_p10852165018293"></a><a name="vpc_port02_0001_p10852165018293"></a>{"tcp_srvports": "80 443", "udp_srvports": "53"}</p>
<p id="vpc_port02_0001_p78371519293"><a name="vpc_port02_0001_p78371519293"></a><a name="vpc_port02_0001_p78371519293"></a>示例表示入方向目的端口为80或者443，出方向源端口为80或者443的tcp报文可支持高并发连接。入方向目的端口为53，出方向源端口为53的udp报文可支持高并发连接。但是此类报文不受ACL和安全组规则的限制。</p>
</li></ul>
</li></ul>
<a name="ul16895739131811"></a><a name="ul16895739131811"></a><ul id="ul16895739131811"><li>其他字段，管理员权限，普通租户不可见。</li></ul>
</td>
</tr>
<tr id="row2895143912187"><td class="cellrowborder" valign="top" width="26.35736426357364%" headers="mcps1.2.5.1.1 "><p id="p14895123921817"><a name="p14895123921817"></a><a name="p14895123921817"></a>binding:vnic_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.608439156084392%" headers="mcps1.2.5.1.2 "><p id="p117612443198"><a name="p117612443198"></a><a name="p117612443198"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.50814918508149%" headers="mcps1.2.5.1.3 "><p id="p1289518390188"><a name="p1289518390188"></a><a name="p1289518390188"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p1289523951811"><a name="p1289523951811"></a><a name="p1289523951811"></a>绑定的vNIC类型</p>
<p id="p618195116205"><a name="p618195116205"></a><a name="p618195116205"></a>【使用说明】normal: 软交换</p>
</td>
</tr>
<tr id="row1989563912183"><td class="cellrowborder" valign="top" width="26.35736426357364%" headers="mcps1.2.5.1.1 "><p id="p108951239111814"><a name="p108951239111814"></a><a name="p108951239111814"></a>port_security_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="15.608439156084392%" headers="mcps1.2.5.1.2 "><p id="p1976174451912"><a name="p1976174451912"></a><a name="p1976174451912"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.50814918508149%" headers="mcps1.2.5.1.3 "><p id="p889623941816"><a name="p889623941816"></a><a name="p889623941816"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p3896639151816"><a name="p3896639151816"></a><a name="p3896639151816"></a>端口安全使能标记，如果不使能则安全组和dhcp防欺骗不生效</p>
</td>
</tr>
</tbody>
</table>

**表 4**  allow\_address\_pair对象

<a name="table1389733912184"></a>
<table><thead align="left"><tr id="row6898123971818"><th class="cellrowborder" valign="top" width="22.35%" id="mcps1.2.5.1.1"><p id="p989817398184"><a name="p989817398184"></a><a name="p989817398184"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="10.94%" id="mcps1.2.5.1.2"><p id="p8780192342511"><a name="p8780192342511"></a><a name="p8780192342511"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.19%" id="mcps1.2.5.1.3"><p id="p19898163910181"><a name="p19898163910181"></a><a name="p19898163910181"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.52%" id="mcps1.2.5.1.4"><p id="p5898173961815"><a name="p5898173961815"></a><a name="p5898173961815"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row158982395184"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.2.5.1.1 "><p id="p78981539151812"><a name="p78981539151812"></a><a name="p78981539151812"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="10.94%" headers="mcps1.2.5.1.2 "><p id="p8780182342516"><a name="p8780182342516"></a><a name="p8780182342516"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.19%" headers="mcps1.2.5.1.3 "><p id="p1689833981819"><a name="p1689833981819"></a><a name="p1689833981819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.52%" headers="mcps1.2.5.1.4 "><p id="p1689819398187"><a name="p1689819398187"></a><a name="p1689819398187"></a>IP地址</p>
<p id="p1089812395185"><a name="p1089812395185"></a><a name="p1089812395185"></a>【使用说明】不支持0.0.0.0</p>
</td>
</tr>
<tr id="row98981639201812"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.2.5.1.1 "><p id="p389873910186"><a name="p389873910186"></a><a name="p389873910186"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="10.94%" headers="mcps1.2.5.1.2 "><p id="p2781723152513"><a name="p2781723152513"></a><a name="p2781723152513"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.19%" headers="mcps1.2.5.1.3 "><p id="p148981139191816"><a name="p148981139191816"></a><a name="p148981139191816"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.52%" headers="mcps1.2.5.1.4 "><p id="p11898133911813"><a name="p11898133911813"></a><a name="p11898133911813"></a>MAC地址</p>
</td>
</tr>
</tbody>
</table>

**表 5**  extra\_dhcp\_opt对象

<a name="table10898183911816"></a>
<table><thead align="left"><tr id="row18899143991812"><th class="cellrowborder" valign="top" width="20.96%" id="mcps1.2.5.1.1"><p id="p68991939161818"><a name="p68991939161818"></a><a name="p68991939161818"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="12.6%" id="mcps1.2.5.1.2"><p id="p15243438162518"><a name="p15243438162518"></a><a name="p15243438162518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.15%" id="mcps1.2.5.1.3"><p id="p78991639111813"><a name="p78991639111813"></a><a name="p78991639111813"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.29%" id="mcps1.2.5.1.4"><p id="p28991391181"><a name="p28991391181"></a><a name="p28991391181"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row10899339141820"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.5.1.1 "><p id="p98991039151815"><a name="p98991039151815"></a><a name="p98991039151815"></a>opt_name</p>
</td>
<td class="cellrowborder" valign="top" width="12.6%" headers="mcps1.2.5.1.2 "><p id="p11243113820252"><a name="p11243113820252"></a><a name="p11243113820252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.15%" headers="mcps1.2.5.1.3 "><p id="p118999393186"><a name="p118999393186"></a><a name="p118999393186"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.29%" headers="mcps1.2.5.1.4 "><p id="p189953910181"><a name="p189953910181"></a><a name="p189953910181"></a>Option名称</p>
</td>
</tr>
<tr id="row18899143971815"><td class="cellrowborder" valign="top" width="20.96%" headers="mcps1.2.5.1.1 "><p id="p48991939171810"><a name="p48991939171810"></a><a name="p48991939171810"></a>opt_value</p>
</td>
<td class="cellrowborder" valign="top" width="12.6%" headers="mcps1.2.5.1.2 "><p id="p172437381254"><a name="p172437381254"></a><a name="p172437381254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.15%" headers="mcps1.2.5.1.3 "><p id="p98998398186"><a name="p98998398186"></a><a name="p98998398186"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.29%" headers="mcps1.2.5.1.4 "><p id="p168991839151814"><a name="p168991839151814"></a><a name="p168991839151814"></a>Option值</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0062207392_section28572113"></a>

**表 6**  响应参数

<a name="zh-cn_topic_0062207392_table1281126"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207392_row10321460"><th class="cellrowborder" valign="top" width="22.89%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207392_p30731970"><a name="zh-cn_topic_0062207392_p30731970"></a><a name="zh-cn_topic_0062207392_p30731970"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="27.200000000000003%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207392_p6261652"><a name="zh-cn_topic_0062207392_p6261652"></a><a name="zh-cn_topic_0062207392_p6261652"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.91%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207392_p12079142"><a name="zh-cn_topic_0062207392_p12079142"></a><a name="zh-cn_topic_0062207392_p12079142"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207392_row38886454"><td class="cellrowborder" valign="top" width="22.89%" headers="mcps1.2.4.1.1 "><p id="p18363114152811"><a name="p18363114152811"></a><a name="p18363114152811"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="27.200000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207392_p53234283"><a name="zh-cn_topic_0062207392_p53234283"></a><a name="zh-cn_topic_0062207392_p53234283"></a><a href="#table15919752145624">port</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="49.91%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207392_p35602929"><a name="zh-cn_topic_0062207392_p35602929"></a><a name="zh-cn_topic_0062207392_p35602929"></a>port对象，参见<a href="#table15919752145624">表7</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 7**  port对象

<a name="table15919752145624"></a>
<table><thead align="left"><tr id="row28529169145624"><th class="cellrowborder" valign="top" width="28.499999999999996%" id="mcps1.2.4.1.1"><p id="p42540009145658"><a name="p42540009145658"></a><a name="p42540009145658"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="28.76%" id="mcps1.2.4.1.2"><p id="p23188741145658"><a name="p23188741145658"></a><a name="p23188741145658"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.74%" id="mcps1.2.4.1.3"><p id="p13444574145658"><a name="p13444574145658"></a><a name="p13444574145658"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13166425145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p28807446145658"><a name="p28807446145658"></a><a name="p28807446145658"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p51701793145658"><a name="p51701793145658"></a><a name="p51701793145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p5183528145658"><a name="p5183528145658"></a><a name="p5183528145658"></a>端口的ID，最大长度不超过255</p>
<p id="p189962619371"><a name="p189962619371"></a><a name="p189962619371"></a>【使用说明】在查询端口列表时非必选</p>
</td>
</tr>
<tr id="row1387566145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p20696121145658"><a name="p20696121145658"></a><a name="p20696121145658"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p65773124145658"><a name="p65773124145658"></a><a name="p65773124145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p10771861145658"><a name="p10771861145658"></a><a name="p10771861145658"></a>端口的名称</p>
</td>
</tr>
<tr id="row36437767145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p949776145658"><a name="p949776145658"></a><a name="p949776145658"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p9822997145658"><a name="p9822997145658"></a><a name="p9822997145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p36061910145658"><a name="p36061910145658"></a><a name="p36061910145658"></a>所属网络的ID</p>
</td>
</tr>
<tr id="row41410455145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p49567182145658"><a name="p49567182145658"></a><a name="p49567182145658"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p55518807145658"><a name="p55518807145658"></a><a name="p55518807145658"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p26909682145658"><a name="p26909682145658"></a><a name="p26909682145658"></a>管理状态</p>
<p id="p40860550145658"><a name="p40860550145658"></a><a name="p40860550145658"></a>【使用说明】只支持true</p>
</td>
</tr>
<tr id="row11261085145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p58114882145658"><a name="p58114882145658"></a><a name="p58114882145658"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p9685031145658"><a name="p9685031145658"></a><a name="p9685031145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p8831008145658"><a name="p8831008145658"></a><a name="p8831008145658"></a>端口MAC地址，例如："mac_address": "fa:16:3e:9e:ff:55"</p>
<p id="p12370211145658"><a name="p12370211145658"></a><a name="p12370211145658"></a>【使用说明】只支持系统动态分配，不支持指定</p>
</td>
</tr>
<tr id="row59425565145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p25296431145658"><a name="p25296431145658"></a><a name="p25296431145658"></a>fixed_ips</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p52484625913"><a name="p52484625913"></a><a name="p52484625913"></a>Array of <a href="#table4290920914597">fixed_ip</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p48560910145658"><a name="p48560910145658"></a><a name="p48560910145658"></a>端口IP，参见<a href="#table4290920914597">表8</a>。例如："fixed_ips": [{"subnet_id": "4dc70db6-cb7f-4200-9790-a6a910776bba", "ip_address": "192.169.25.79"}]</p>
</td>
</tr>
<tr id="row52336547145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p42357933145658"><a name="p42357933145658"></a><a name="p42357933145658"></a>device_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p8440512145658"><a name="p8440512145658"></a><a name="p8440512145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p23990357145658"><a name="p23990357145658"></a><a name="p23990357145658"></a>设备ID</p>
<p id="p14586626145658"><a name="p14586626145658"></a><a name="p14586626145658"></a>【使用说明】不支持设置和更新，由系统自动维护，该字段非空的端口不允许删除</p>
</td>
</tr>
<tr id="row8304195145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p30450002145658"><a name="p30450002145658"></a><a name="p30450002145658"></a>device_owner</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p50531130145658"><a name="p50531130145658"></a><a name="p50531130145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p60282892145658"><a name="p60282892145658"></a><a name="p60282892145658"></a>设备所属（DHCP/Router/ Nova等）</p>
<p id="p2837225125711"><a name="p2837225125711"></a><a name="p2837225125711"></a>【使用说明】不支持更新，只允许用户在创建虚拟IP端口时，为虚拟IP端口设置device_owner为neutron:VIP_PORT，当端口的该字段不为空时，仅支持该字段为neutron:VIP_PORT时的端口删除。</p>
<p id="p1458812975819"><a name="p1458812975819"></a><a name="p1458812975819"></a>该字段非空的端口不允许删除。</p>
</td>
</tr>
<tr id="row47218120145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p43524921145658"><a name="p43524921145658"></a><a name="p43524921145658"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p35857692145658"><a name="p35857692145658"></a><a name="p35857692145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row925022145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p12676379145658"><a name="p12676379145658"></a><a name="p12676379145658"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p20153784145658"><a name="p20153784145658"></a><a name="p20153784145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p12312282145658"><a name="p12312282145658"></a><a name="p12312282145658"></a>端口状态，可以为ACTIVE，BUILD，DOWN；</p>
<p id="p43701677145658"><a name="p43701677145658"></a><a name="p43701677145658"></a>【使用说明】Hana硬直通虚拟机端口状态总为DOWN</p>
</td>
</tr>
<tr id="row36940776145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p48921078145658"><a name="p48921078145658"></a><a name="p48921078145658"></a>security_groups</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p3184354145658"><a name="p3184354145658"></a><a name="p3184354145658"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p4527282145658"><a name="p4527282145658"></a><a name="p4527282145658"></a>扩展属性：安全组的UUID，例如："security_groups": ["a0608cbf-d047-4f54-8b28-cd7b59853fff"]</p>
<p id="p103001912487"><a name="p103001912487"></a><a name="p103001912487"></a>【使用说明】不支持更新为空。</p>
</td>
</tr>
<tr id="row17626705145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p41382197145658"><a name="p41382197145658"></a><a name="p41382197145658"></a>allowed_address_pairs</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p11976131610013"><a name="p11976131610013"></a><a name="p11976131610013"></a>Array of <a href="#zh-cn_topic_0062207355_table57914257">allow_address_pair</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p30975735145658"><a name="p30975735145658"></a><a name="p30975735145658"></a>扩展属性：IP/Mac对列表，allow_address_pair参见<a href="#zh-cn_topic_0062207355_table57914257">表9</a></p>
<p id="p7136530194312"><a name="p7136530194312"></a><a name="p7136530194312"></a>【使用说明】</p>
<a name="ul18386852174311"></a><a name="ul18386852174311"></a><ul id="ul18386852174311"><li>IP地址不允许为 “0.0.0.0”</li><li>如果allowed_address_pairs配置地址池较大的CIDR（掩码小于24位），建议为该port配置一个单独的安全组</li><li>硬件SDN环境不支持ip_address属性配置为CIDR格式</li><li>为虚拟IP配置后端ECS场景，allowed_address_pairs中配置的IP地址，必须为ECS网卡已有的IP地址，否则可能会导致虚拟IP通信异常。</li></ul>
</td>
</tr>
<tr id="row938573145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p34089655145658"><a name="p34089655145658"></a><a name="p34089655145658"></a>extra_dhcp_opts</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p251517111015"><a name="p251517111015"></a><a name="p251517111015"></a>Array of <a href="#table5056075615524">extra_dhcp_opt</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p45787521145658"><a name="p45787521145658"></a><a name="p45787521145658"></a>扩展属性：DHCP的扩展Option，参见<a href="#table5056075615524">表10</a></p>
</td>
</tr>
<tr id="row46629855145636"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p62371645145658"><a name="p62371645145658"></a><a name="p62371645145658"></a>binding:vif_details</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p18938488145658"><a name="p18938488145658"></a><a name="p18938488145658"></a><a href="#table72371439857">binding:vif_details</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p62312767145658"><a name="p62312767145658"></a><a name="p62312767145658"></a>vif的详细信息，参见<a href="#table72371439857">表11</a></p>
</td>
</tr>
<tr id="row35771758145636"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p7522524145658"><a name="p7522524145658"></a><a name="p7522524145658"></a>binding:profile</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p5344685145658"><a name="p5344685145658"></a><a name="p5344685145658"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p4278449145658"><a name="p4278449145658"></a><a name="p4278449145658"></a>扩展属性：提供用户设置自定义信息</p>
<p id="p38506045145658"><a name="p38506045145658"></a><a name="p38506045145658"></a>【使用说明】</p>
<a name="ul11010089145658"></a><a name="ul11010089145658"></a><ul id="ul11010089145658"><li>internal_elb字段，布尔类型，普通租户可见。只有在创建内网ELB的虚拟IP的网卡时设置为true。普通租户没有权限更改该字段，由系统维护。<p id="p041674418210"><a name="p041674418210"></a><a name="p041674418210"></a>举例：</p>
<p id="p1774284092111"><a name="p1774284092111"></a><a name="p1774284092111"></a>{"internal_elb": true}</p>
</li><li>disable_security_groups字段，布尔类型，普通租户可见。默认为false高性能通信场景下，允许指定为true普通租户可见。仅支持创建port和读取时指定。当前仅支持指定为true，不支持指定为false<p id="p19402030145658"><a name="p19402030145658"></a><a name="p19402030145658"></a>举例：</p>
<p id="p40400544145658"><a name="p40400544145658"></a><a name="p40400544145658"></a>{"disable_security_groups"：true }，</p>
<p id="p28060583145658"><a name="p28060583145658"></a><a name="p28060583145658"></a>当前仅支持指定为true，不支持指定为false，指定为true时，FWaaS功能不生效。</p>
</li></ul>
<a name="ul83681416151219"></a><a name="ul83681416151219"></a><ul id="ul83681416151219"><li>仅对于“华北-北京二”：udp_srvports和tcp_srvports，字段，字符串类型，默认不设置udp_srvports和tcp_srvports字段。允许指定udp_srvports和tcp_srvports字段为端口号，表示这些端口的tcp报文和udp报文可支持高并发连接，但是此类报文不受ACL和安全组规则的限制。udp_srvports和tcp_srvports字段同时支持更新操作。<a name="vpc_port02_0001_ul119701359152919_1"></a><a name="vpc_port02_0001_ul119701359152919_1"></a><ul id="vpc_port02_0001_ul119701359152919_1"><li>格式：<p id="vpc_port02_0001_p7108830192916_1"><a name="vpc_port02_0001_p7108830192916_1"></a><a name="vpc_port02_0001_p7108830192916_1"></a>{"tcp_srvports": "port1 port2 port3", "udp_srvports": "port1 port2 port3"}</p>
<p id="vpc_port02_0001_p47335481297_1"><a name="vpc_port02_0001_p47335481297_1"></a><a name="vpc_port02_0001_p47335481297_1"></a>端口号之间以空格间隔，最多允许指定的端口号总共为15个，端口号范围是1到65535。</p>
</li><li>示例：<p id="vpc_port02_0001_p10852165018293_1"><a name="vpc_port02_0001_p10852165018293_1"></a><a name="vpc_port02_0001_p10852165018293_1"></a>{"tcp_srvports": "80 443", "udp_srvports": "53"}</p>
<p id="vpc_port02_0001_p78371519293_1"><a name="vpc_port02_0001_p78371519293_1"></a><a name="vpc_port02_0001_p78371519293_1"></a>示例表示入方向目的端口为80或者443，出方向源端口为80或者443的tcp报文可支持高并发连接。入方向目的端口为53，出方向源端口为53的udp报文可支持高并发连接。但是此类报文不受ACL和安全组规则的限制。</p>
</li></ul>
</li></ul>
<a name="ul51218659145658"></a><a name="ul51218659145658"></a>
</td>
</tr>
<tr id="row63233200145636"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p4700493145658"><a name="p4700493145658"></a><a name="p4700493145658"></a>binding:vnic_type</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p45195649145658"><a name="p45195649145658"></a><a name="p45195649145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p42146344145658"><a name="p42146344145658"></a><a name="p42146344145658"></a>绑定的vNIC类型</p>
<p id="p43772780145658"><a name="p43772780145658"></a><a name="p43772780145658"></a>normal: 软交换</p>
</td>
</tr>
<tr id="row37613242198"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p20178562198"><a name="p20178562198"></a><a name="p20178562198"></a>port_security_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p532005162198"><a name="p532005162198"></a><a name="p532005162198"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p184376702198"><a name="p184376702198"></a><a name="p184376702198"></a>端口安全使能标记，如果不使能则安全组和dhcp防欺骗不生效</p>
</td>
</tr>
<tr id="row167271926144411"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p117281926144417"><a name="p117281926144417"></a><a name="p117281926144417"></a>dns_assignment</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p1272862616446"><a name="p1272862616446"></a><a name="p1272862616446"></a>Array of <a href="#table1960316535179">dns_assignment</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p1472919269447"><a name="p1472919269447"></a><a name="p1472919269447"></a>扩展属性：主网卡默认内网域名信息</p>
<p id="p1834325274510"><a name="p1834325274510"></a><a name="p1834325274510"></a>【使用说明】不支持设置和更新，由系统自动维护</p>
<a name="ul1766216288464"></a><a name="ul1766216288464"></a><ul id="ul1766216288464"><li>hostname：与端口dns_name一致</li><li>ip_address：端口ipv4私有地址</li><li>fqdn：为端口创建默认内网fqdn</li></ul>
</td>
</tr>
<tr id="row119851851490"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p39859518498"><a name="p39859518498"></a><a name="p39859518498"></a>dns_name</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p139852519498"><a name="p139852519498"></a><a name="p139852519498"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p098555164915"><a name="p098555164915"></a><a name="p098555164915"></a>扩展属性：主网卡默认内网DNS名称</p>
<p id="p11538191913508"><a name="p11538191913508"></a><a name="p11538191913508"></a>【使用说明】不支持设置和更新，由系统自动维护，访问该默认内网域名前，请确保子网使用当前系统提供的DNS</p>
</td>
</tr>
<tr id="row8784124710810"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p759775317217"><a name="p759775317217"></a><a name="p759775317217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p765335213239"><a name="p765335213239"></a><a name="p765335213239"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row19797526919"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间，UTC时间</p>
<p id="p65980291419"><a name="p65980291419"></a><a name="p65980291419"></a>格式yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row124097610917"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间，UTC时间</p>
<p id="p17388812174410"><a name="p17388812174410"></a><a name="p17388812174410"></a>格式yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

**表 8**  fixed\_ip对象

<a name="table4290920914597"></a>
<table><thead align="left"><tr id="row3523499914597"><th class="cellrowborder" valign="top" width="25.95259525952595%" id="mcps1.2.4.1.1"><p id="p6174509115118"><a name="p6174509115118"></a><a name="p6174509115118"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="25.95259525952595%" id="mcps1.2.4.1.2"><p id="p3529643715118"><a name="p3529643715118"></a><a name="p3529643715118"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.09480948094809%" id="mcps1.2.4.1.3"><p id="p2048854115118"><a name="p2048854115118"></a><a name="p2048854115118"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2319879914597"><td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.1 "><p id="p626497215118"><a name="p626497215118"></a><a name="p626497215118"></a>subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.2 "><p id="p3770069415118"><a name="p3770069415118"></a><a name="p3770069415118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.09480948094809%" headers="mcps1.2.4.1.3 "><p id="p2612244315118"><a name="p2612244315118"></a><a name="p2612244315118"></a>所属子网ID</p>
<p id="p3377540315118"><a name="p3377540315118"></a><a name="p3377540315118"></a>【使用说明】不支持更新</p>
</td>
</tr>
<tr id="row636738414597"><td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.1 "><p id="p6042468915118"><a name="p6042468915118"></a><a name="p6042468915118"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.2 "><p id="p6256165915118"><a name="p6256165915118"></a><a name="p6256165915118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.09480948094809%" headers="mcps1.2.4.1.3 "><p id="p1336175915118"><a name="p1336175915118"></a><a name="p1336175915118"></a>端口IP地址</p>
<p id="p5314696715118"><a name="p5314696715118"></a><a name="p5314696715118"></a>【使用说明】不支持更新</p>
</td>
</tr>
</tbody>
</table>

**表 9**  allow\_address\_pair对象

<a name="zh-cn_topic_0062207355_table57914257"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207355_row41852331"><th class="cellrowborder" valign="top" width="25.81%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207355_p34595685"><a name="zh-cn_topic_0062207355_p34595685"></a><a name="zh-cn_topic_0062207355_p34595685"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="26.240000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207355_p50787128"><a name="zh-cn_topic_0062207355_p50787128"></a><a name="zh-cn_topic_0062207355_p50787128"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="47.949999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207355_p52626454"><a name="zh-cn_topic_0062207355_p52626454"></a><a name="zh-cn_topic_0062207355_p52626454"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207355_row34884411"><td class="cellrowborder" valign="top" width="25.81%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207355_p7065065"><a name="zh-cn_topic_0062207355_p7065065"></a><a name="zh-cn_topic_0062207355_p7065065"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="26.240000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207355_p35399367"><a name="zh-cn_topic_0062207355_p35399367"></a><a name="zh-cn_topic_0062207355_p35399367"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.949999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207355_p64721603"><a name="zh-cn_topic_0062207355_p64721603"></a><a name="zh-cn_topic_0062207355_p64721603"></a>IP地址</p>
<p id="zh-cn_topic_0062207355_p45623521"><a name="zh-cn_topic_0062207355_p45623521"></a><a name="zh-cn_topic_0062207355_p45623521"></a>【使用说明】不支持0.0.0.0</p>
</td>
</tr>
<tr id="zh-cn_topic_0062207355_row7958508"><td class="cellrowborder" valign="top" width="25.81%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207355_p40659381"><a name="zh-cn_topic_0062207355_p40659381"></a><a name="zh-cn_topic_0062207355_p40659381"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="26.240000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207355_p5075526"><a name="zh-cn_topic_0062207355_p5075526"></a><a name="zh-cn_topic_0062207355_p5075526"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.949999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207355_p51982593"><a name="zh-cn_topic_0062207355_p51982593"></a><a name="zh-cn_topic_0062207355_p51982593"></a>MAC地址</p>
</td>
</tr>
</tbody>
</table>

**表 10**  extra\_dhcp\_opt对象

<a name="table5056075615524"></a>
<table><thead align="left"><tr id="row739480215524"><th class="cellrowborder" valign="top" width="25.892589258925895%" id="mcps1.2.4.1.1"><p id="p3368663215532"><a name="p3368663215532"></a><a name="p3368663215532"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="26.072607260726073%" id="mcps1.2.4.1.2"><p id="p4426268215532"><a name="p4426268215532"></a><a name="p4426268215532"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.03480348034804%" id="mcps1.2.4.1.3"><p id="p3407518415532"><a name="p3407518415532"></a><a name="p3407518415532"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2636755215524"><td class="cellrowborder" valign="top" width="25.892589258925895%" headers="mcps1.2.4.1.1 "><p id="p2765891815532"><a name="p2765891815532"></a><a name="p2765891815532"></a>opt_name</p>
</td>
<td class="cellrowborder" valign="top" width="26.072607260726073%" headers="mcps1.2.4.1.2 "><p id="p2577986315532"><a name="p2577986315532"></a><a name="p2577986315532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.03480348034804%" headers="mcps1.2.4.1.3 "><p id="p5884162715532"><a name="p5884162715532"></a><a name="p5884162715532"></a>Option名称</p>
</td>
</tr>
<tr id="row3942590315524"><td class="cellrowborder" valign="top" width="25.892589258925895%" headers="mcps1.2.4.1.1 "><p id="p1298235215532"><a name="p1298235215532"></a><a name="p1298235215532"></a>opt_value</p>
</td>
<td class="cellrowborder" valign="top" width="26.072607260726073%" headers="mcps1.2.4.1.2 "><p id="p4493762615532"><a name="p4493762615532"></a><a name="p4493762615532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.03480348034804%" headers="mcps1.2.4.1.3 "><p id="p5057146315532"><a name="p5057146315532"></a><a name="p5057146315532"></a>Option值</p>
</td>
</tr>
</tbody>
</table>

**表 11**  binding:vif\_details对象

<a name="table72371439857"></a>
<table><thead align="left"><tr id="vpc_port02_0002_row12317239452"><th class="cellrowborder" valign="top" width="24.267573242675734%" id="mcps1.2.4.1.1"><p id="vpc_port02_0002_p63171391658"><a name="vpc_port02_0002_p63171391658"></a><a name="vpc_port02_0002_p63171391658"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.52804719528047%" id="mcps1.2.4.1.2"><p id="vpc_port02_0002_p9317839756"><a name="vpc_port02_0002_p9317839756"></a><a name="vpc_port02_0002_p9317839756"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.204379562043805%" id="mcps1.2.4.1.3"><p id="vpc_port02_0002_p531716396519"><a name="vpc_port02_0002_p531716396519"></a><a name="vpc_port02_0002_p531716396519"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_port02_0002_row23171239156"><td class="cellrowborder" valign="top" width="24.267573242675734%" headers="mcps1.2.4.1.1 "><p id="vpc_port02_0002_p1831793913514"><a name="vpc_port02_0002_p1831793913514"></a><a name="vpc_port02_0002_p1831793913514"></a>primary_interface</p>
</td>
<td class="cellrowborder" valign="top" width="19.52804719528047%" headers="mcps1.2.4.1.2 "><p id="vpc_port02_0002_p1431753910515"><a name="vpc_port02_0002_p1431753910515"></a><a name="vpc_port02_0002_p1431753910515"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="56.204379562043805%" headers="mcps1.2.4.1.3 "><p id="vpc_port02_0002_p15138343119"><a name="vpc_port02_0002_p15138343119"></a><a name="vpc_port02_0002_p15138343119"></a>取值为true，表示是虚拟机的主网卡。</p>
</td>
</tr>
</tbody>
</table>

**表 12**  dns\_assignment对象

<a name="table1960316535179"></a>
<table><thead align="left"><tr id="vpc_port01_0006_row860475311718"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="vpc_port01_0006_p85811122186"><a name="vpc_port01_0006_p85811122186"></a><a name="vpc_port01_0006_p85811122186"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="vpc_port01_0006_p145819129183"><a name="vpc_port01_0006_p145819129183"></a><a name="vpc_port01_0006_p145819129183"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="vpc_port01_0006_p95841215189"><a name="vpc_port01_0006_p95841215189"></a><a name="vpc_port01_0006_p95841215189"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_port01_0006_row126042530175"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="vpc_port01_0006_p5604753181710"><a name="vpc_port01_0006_p5604753181710"></a><a name="vpc_port01_0006_p5604753181710"></a>hostname</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="vpc_port01_0006_p1160475381714"><a name="vpc_port01_0006_p1160475381714"></a><a name="vpc_port01_0006_p1160475381714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="vpc_port01_0006_p5604185321716"><a name="vpc_port01_0006_p5604185321716"></a><a name="vpc_port01_0006_p5604185321716"></a>端口hostname</p>
</td>
</tr>
<tr id="vpc_port01_0006_row12604185316171"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="vpc_port01_0006_p12604185301714"><a name="vpc_port01_0006_p12604185301714"></a><a name="vpc_port01_0006_p12604185301714"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="vpc_port01_0006_p12604125311719"><a name="vpc_port01_0006_p12604125311719"></a><a name="vpc_port01_0006_p12604125311719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="vpc_port01_0006_p1060417536175"><a name="vpc_port01_0006_p1060417536175"></a><a name="vpc_port01_0006_p1060417536175"></a>端口IP地址</p>
</td>
</tr>
<tr id="vpc_port01_0006_row1860435321719"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="vpc_port01_0006_p760425311178"><a name="vpc_port01_0006_p760425311178"></a><a name="vpc_port01_0006_p760425311178"></a>fqdn</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="vpc_port01_0006_p1960465391715"><a name="vpc_port01_0006_p1960465391715"></a><a name="vpc_port01_0006_p1960465391715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="vpc_port01_0006_p1860485318172"><a name="vpc_port01_0006_p1860485318172"></a><a name="vpc_port01_0006_p1860485318172"></a>端口内网fqdn</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0062207392_section55822426"></a>

请求样例

```
PUT https://{Endpoint}/v2.0/ports/7a9a954a-eb41-4954-a300-11ab17a361a2 
 
{
    "port": {
           "name": "port-test02"
    }
}
```

响应样例

```
{
    "port": {
        "id": "a7d98f3c-b42f-460b-96a1-07601e145961",
        "name": "port-test02",
        "status": "DOWN",
        "admin_state_up": true,
        "fixed_ips": [],
        "mac_address": "fa:16:3e:01:f7:90",
        "network_id": "00ae08c5-f727-49ab-ad4b-b069398aa171",
        "tenant_id": "db82c9e1415a464ea68048baa8acc6b8",
        "project_id": "db82c9e1415a464ea68048baa8acc6b8",
        "device_id": "",
        "device_owner": "",
        "security_groups": [
            "d0d58aa9-cda9-414c-9c52-6c3daf8534e6"
        ],
        "extra_dhcp_opts": [],
        "allowed_address_pairs": [],
        "binding:vnic_type": "normal",
        "binding:vif_details": {},
        "binding:profile": {},
        "port_security_enabled": true,
        "created_at": "2018-09-20T01:45:26",
        "updated_at": "2018-09-20T01:48:56"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

