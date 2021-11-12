# 创建端口<a name="vpc_port02_0003"></a>

## 功能介绍<a name="zh-cn_topic_0062207340_section45663083"></a>

创建端口。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=NeutronCreatePort)中直接运行调试该接口。

## URI<a name="zh-cn_topic_0062207340_section8314568"></a>

POST /v2.0/ports

## 请求消息<a name="zh-cn_topic_0062207340_section21522370"></a>

**表 1**  请求参数

<a name="zh-cn_topic_0062207340_table29618759"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207340_row3151905"><th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0062207340_p53977738"><a name="zh-cn_topic_0062207340_p53977738"></a><a name="zh-cn_topic_0062207340_p53977738"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="10.2%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0062207340_p10120656"><a name="zh-cn_topic_0062207340_p10120656"></a><a name="zh-cn_topic_0062207340_p10120656"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.16%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0062207340_p14466778"><a name="zh-cn_topic_0062207340_p14466778"></a><a name="zh-cn_topic_0062207340_p14466778"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="67.35%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0062207340_p30958352"><a name="zh-cn_topic_0062207340_p30958352"></a><a name="zh-cn_topic_0062207340_p30958352"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207340_row24598620"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0062207340_p46331171"><a name="zh-cn_topic_0062207340_p46331171"></a><a name="zh-cn_topic_0062207340_p46331171"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="10.2%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0062207340_p61837391"><a name="zh-cn_topic_0062207340_p61837391"></a><a name="zh-cn_topic_0062207340_p61837391"></a><a href="#table15919752145624">port</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="8.16%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0062207340_p42772808"><a name="zh-cn_topic_0062207340_p42772808"></a><a name="zh-cn_topic_0062207340_p42772808"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.35%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0062207340_p42045429"><a name="zh-cn_topic_0062207340_p42045429"></a><a name="zh-cn_topic_0062207340_p42045429"></a>port对象列表，参见<a href="#table15919752145624">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  port对象

