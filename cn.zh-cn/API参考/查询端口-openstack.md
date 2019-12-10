# 查询端口<a name="ZH-CN_TOPIC_0201534191"></a>

## 功能介绍<a name="zh-cn_topic_0062207351_section48492792"></a>

查询端口详情。

## URI<a name="zh-cn_topic_0062207351_section33781949"></a>

GET /v2.0/ports/\{port\_id\}

## 请求消息<a name="zh-cn_topic_0062207351_section65197270"></a>

无

## 响应消息<a name="zh-cn_topic_0062207351_section49904522"></a>

**表 1**  响应参数

<a name="zh-cn_topic_0062207351_table21718662"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207351_row2001795"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207351_p27927672"><a name="zh-cn_topic_0062207351_p27927672"></a><a name="zh-cn_topic_0062207351_p27927672"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207351_p47548937"><a name="zh-cn_topic_0062207351_p47548937"></a><a name="zh-cn_topic_0062207351_p47548937"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207351_p46581538"><a name="zh-cn_topic_0062207351_p46581538"></a><a name="zh-cn_topic_0062207351_p46581538"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207351_row15008249"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207351_p7708685"><a name="zh-cn_topic_0062207351_p7708685"></a><a name="zh-cn_topic_0062207351_p7708685"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207351_p20423749"><a name="zh-cn_topic_0062207351_p20423749"></a><a name="zh-cn_topic_0062207351_p20423749"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207351_p50928963"><a name="zh-cn_topic_0062207351_p50928963"></a><a name="zh-cn_topic_0062207351_p50928963"></a>port对象列表，参见<a href="#table15919752145624">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  port对象

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
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p1059419436401"><a name="p1059419436401"></a><a name="p1059419436401"></a>Array of <a href="#table4290920914597">fixed_ip</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p48560910145658"><a name="p48560910145658"></a><a name="p48560910145658"></a>端口IP，参见<a href="#table4290920914597">表3</a>。例如："fixed_ips": [{"subnet_id": "4dc70db6-cb7f-4200-9790-a6a910776bba", "ip_address": "192.169.25.79"}]</p>
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
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p4527282145658"><a name="p4527282145658"></a><a name="p4527282145658"></a>扩展属性：安全组的UUID,例如："security_groups": ["a0608cbf-d047-4f54-8b28-cd7b59853fff"]</p>
<p id="p103001912487"><a name="p103001912487"></a><a name="p103001912487"></a>【使用说明】不支持更新为空。</p>
</td>
</tr>
<tr id="row17626705145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p41382197145658"><a name="p41382197145658"></a><a name="p41382197145658"></a>allowed_address_pairs</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p94821354415"><a name="p94821354415"></a><a name="p94821354415"></a>Array of <a href="#zh-cn_topic_0062207355_table57914257">allow_address_pair</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p30975735145658"><a name="p30975735145658"></a><a name="p30975735145658"></a>扩展属性：IP/Mac对列表，allow_address_pair参见<a href="#zh-cn_topic_0062207355_table57914257">allow_address_pair</a></p>
<p id="p7136530194312"><a name="p7136530194312"></a><a name="p7136530194312"></a>【使用说明】</p>
<a name="ul18386852174311"></a><a name="ul18386852174311"></a><ul id="ul18386852174311"><li>IP地址不允许为 “0.0.0.0”</li><li>如果allowed_address_pairs配置地址池较大的CIDR（掩码小于24位），建议为该port配置一个单独的安全组</li><li>硬件SDN环境不支持ip_address属性配置为CIDR格式</li><li>为虚拟IP配置后端ECS场景，allowed_address_pairs中配置的IP地址，必须为ECS网卡已有的IP地址，否则可能会导致虚拟IP通信异常。</li></ul>
</td>
</tr>
<tr id="row938573145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p34089655145658"><a name="p34089655145658"></a><a name="p34089655145658"></a>extra_dhcp_opts</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p9798680145658"><a name="p9798680145658"></a><a name="p9798680145658"></a>Array of <a href="#table5056075615524">extra_dhcp_opt</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p45787521145658"><a name="p45787521145658"></a><a name="p45787521145658"></a>扩展属性：DHCP的扩展Option，参见<a href="#table5056075615524">表5</a></p>
</td>
</tr>
<tr id="row46629855145636"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p62371645145658"><a name="p62371645145658"></a><a name="p62371645145658"></a>binding:vif_details</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p18938488145658"><a name="p18938488145658"></a><a name="p18938488145658"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p62312767145658"><a name="p62312767145658"></a><a name="p62312767145658"></a>vif的详细信息， "ovs_hybrid_plug": 是否为ovs/bridge混合模式</p>
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
<p id="p28060583145658"><a name="p28060583145658"></a><a name="p28060583145658"></a>当前仅支持指定为true，不支持指定为false，指定为true时，FWaaS<span>功能不生效</span>。</p>
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
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p1272862616446"><a name="p1272862616446"></a><a name="p1272862616446"></a>String</p>
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
<p id="p11538191913508"><a name="p11538191913508"></a><a name="p11538191913508"></a>【使用说明】不支持设置和更新，由系统自动维护,访问该默认内网域名前，请确保子网使用当前系统提供的DNS</p>
</td>
</tr>
<tr id="row8784124710810"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.76%" headers="mcps1.2.4.1.2 "><p id="p759775317217"><a name="p759775317217"></a><a name="p759775317217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.74%" headers="mcps1.2.4.1.3 "><p id="p363353052314"><a name="p363353052314"></a><a name="p363353052314"></a>项目ID</p>
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
<p id="p1242622584318"><a name="p1242622584318"></a><a name="p1242622584318"></a>格式yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