<a name="table15919752145624"></a>
<table><thead align="left"><tr id="row28529169145624"><th class="cellrowborder" valign="top" width="21.617838216178384%" id="mcps1.2.5.1.1"><p id="p42540009145658"><a name="p42540009145658"></a><a name="p42540009145658"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="16.238376162383762%" id="mcps1.2.5.1.2"><p id="p12649155111318"><a name="p12649155111318"></a><a name="p12649155111318"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="22.617738226177384%" id="mcps1.2.5.1.3"><p id="p23188741145658"><a name="p23188741145658"></a><a name="p23188741145658"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.52604739526047%" id="mcps1.2.5.1.4"><p id="p13444574145658"><a name="p13444574145658"></a><a name="p13444574145658"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1387566145624"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p20696121145658"><a name="p20696121145658"></a><a name="p20696121145658"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p1164911519139"><a name="p1164911519139"></a><a name="p1164911519139"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p65773124145658"><a name="p65773124145658"></a><a name="p65773124145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p10771861145658"><a name="p10771861145658"></a><a name="p10771861145658"></a>端口的名称</p>
</td>
</tr>
<tr id="row36437767145624"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p949776145658"><a name="p949776145658"></a><a name="p949776145658"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p13649951101311"><a name="p13649951101311"></a><a name="p13649951101311"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p9822997145658"><a name="p9822997145658"></a><a name="p9822997145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><a name="ul11467183751510"></a><a name="ul11467183751510"></a><ul id="ul11467183751510"><li>功能说明：端口所属网络的ID</li><li>约束：必须是存在的网络ID</li></ul>
<div class="note" id="note202751315165"><a name="note202751315165"></a><a name="note202751315165"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="vpc_port01_0006_p192202399225"><a name="vpc_port01_0006_p192202399225"></a><a name="vpc_port01_0006_p192202399225"></a>网络ID的获取方式：</p>
<a name="vpc_port01_0006_ul19184152410233"></a><a name="vpc_port01_0006_ul19184152410233"></a><ul id="vpc_port01_0006_ul19184152410233"><li>方法1：登录虚拟私有云服务的控制台界面，单击VPC下的子网，进入子网详情页面，查找网络ID。</li><li>方法2：通过虚拟私有云服务的API接口查询，具体操作可参考<a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0003.html" target="_blank" rel="noopener noreferrer">查询子网列表</a>。</li></ul>
</div></div>
</td>
</tr>
<tr id="row59425565145624"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p25296431145658"><a name="p25296431145658"></a><a name="p25296431145658"></a>fixed_ips</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p7649105119133"><a name="p7649105119133"></a><a name="p7649105119133"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p19425171418512"><a name="p19425171418512"></a><a name="p19425171418512"></a>Array of <a href="#table335683819394">fixed_ip</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p48560910145658"><a name="p48560910145658"></a><a name="p48560910145658"></a>端口IP，参见<a href="#table335683819394">表3</a>。例如："fixed_ips": [{"subnet_id": "4dc70db6-cb7f-4200-9790-a6a910776bba", "ip_address": "192.169.25.79"}]</p>
</td>
</tr>
<tr id="row36940776145630"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p48921078145658"><a name="p48921078145658"></a><a name="p48921078145658"></a>security_groups</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p265175111316"><a name="p265175111316"></a><a name="p265175111316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p3184354145658"><a name="p3184354145658"></a><a name="p3184354145658"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p4527282145658"><a name="p4527282145658"></a><a name="p4527282145658"></a>扩展属性：安全组的UUID，例如："security_groups": ["a0608cbf-d047-4f54-8b28-cd7b59853fff"]</p>
<p id="p103001912487"><a name="p103001912487"></a><a name="p103001912487"></a>【使用说明】不支持更新为空。</p>
</td>
</tr>
<tr id="row17626705145630"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p41382197145658"><a name="p41382197145658"></a><a name="p41382197145658"></a>allowed_address_pairs</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p3651451141318"><a name="p3651451141318"></a><a name="p3651451141318"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p380974085115"><a name="p380974085115"></a><a name="p380974085115"></a>Array of <a href="#zh-cn_topic_0062207355_table57914257">allow_address_pair</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p30975735145658"><a name="p30975735145658"></a><a name="p30975735145658"></a>扩展属性：IP/Mac对列表，allow_address_pair参见<a href="#zh-cn_topic_0062207355_table57914257">表4</a></p>
<p id="p7136530194312"><a name="p7136530194312"></a><a name="p7136530194312"></a>【使用说明】</p>
<a name="ul18386852174311"></a><a name="ul18386852174311"></a><ul id="ul18386852174311"><li>IP地址不允许为 “0.0.0.0”</li><li>如果allowed_address_pairs配置地址池较大的CIDR（掩码小于24位），建议为该port配置一个单独的安全组</li><li>如果allowed_address_pairs为“1.1.1.1/0”，表示关闭源目地址检查开关</li><li>硬件SDN环境不支持ip_address属性配置为CIDR格式</li><li>为虚拟IP配置后端ECS场景，allowed_address_pairs中配置的IP地址，必须为ECS网卡已有的IP地址，否则可能会导致虚拟IP通信异常</li><li>被绑定的云服务器网卡allowed_address_pairs填“1.1.1.1/0”</li></ul>
</td>
</tr>
<tr id="row938573145630"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p34089655145658"><a name="p34089655145658"></a><a name="p34089655145658"></a>extra_dhcp_opts</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p76511051151311"><a name="p76511051151311"></a><a name="p76511051151311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p157814465211"><a name="p157814465211"></a><a name="p157814465211"></a>Array of <a href="#table5056075615524">extra_dhcp_opt</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p45787521145658"><a name="p45787521145658"></a><a name="p45787521145658"></a>扩展属性：DHCP的扩展Option，参见<a href="#table5056075615524">表5</a></p>
</td>
</tr>
<tr id="row35771758145636"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p7522524145658"><a name="p7522524145658"></a><a name="p7522524145658"></a>binding:profile</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p9651115116136"><a name="p9651115116136"></a><a name="p9651115116136"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p782052216191"><a name="p782052216191"></a><a name="p782052216191"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p4278449145658"><a name="p4278449145658"></a><a name="p4278449145658"></a>扩展属性：提供用户设置自定义信息</p>
<p id="p38506045145658"><a name="p38506045145658"></a><a name="p38506045145658"></a>【使用说明】</p>
<a name="ul11010089145658"></a><a name="ul11010089145658"></a><ul id="ul11010089145658"><li>internal_elb字段，布尔类型，普通租户可见。只有在创建内网ELB的虚拟IP的网卡时设置为true。普通租户没有权限更改该字段，由系统维护。<p id="p041674418210"><a name="p041674418210"></a><a name="p041674418210"></a>举例：</p>
<p id="p1774284092111"><a name="p1774284092111"></a><a name="p1774284092111"></a>{"internal_elb": true}</p>
</li><li>disable_security_groups字段，布尔类型，普通租户可见。默认为false高性能通信场景下，允许指定为true普通租户可见。仅支持创建port和读取时指定。当前仅支持指定为true，不支持指定为false<p id="p19402030145658"><a name="p19402030145658"></a><a name="p19402030145658"></a>举例：</p>
<p id="p40400544145658"><a name="p40400544145658"></a><a name="p40400544145658"></a>{"disable_security_groups"：true }，</p>
<p id="p28060583145658"><a name="p28060583145658"></a><a name="p28060583145658"></a>当前仅支持指定为true，不支持指定为false，指定为true时，FWaaS功能不生效。</p>
</li></ul>
<a name="ul12109162518113"></a><a name="ul12109162518113"></a><ul id="ul12109162518113"><li>仅对于“华北-北京二”：udp_srvports和tcp_srvports，字段，字符串类型，默认不设置udp_srvports和tcp_srvports字段。允许指定udp_srvports和tcp_srvports字段为端口号，表示这些端口的tcp报文和udp报文可支持高并发连接，但是此类报文不受ACL和安全组规则的限制。udp_srvports和tcp_srvports字段同时支持更新操作。<a name="vpc_port02_0001_ul119701359152919"></a><a name="vpc_port02_0001_ul119701359152919"></a><ul id="vpc_port02_0001_ul119701359152919"><li>格式：<p id="vpc_port02_0001_p7108830192916"><a name="vpc_port02_0001_p7108830192916"></a><a name="vpc_port02_0001_p7108830192916"></a>{"tcp_srvports": "port1 port2 port3", "udp_srvports": "port1 port2 port3"}</p>
<p id="vpc_port02_0001_p47335481297"><a name="vpc_port02_0001_p47335481297"></a><a name="vpc_port02_0001_p47335481297"></a>端口号之间以空格间隔，最多允许指定的端口号总共为15个，端口号范围是1到65535。</p>
</li><li>示例：<p id="vpc_port02_0001_p10852165018293"><a name="vpc_port02_0001_p10852165018293"></a><a name="vpc_port02_0001_p10852165018293"></a>{"tcp_srvports": "80 443", "udp_srvports": "53"}</p>
<p id="vpc_port02_0001_p78371519293"><a name="vpc_port02_0001_p78371519293"></a><a name="vpc_port02_0001_p78371519293"></a>示例表示入方向目的端口为80或者443，出方向源端口为80或者443的tcp报文可支持高并发连接。入方向目的端口为53，出方向源端口为53的udp报文可支持高并发连接。但是此类报文不受ACL和安全组规则的限制。</p>
</li></ul>
</li></ul>
<a name="ul51218659145658"></a><a name="ul51218659145658"></a>
</td>
</tr>
<tr id="row63233200145636"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p4700493145658"><a name="p4700493145658"></a><a name="p4700493145658"></a>binding:vnic_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p2065120517132"><a name="p2065120517132"></a><a name="p2065120517132"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p45195649145658"><a name="p45195649145658"></a><a name="p45195649145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p42146344145658"><a name="p42146344145658"></a><a name="p42146344145658"></a>绑定的vNIC类型</p>
<p id="p43772780145658"><a name="p43772780145658"></a><a name="p43772780145658"></a>【使用说明】normal: 软交换</p>
</td>
</tr>
<tr id="row37613242198"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p20178562198"><a name="p20178562198"></a><a name="p20178562198"></a>port_security_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p1665125191310"><a name="p1665125191310"></a><a name="p1665125191310"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p532005162198"><a name="p532005162198"></a><a name="p532005162198"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p184376702198"><a name="p184376702198"></a><a name="p184376702198"></a>端口安全使能标记，如果不使能则安全组和dhcp防欺骗不生效</p>
</td>
</tr>
<tr id="row7819926185016"><td class="cellrowborder" valign="top" width="21.617838216178384%" headers="mcps1.2.5.1.1 "><p id="p2820202605014"><a name="p2820202605014"></a><a name="p2820202605014"></a>device_owner</p>
</td>
<td class="cellrowborder" valign="top" width="16.238376162383762%" headers="mcps1.2.5.1.2 "><p id="p1635527125116"><a name="p1635527125116"></a><a name="p1635527125116"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.617738226177384%" headers="mcps1.2.5.1.3 "><p id="p33612272511"><a name="p33612272511"></a><a name="p33612272511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.52604739526047%" headers="mcps1.2.5.1.4 "><p id="p10820526135010"><a name="p10820526135010"></a><a name="p10820526135010"></a>功能说明：端口设备所属取值范围：目前只支持指定""和"neutron:VIP_PORT"；neutron:VIP_PORT表示创建的是VIP</p>
</td>
</tr>
</tbody>
</table>

**表 3**  fixed\_ip对象

<a name="table335683819394"></a>
<table><thead align="left"><tr id="row12358183883913"><th class="cellrowborder" valign="top" width="19.970000000000002%" id="mcps1.2.5.1.1"><p id="p1435813382397"><a name="p1435813382397"></a><a name="p1435813382397"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="16.160000000000004%" id="mcps1.2.5.1.2"><p id="p95341852173912"><a name="p95341852173912"></a><a name="p95341852173912"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.39%" id="mcps1.2.5.1.3"><p id="p1835873833918"><a name="p1835873833918"></a><a name="p1835873833918"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.480000000000004%" id="mcps1.2.5.1.4"><p id="p43582038153914"><a name="p43582038153914"></a><a name="p43582038153914"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13582389394"><td class="cellrowborder" valign="top" width="19.970000000000002%" headers="mcps1.2.5.1.1 "><p id="p23591038103919"><a name="p23591038103919"></a><a name="p23591038103919"></a>subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.160000000000004%" headers="mcps1.2.5.1.2 "><p id="p0534125243910"><a name="p0534125243910"></a><a name="p0534125243910"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.5.1.3 "><p id="p8359173814394"><a name="p8359173814394"></a><a name="p8359173814394"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.480000000000004%" headers="mcps1.2.5.1.4 "><p id="p8359183883914"><a name="p8359183883914"></a><a name="p8359183883914"></a>所属子网ID</p>
<p id="p63591138193910"><a name="p63591138193910"></a><a name="p63591138193910"></a>【使用说明】不支持更新</p>
</td>
</tr>
<tr id="row113599384396"><td class="cellrowborder" valign="top" width="19.970000000000002%" headers="mcps1.2.5.1.1 "><p id="p935913810395"><a name="p935913810395"></a><a name="p935913810395"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="16.160000000000004%" headers="mcps1.2.5.1.2 "><p id="p1053455203914"><a name="p1053455203914"></a><a name="p1053455203914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.39%" headers="mcps1.2.5.1.3 "><p id="p6359238183912"><a name="p6359238183912"></a><a name="p6359238183912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.480000000000004%" headers="mcps1.2.5.1.4 "><p id="p17359183883918"><a name="p17359183883918"></a><a name="p17359183883918"></a>端口IP地址</p>
<p id="p163591338103915"><a name="p163591338103915"></a><a name="p163591338103915"></a>【使用说明】不支持更新</p>
</td>
</tr>
</tbody>
</table>