**表 3**  fixed\_ip对象

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

**表 4**  allow\_address\_pair对象

<a name="zh-cn_topic_0062207355_table57914257"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207355_row41852331"><th class="cellrowborder" valign="top" width="27.87%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207355_p34595685"><a name="zh-cn_topic_0062207355_p34595685"></a><a name="zh-cn_topic_0062207355_p34595685"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="19.67%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207355_p50787128"><a name="zh-cn_topic_0062207355_p50787128"></a><a name="zh-cn_topic_0062207355_p50787128"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="52.459999999999994%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207355_p52626454"><a name="zh-cn_topic_0062207355_p52626454"></a><a name="zh-cn_topic_0062207355_p52626454"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207355_row34884411"><td class="cellrowborder" valign="top" width="27.87%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207355_p7065065"><a name="zh-cn_topic_0062207355_p7065065"></a><a name="zh-cn_topic_0062207355_p7065065"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207355_p35399367"><a name="zh-cn_topic_0062207355_p35399367"></a><a name="zh-cn_topic_0062207355_p35399367"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.459999999999994%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207355_p64721603"><a name="zh-cn_topic_0062207355_p64721603"></a><a name="zh-cn_topic_0062207355_p64721603"></a>IP地址</p>
<p id="zh-cn_topic_0062207355_p45623521"><a name="zh-cn_topic_0062207355_p45623521"></a><a name="zh-cn_topic_0062207355_p45623521"></a>【使用说明】不支持0.0.0.0</p>
</td>
</tr>
<tr id="zh-cn_topic_0062207355_row7958508"><td class="cellrowborder" valign="top" width="27.87%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207355_p40659381"><a name="zh-cn_topic_0062207355_p40659381"></a><a name="zh-cn_topic_0062207355_p40659381"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207355_p5075526"><a name="zh-cn_topic_0062207355_p5075526"></a><a name="zh-cn_topic_0062207355_p5075526"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.459999999999994%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207355_p51982593"><a name="zh-cn_topic_0062207355_p51982593"></a><a name="zh-cn_topic_0062207355_p51982593"></a>MAC地址</p>
</td>
</tr>
</tbody>
</table>

**表 5**  extra\_dhcp\_opt对象

<a name="table5056075615524"></a>
<table><thead align="left"><tr id="row739480215524"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p3368663215532"><a name="p3368663215532"></a><a name="p3368663215532"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p4426268215532"><a name="p4426268215532"></a><a name="p4426268215532"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p3407518415532"><a name="p3407518415532"></a><a name="p3407518415532"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2636755215524"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p2765891815532"><a name="p2765891815532"></a><a name="p2765891815532"></a>opt_name</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p2577986315532"><a name="p2577986315532"></a><a name="p2577986315532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p5884162715532"><a name="p5884162715532"></a><a name="p5884162715532"></a>Option名称</p>
</td>
</tr>
<tr id="row3942590315524"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1298235215532"><a name="p1298235215532"></a><a name="p1298235215532"></a>opt_value</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p4493762615532"><a name="p4493762615532"></a><a name="p4493762615532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p5057146315532"><a name="p5057146315532"></a><a name="p5057146315532"></a>Option值</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0062207351_section46487516"></a>

请求样例

```
GET https://{Endpoint}/v2.0/ports/791870bd-36a7-4d9b-b015-a78e9b06af08
```

响应样例

```
{
    "port": {
        "id": "791870bd-36a7-4d9b-b015-a78e9b06af08",
        "name": "port-test",
        "status": "DOWN",
        "admin_state_up": true,
        "fixed_ips": [],
        "mac_address": "fa:16:3e:01:e0:b2",
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
        "created_at": "2018-09-13T01:43:41",
        "updated_at": "2018-09-13T01:43:41"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