**表 4**  allow\_address\_pair对象

<a name="zh-cn_topic_0062207355_table57914257"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207355_row41852331"><th class="cellrowborder" valign="top" width="19.759999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0062207355_p34595685"><a name="zh-cn_topic_0062207355_p34595685"></a><a name="zh-cn_topic_0062207355_p34595685"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="14.879999999999999%" id="mcps1.2.5.1.2"><p id="p158591550182213"><a name="p158591550182213"></a><a name="p158591550182213"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.69%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0062207355_p50787128"><a name="zh-cn_topic_0062207355_p50787128"></a><a name="zh-cn_topic_0062207355_p50787128"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.67%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0062207355_p52626454"><a name="zh-cn_topic_0062207355_p52626454"></a><a name="zh-cn_topic_0062207355_p52626454"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207355_row34884411"><td class="cellrowborder" valign="top" width="19.759999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0062207355_p7065065"><a name="zh-cn_topic_0062207355_p7065065"></a><a name="zh-cn_topic_0062207355_p7065065"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="14.879999999999999%" headers="mcps1.2.5.1.2 "><p id="p108591150162214"><a name="p108591150162214"></a><a name="p108591150162214"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0062207355_p35399367"><a name="zh-cn_topic_0062207355_p35399367"></a><a name="zh-cn_topic_0062207355_p35399367"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.67%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0062207355_p64721603"><a name="zh-cn_topic_0062207355_p64721603"></a><a name="zh-cn_topic_0062207355_p64721603"></a>IP地址</p>
<p id="p9941154182714"><a name="p9941154182714"></a><a name="p9941154182714"></a>【使用说明】</p>
<a name="ul816613502913"></a><a name="ul816613502913"></a><ul id="ul816613502913"><li>不支持0.0.0.0</li><li>如果填写allowed_address_pairs参数，则ip_address是必选参数。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0062207355_row7958508"><td class="cellrowborder" valign="top" width="19.759999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0062207355_p40659381"><a name="zh-cn_topic_0062207355_p40659381"></a><a name="zh-cn_topic_0062207355_p40659381"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="14.879999999999999%" headers="mcps1.2.5.1.2 "><p id="p68591350122211"><a name="p68591350122211"></a><a name="p68591350122211"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0062207355_p5075526"><a name="zh-cn_topic_0062207355_p5075526"></a><a name="zh-cn_topic_0062207355_p5075526"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.67%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0062207355_p51982593"><a name="zh-cn_topic_0062207355_p51982593"></a><a name="zh-cn_topic_0062207355_p51982593"></a>MAC地址</p>
</td>
</tr>
</tbody>
</table>

**表 5**  extra\_dhcp\_opt对象

<a name="table5056075615524"></a>
<table><thead align="left"><tr id="row739480215524"><th class="cellrowborder" valign="top" width="19.88%" id="mcps1.2.5.1.1"><p id="p3368663215532"><a name="p3368663215532"></a><a name="p3368663215532"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="14.64%" id="mcps1.2.5.1.2"><p id="p578413122319"><a name="p578413122319"></a><a name="p578413122319"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.9%" id="mcps1.2.5.1.3"><p id="p4426268215532"><a name="p4426268215532"></a><a name="p4426268215532"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.58%" id="mcps1.2.5.1.4"><p id="p3407518415532"><a name="p3407518415532"></a><a name="p3407518415532"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2636755215524"><td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.5.1.1 "><p id="p2765891815532"><a name="p2765891815532"></a><a name="p2765891815532"></a>opt_name</p>
</td>
<td class="cellrowborder" valign="top" width="14.64%" headers="mcps1.2.5.1.2 "><p id="p878411362316"><a name="p878411362316"></a><a name="p878411362316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.9%" headers="mcps1.2.5.1.3 "><p id="p2577986315532"><a name="p2577986315532"></a><a name="p2577986315532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.58%" headers="mcps1.2.5.1.4 "><p id="p5884162715532"><a name="p5884162715532"></a><a name="p5884162715532"></a>Option名称</p>
</td>
</tr>
<tr id="row3942590315524"><td class="cellrowborder" valign="top" width="19.88%" headers="mcps1.2.5.1.1 "><p id="p1298235215532"><a name="p1298235215532"></a><a name="p1298235215532"></a>opt_value</p>
</td>
<td class="cellrowborder" valign="top" width="14.64%" headers="mcps1.2.5.1.2 "><p id="p1278420314232"><a name="p1278420314232"></a><a name="p1278420314232"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.9%" headers="mcps1.2.5.1.3 "><p id="p4493762615532"><a name="p4493762615532"></a><a name="p4493762615532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.58%" headers="mcps1.2.5.1.4 "><p id="p5057146315532"><a name="p5057146315532"></a><a name="p5057146315532"></a>Option值</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0062207340_section59483605"></a>

**表 6**  响应参数

<a name="zh-cn_topic_0062207340_table42633357"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207340_row53195707"><th class="cellrowborder" valign="top" width="15.559999999999999%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207340_p13884972"><a name="zh-cn_topic_0062207340_p13884972"></a><a name="zh-cn_topic_0062207340_p13884972"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.110000000000001%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207340_p50940942"><a name="zh-cn_topic_0062207340_p50940942"></a><a name="zh-cn_topic_0062207340_p50940942"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="73.33%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207340_p21379907"><a name="zh-cn_topic_0062207340_p21379907"></a><a name="zh-cn_topic_0062207340_p21379907"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207340_row54050919"><td class="cellrowborder" valign="top" width="15.559999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207340_p16048282"><a name="zh-cn_topic_0062207340_p16048282"></a><a name="zh-cn_topic_0062207340_p16048282"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207340_p24842503"><a name="zh-cn_topic_0062207340_p24842503"></a><a name="zh-cn_topic_0062207340_p24842503"></a><a href="#table923516594178">port</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="73.33%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207340_p51342761"><a name="zh-cn_topic_0062207340_p51342761"></a><a name="zh-cn_topic_0062207340_p51342761"></a>ports信息，参见<a href="#table923516594178">表7</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 7**  port对象

<a name="table923516594178"></a>
<table><thead align="left"><tr id="row323595915177"><th class="cellrowborder" valign="top" width="28.499999999999996%" id="mcps1.2.4.1.1"><p id="p823545971716"><a name="p823545971716"></a><a name="p823545971716"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="28.76%" id="mcps1.2.4.1.2"><p id="p12361759201719"><a name="p12361759201719"></a><a name="p12361759201719"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.74%" id="mcps1.2.4.1.3"><p id="p10236459121717"><a name="p10236459121717"></a><a name="p10236459121717"></a>说明</p>
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
<tr id="row14236145911171"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p172361159151713"><a name="p172361159151713"></a><a name="p172361159151713"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p16236165941716"><a name="p16236165941716"></a><a name="p16236165941716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p523605911719"><a name="p523605911719"></a><a name="p523605911719"></a>端口的名称</p>
</td>
</tr>
<tr id="row9236185901720"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p82367590175"><a name="p82367590175"></a><a name="p82367590175"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p17236159191713"><a name="p17236159191713"></a><a name="p17236159191713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p16236175961717"><a name="p16236175961717"></a><a name="p16236175961717"></a>所属网络的ID</p>
</td>
</tr>
<tr id="row2236115914175"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p17236155920178"><a name="p17236155920178"></a><a name="p17236155920178"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p223615598178"><a name="p223615598178"></a><a name="p223615598178"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p152361598171"><a name="p152361598171"></a><a name="p152361598171"></a>管理状态</p>
<p id="p2236259111714"><a name="p2236259111714"></a><a name="p2236259111714"></a>【使用说明】只支持true</p>
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
<tr id="row122362059111720"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p8236195911712"><a name="p8236195911712"></a><a name="p8236195911712"></a>fixed_ips</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p449815610539"><a name="p449815610539"></a><a name="p449815610539"></a>Array of <a href="#table1424105920176">fixed_ip</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p023685911174"><a name="p023685911174"></a><a name="p023685911174"></a>端口IP，参见<a href="#table1424105920176">表8</a>。例如："fixed_ips": [{"subnet_id": "4dc70db6-cb7f-4200-9790-a6a910776bba", "ip_address": "192.169.25.79"}]</p>
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
<tr id="row1323718599176"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p3237195910174"><a name="p3237195910174"></a><a name="p3237195910174"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p1623716594171"><a name="p1623716594171"></a><a name="p1623716594171"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p523717591175"><a name="p523717591175"></a><a name="p523717591175"></a>端口状态，可以为ACTIVE，BUILD，DOWN；</p>
<p id="p823735915171"><a name="p823735915171"></a><a name="p823735915171"></a>【使用说明】Hana硬直通虚拟机端口状态总为DOWN</p>
</td>
</tr>
<tr id="row823725971717"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p1523705981720"><a name="p1523705981720"></a><a name="p1523705981720"></a>security_groups</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p02377596178"><a name="p02377596178"></a><a name="p02377596178"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p162375598174"><a name="p162375598174"></a><a name="p162375598174"></a>扩展属性：安全组的UUID，例如："security_groups": ["a0608cbf-d047-4f54-8b28-cd7b59853fff"]</p>
<p id="p1723714597175"><a name="p1723714597175"></a><a name="p1723714597175"></a>【使用说明】不支持更新为空。</p>
</td>
</tr>
<tr id="row16237259141710"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p1823705901716"><a name="p1823705901716"></a><a name="p1823705901716"></a>allowed_address_pairs</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p5114142220534"><a name="p5114142220534"></a><a name="p5114142220534"></a>Array of <a href="#table13242185941715">allow_address_pair</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p52370591173"><a name="p52370591173"></a><a name="p52370591173"></a>扩展属性：IP/Mac对列表，allow_address_pair参见<a href="#table13242185941715">表9</a></p>
<p id="p1023712595179"><a name="p1023712595179"></a><a name="p1023712595179"></a>【使用说明】</p>
<a name="ul182371859131719"></a><a name="ul182371859131719"></a><ul id="ul182371859131719"><li>IP地址不允许为 “0.0.0.0”</li><li>如果allowed_address_pairs配置地址池较大的CIDR（掩码小于24位），建议为该port配置一个单独的安全组</li><li>如果allowed_address_pairs为“1.1.1.1/0”，表示关闭源目地址检查开关</li><li>硬件SDN环境不支持ip_address属性配置为CIDR格式</li><li>为虚拟IP配置后端ECS场景，allowed_address_pairs中配置的IP地址，必须为ECS网卡已有的IP地址，否则可能会导致虚拟IP通信异常</li><li>被绑定的云服务器网卡allowed_address_pairs填“1.1.1.1/0”</li></ul>
</td>
</tr>
<tr id="row9238165915173"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p9238459131711"><a name="p9238459131711"></a><a name="p9238459131711"></a>extra_dhcp_opts</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p1779121305411"><a name="p1779121305411"></a><a name="p1779121305411"></a>Array of <a href="#table1243759131714">extra_dhcp_opt</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p32381959151718"><a name="p32381959151718"></a><a name="p32381959151718"></a>扩展属性：DHCP的扩展Option，参见<a href="#table1243759131714">表10</a></p>
</td>
</tr>
<tr id="row923835951719"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p1123810593174"><a name="p1123810593174"></a><a name="p1123810593174"></a>binding:vif_details</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p14238159171719"><a name="p14238159171719"></a><a name="p14238159171719"></a><a href="#table72371439857">binding:vif_details</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p7238155916178"><a name="p7238155916178"></a><a name="p7238155916178"></a>vif的详细信息，参见<a href="#table72371439857">表11</a></p>
</td>
</tr>
<tr id="row1423875901713"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p182381859111716"><a name="p182381859111716"></a><a name="p182381859111716"></a>binding:profile</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p882857132610"><a name="p882857132610"></a><a name="p882857132610"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p12238759201715"><a name="p12238759201715"></a><a name="p12238759201715"></a>扩展属性：提供用户设置自定义信息</p>
<p id="p1423817599179"><a name="p1423817599179"></a><a name="p1423817599179"></a>【使用说明】</p>
<a name="ul1323895918178"></a><a name="ul1323895918178"></a><ul id="ul1323895918178"><li>internal_elb字段，布尔类型，普通租户可见。只有在创建内网ELB的虚拟IP的网卡时设置为true。普通租户没有权限更改该字段，由系统维护。<p id="p72380595178"><a name="p72380595178"></a><a name="p72380595178"></a>举例：</p>
<p id="p16238195914173"><a name="p16238195914173"></a><a name="p16238195914173"></a>{"internal_elb": true}</p>
</li><li>disable_security_groups字段，布尔类型，普通租户可见。默认为false高性能通信场景下，允许指定为true普通租户可见。仅支持创建port和读取时指定。当前仅支持指定为true，不支持指定为false<p id="p17238175951711"><a name="p17238175951711"></a><a name="p17238175951711"></a>举例：</p>
<p id="p523916592177"><a name="p523916592177"></a><a name="p523916592177"></a>{"disable_security_groups"：true }，</p>
<p id="p423995931715"><a name="p423995931715"></a><a name="p423995931715"></a>当前仅支持指定为true，不支持指定为false，指定为true时，FWaaS功能不生效。</p>
</li></ul>
<a name="ul88867533115"></a><a name="ul88867533115"></a><ul id="ul88867533115"><li>仅对于“华北-北京二”：udp_srvports和tcp_srvports，字段，字符串类型，默认不设置udp_srvports和tcp_srvports字段。允许指定udp_srvports和tcp_srvports字段为端口号，表示这些端口的tcp报文和udp报文可支持高并发连接，但是此类报文不受ACL和安全组规则的限制。udp_srvports和tcp_srvports字段同时支持更新操作。<a name="vpc_port02_0001_ul119701359152919_1"></a><a name="vpc_port02_0001_ul119701359152919_1"></a><ul id="vpc_port02_0001_ul119701359152919_1"><li>格式：<p id="vpc_port02_0001_p7108830192916_1"><a name="vpc_port02_0001_p7108830192916_1"></a><a name="vpc_port02_0001_p7108830192916_1"></a>{"tcp_srvports": "port1 port2 port3", "udp_srvports": "port1 port2 port3"}</p>
<p id="vpc_port02_0001_p47335481297_1"><a name="vpc_port02_0001_p47335481297_1"></a><a name="vpc_port02_0001_p47335481297_1"></a>端口号之间以空格间隔，最多允许指定的端口号总共为15个，端口号范围是1到65535。</p>
</li><li>示例：<p id="vpc_port02_0001_p10852165018293_1"><a name="vpc_port02_0001_p10852165018293_1"></a><a name="vpc_port02_0001_p10852165018293_1"></a>{"tcp_srvports": "80 443", "udp_srvports": "53"}</p>
<p id="vpc_port02_0001_p78371519293_1"><a name="vpc_port02_0001_p78371519293_1"></a><a name="vpc_port02_0001_p78371519293_1"></a>示例表示入方向目的端口为80或者443，出方向源端口为80或者443的tcp报文可支持高并发连接。入方向目的端口为53，出方向源端口为53的udp报文可支持高并发连接。但是此类报文不受ACL和安全组规则的限制。</p>
</li></ul>
</li></ul>
</td>
</tr>
<tr id="row1923995919171"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p82391459121715"><a name="p82391459121715"></a><a name="p82391459121715"></a>binding:vnic_type</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p224035916176"><a name="p224035916176"></a><a name="p224035916176"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p1524025912179"><a name="p1524025912179"></a><a name="p1524025912179"></a>绑定的vNIC类型</p>
<p id="p13240185916172"><a name="p13240185916172"></a><a name="p13240185916172"></a>normal: 软交换</p>
</td>
</tr>
<tr id="row172402595177"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p192405596173"><a name="p192405596173"></a><a name="p192405596173"></a>port_security_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p1224025916179"><a name="p1224025916179"></a><a name="p1224025916179"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p62406593179"><a name="p62406593179"></a><a name="p62406593179"></a>端口安全使能标记，如果不使能则安全组和dhcp防欺骗不生效</p>
</td>
</tr>
<tr id="row17240659151715"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p132407598171"><a name="p132407598171"></a><a name="p132407598171"></a>dns_assignment</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p1124016595177"><a name="p1124016595177"></a><a name="p1124016595177"></a>Array of <a href="#table1960316535179">dns_assignment</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p42401059101716"><a name="p42401059101716"></a><a name="p42401059101716"></a>扩展属性：主网卡默认内网域名信息</p>
<p id="p19240159101719"><a name="p19240159101719"></a><a name="p19240159101719"></a>【使用说明】不支持设置和更新，由系统自动维护</p>
<a name="ul124055910171"></a><a name="ul124055910171"></a><ul id="ul124055910171"><li>hostname：与端口dns_name一致</li><li>ip_address：端口ipv4私有地址</li><li>fqdn：为端口创建默认内网fqdn</li></ul>
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
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p13416184120236"><a name="p13416184120236"></a><a name="p13416184120236"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
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
<p id="p096314469434"><a name="p096314469434"></a><a name="p096314469434"></a>格式yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

**表 8**  fixed\_ip对象

<a name="table1424105920176"></a>
<table><thead align="left"><tr id="row82411959181716"><th class="cellrowborder" valign="top" width="25.95259525952595%" id="mcps1.2.4.1.1"><p id="p12241155901717"><a name="p12241155901717"></a><a name="p12241155901717"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="25.95259525952595%" id="mcps1.2.4.1.2"><p id="p19242135915171"><a name="p19242135915171"></a><a name="p19242135915171"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.09480948094809%" id="mcps1.2.4.1.3"><p id="p22425592175"><a name="p22425592175"></a><a name="p22425592175"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1824216590171"><td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.1 "><p id="p10242135912173"><a name="p10242135912173"></a><a name="p10242135912173"></a>subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.2 "><p id="p13242175917172"><a name="p13242175917172"></a><a name="p13242175917172"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.09480948094809%" headers="mcps1.2.4.1.3 "><p id="p16242165917172"><a name="p16242165917172"></a><a name="p16242165917172"></a>所属子网ID</p>
<p id="p18242559181712"><a name="p18242559181712"></a><a name="p18242559181712"></a>【使用说明】不支持更新</p>
</td>
</tr>
<tr id="row19242115921715"><td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.1 "><p id="p52421597171"><a name="p52421597171"></a><a name="p52421597171"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.2 "><p id="p19242159101715"><a name="p19242159101715"></a><a name="p19242159101715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.09480948094809%" headers="mcps1.2.4.1.3 "><p id="p1324225914173"><a name="p1324225914173"></a><a name="p1324225914173"></a>端口IP地址</p>
<p id="p142421597171"><a name="p142421597171"></a><a name="p142421597171"></a>【使用说明】不支持更新</p>
</td>
</tr>
</tbody>
</table>

**表 9**  allow\_address\_pair对象

<a name="table13242185941715"></a>
<table><thead align="left"><tr id="row1424216590179"><th class="cellrowborder" valign="top" width="25.89%" id="mcps1.2.4.1.1"><p id="p192423596172"><a name="p192423596172"></a><a name="p192423596172"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="26.07%" id="mcps1.2.4.1.2"><p id="p22424595171"><a name="p22424595171"></a><a name="p22424595171"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.04%" id="mcps1.2.4.1.3"><p id="p824225991716"><a name="p824225991716"></a><a name="p824225991716"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row132423598170"><td class="cellrowborder" valign="top" width="25.89%" headers="mcps1.2.4.1.1 "><p id="p424285961710"><a name="p424285961710"></a><a name="p424285961710"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="26.07%" headers="mcps1.2.4.1.2 "><p id="p12431859111711"><a name="p12431859111711"></a><a name="p12431859111711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.04%" headers="mcps1.2.4.1.3 "><p id="p4243135921717"><a name="p4243135921717"></a><a name="p4243135921717"></a>IP地址</p>
<p id="p424395914172"><a name="p424395914172"></a><a name="p424395914172"></a>【使用说明】不支持0.0.0.0</p>
</td>
</tr>
<tr id="row424375911712"><td class="cellrowborder" valign="top" width="25.89%" headers="mcps1.2.4.1.1 "><p id="p3243145918179"><a name="p3243145918179"></a><a name="p3243145918179"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="26.07%" headers="mcps1.2.4.1.2 "><p id="p14243175911711"><a name="p14243175911711"></a><a name="p14243175911711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.04%" headers="mcps1.2.4.1.3 "><p id="p16243659181717"><a name="p16243659181717"></a><a name="p16243659181717"></a>MAC地址</p>
</td>
</tr>
</tbody>
</table>

**表 10**  extra\_dhcp\_opt对象

<a name="table1243759131714"></a>
<table><thead align="left"><tr id="row172431659121719"><th class="cellrowborder" valign="top" width="25.892589258925895%" id="mcps1.2.4.1.1"><p id="p3243125918170"><a name="p3243125918170"></a><a name="p3243125918170"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="26.332633263326333%" id="mcps1.2.4.1.2"><p id="p624314592174"><a name="p624314592174"></a><a name="p624314592174"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="47.774777477747776%" id="mcps1.2.4.1.3"><p id="p3243359191710"><a name="p3243359191710"></a><a name="p3243359191710"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1224395911717"><td class="cellrowborder" valign="top" width="25.892589258925895%" headers="mcps1.2.4.1.1 "><p id="p15244259171718"><a name="p15244259171718"></a><a name="p15244259171718"></a>opt_name</p>
</td>
<td class="cellrowborder" valign="top" width="26.332633263326333%" headers="mcps1.2.4.1.2 "><p id="p14244145916177"><a name="p14244145916177"></a><a name="p14244145916177"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p182446594178"><a name="p182446594178"></a><a name="p182446594178"></a>Option名称</p>
</td>
</tr>
<tr id="row924445915176"><td class="cellrowborder" valign="top" width="25.892589258925895%" headers="mcps1.2.4.1.1 "><p id="p1244155931716"><a name="p1244155931716"></a><a name="p1244155931716"></a>opt_value</p>
</td>
<td class="cellrowborder" valign="top" width="26.332633263326333%" headers="mcps1.2.4.1.2 "><p id="p32441590178"><a name="p32441590178"></a><a name="p32441590178"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.774777477747776%" headers="mcps1.2.4.1.3 "><p id="p7244125921713"><a name="p7244125921713"></a><a name="p7244125921713"></a>Option值</p>
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
<table><thead align="left"><tr id="vpc_port01_0006_row860475311718"><th class="cellrowborder" valign="top" width="24.122412241224122%" id="mcps1.2.4.1.1"><p id="vpc_port01_0006_p85811122186"><a name="vpc_port01_0006_p85811122186"></a><a name="vpc_port01_0006_p85811122186"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.671967196719674%" id="mcps1.2.4.1.2"><p id="vpc_port01_0006_p145819129183"><a name="vpc_port01_0006_p145819129183"></a><a name="vpc_port01_0006_p145819129183"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.20562056205621%" id="mcps1.2.4.1.3"><p id="vpc_port01_0006_p95841215189"><a name="vpc_port01_0006_p95841215189"></a><a name="vpc_port01_0006_p95841215189"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_port01_0006_row126042530175"><td class="cellrowborder" valign="top" width="24.122412241224122%" headers="mcps1.2.4.1.1 "><p id="vpc_port01_0006_p5604753181710"><a name="vpc_port01_0006_p5604753181710"></a><a name="vpc_port01_0006_p5604753181710"></a>hostname</p>
</td>
<td class="cellrowborder" valign="top" width="19.671967196719674%" headers="mcps1.2.4.1.2 "><p id="vpc_port01_0006_p1160475381714"><a name="vpc_port01_0006_p1160475381714"></a><a name="vpc_port01_0006_p1160475381714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.20562056205621%" headers="mcps1.2.4.1.3 "><p id="vpc_port01_0006_p5604185321716"><a name="vpc_port01_0006_p5604185321716"></a><a name="vpc_port01_0006_p5604185321716"></a>端口hostname</p>
</td>
</tr>
<tr id="vpc_port01_0006_row12604185316171"><td class="cellrowborder" valign="top" width="24.122412241224122%" headers="mcps1.2.4.1.1 "><p id="vpc_port01_0006_p12604185301714"><a name="vpc_port01_0006_p12604185301714"></a><a name="vpc_port01_0006_p12604185301714"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="19.671967196719674%" headers="mcps1.2.4.1.2 "><p id="vpc_port01_0006_p12604125311719"><a name="vpc_port01_0006_p12604125311719"></a><a name="vpc_port01_0006_p12604125311719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.20562056205621%" headers="mcps1.2.4.1.3 "><p id="vpc_port01_0006_p1060417536175"><a name="vpc_port01_0006_p1060417536175"></a><a name="vpc_port01_0006_p1060417536175"></a>端口IP地址</p>
</td>
</tr>
<tr id="vpc_port01_0006_row1860435321719"><td class="cellrowborder" valign="top" width="24.122412241224122%" headers="mcps1.2.4.1.1 "><p id="vpc_port01_0006_p760425311178"><a name="vpc_port01_0006_p760425311178"></a><a name="vpc_port01_0006_p760425311178"></a>fqdn</p>
</td>
<td class="cellrowborder" valign="top" width="19.671967196719674%" headers="mcps1.2.4.1.2 "><p id="vpc_port01_0006_p1960465391715"><a name="vpc_port01_0006_p1960465391715"></a><a name="vpc_port01_0006_p1960465391715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.20562056205621%" headers="mcps1.2.4.1.3 "><p id="vpc_port01_0006_p1860485318172"><a name="vpc_port01_0006_p1860485318172"></a><a name="vpc_port01_0006_p1860485318172"></a>端口内网fqdn</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0062207340_section65590400"></a>

请求样例

```
POST https://{Endpoint}/v2.0/ports

{
    "port": {
       "admin_state_up": true,
        "network_id": "00ae08c5-f727-49ab-ad4b-b069398aa171",
        "name": "port-test"
    }
}
```

响应样例

```
{
    "port": {
        "id": "a7d98f3c-b42f-460b-96a1-07601e145961",
        "name": "port-test",
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
        "updated_at": "2018-09-20T01:45:26"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

