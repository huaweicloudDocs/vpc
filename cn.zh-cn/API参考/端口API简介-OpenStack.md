# 端口API简介<a name="ZH-CN_TOPIC_0062207805"></a>

## 对象简介<a name="zh-cn_topic_0062207355_section2160855"></a>

对端口资源进行管理和操作，包括查询端口列表、创建端口、查询指定端口、删除端口以及更新端口等接口。

## 对象模型<a name="zh-cn_topic_0062207355_section19447695"></a>

**表 1**  port对象

<a name="table15919752145624"></a>
<table><thead align="left"><tr id="row28529169145624"><th class="cellrowborder" valign="top" width="15.686274509803921%" id="mcps1.2.8.1.1"><p id="p42540009145658"><a name="p42540009145658"></a><a name="p42540009145658"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="7.8431372549019605%" id="mcps1.2.8.1.2"><p id="p19543620153319"><a name="p19543620153319"></a><a name="p19543620153319"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.686274509803921%" id="mcps1.2.8.1.3"><p id="p23188741145658"><a name="p23188741145658"></a><a name="p23188741145658"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.823529411764705%" id="mcps1.2.8.1.4"><p id="p66348700145658"><a name="p66348700145658"></a><a name="p66348700145658"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="13.725490196078432%" id="mcps1.2.8.1.5"><p id="p5535640145658"><a name="p5535640145658"></a><a name="p5535640145658"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="14.705882352941178%" id="mcps1.2.8.1.6"><p id="p45733729145658"><a name="p45733729145658"></a><a name="p45733729145658"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="23.52941176470588%" id="mcps1.2.8.1.7"><p id="p13444574145658"><a name="p13444574145658"></a><a name="p13444574145658"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13166425145624"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p28807446145658"><a name="p28807446145658"></a><a name="p28807446145658"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p75431220103312"><a name="p75431220103312"></a><a name="p75431220103312"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p51701793145658"><a name="p51701793145658"></a><a name="p51701793145658"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p27095680145658"><a name="p27095680145658"></a><a name="p27095680145658"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p47266460145658"><a name="p47266460145658"></a><a name="p47266460145658"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p3378012145658"><a name="p3378012145658"></a><a name="p3378012145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p5183528145658"><a name="p5183528145658"></a><a name="p5183528145658"></a>端口的ID，最大长度不超过255</p>
<p id="p189962619371"><a name="p189962619371"></a><a name="p189962619371"></a>【使用说明】在查询端口列表时非必选</p>
</td>
</tr>
<tr id="row1387566145624"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p20696121145658"><a name="p20696121145658"></a><a name="p20696121145658"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p154322073310"><a name="p154322073310"></a><a name="p154322073310"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p65773124145658"><a name="p65773124145658"></a><a name="p65773124145658"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p26022840145658"><a name="p26022840145658"></a><a name="p26022840145658"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p27475259145658"><a name="p27475259145658"></a><a name="p27475259145658"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p10903544145658"><a name="p10903544145658"></a><a name="p10903544145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p10771861145658"><a name="p10771861145658"></a><a name="p10771861145658"></a>端口的名称</p>
</td>
</tr>
<tr id="row36437767145624"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p949776145658"><a name="p949776145658"></a><a name="p949776145658"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p10543132010333"><a name="p10543132010333"></a><a name="p10543132010333"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p9822997145658"><a name="p9822997145658"></a><a name="p9822997145658"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p57465270145658"><a name="p57465270145658"></a><a name="p57465270145658"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p24175325145658"><a name="p24175325145658"></a><a name="p24175325145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p12044271145658"><a name="p12044271145658"></a><a name="p12044271145658"></a>存在的网络ID</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p36061910145658"><a name="p36061910145658"></a><a name="p36061910145658"></a>所属网络的ID</p>
</td>
</tr>
<tr id="row41410455145624"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p49567182145658"><a name="p49567182145658"></a><a name="p49567182145658"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p175433202335"><a name="p175433202335"></a><a name="p175433202335"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p55518807145658"><a name="p55518807145658"></a><a name="p55518807145658"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p729553145658"><a name="p729553145658"></a><a name="p729553145658"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p59093860145658"><a name="p59093860145658"></a><a name="p59093860145658"></a>true</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p21873335145658"><a name="p21873335145658"></a><a name="p21873335145658"></a>true或false</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p26909682145658"><a name="p26909682145658"></a><a name="p26909682145658"></a>管理状态</p>
<p id="p40860550145658"><a name="p40860550145658"></a><a name="p40860550145658"></a>【使用说明】只支持true</p>
</td>
</tr>
<tr id="row11261085145624"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p58114882145658"><a name="p58114882145658"></a><a name="p58114882145658"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p6543320173310"><a name="p6543320173310"></a><a name="p6543320173310"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p9685031145658"><a name="p9685031145658"></a><a name="p9685031145658"></a>String(32)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p46290069145658"><a name="p46290069145658"></a><a name="p46290069145658"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p58508083145658"><a name="p58508083145658"></a><a name="p58508083145658"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p41534249145658"><a name="p41534249145658"></a><a name="p41534249145658"></a>合法的mac地址，范围为fa:16:3e:xx:xx:xx</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p8831008145658"><a name="p8831008145658"></a><a name="p8831008145658"></a>端口MAC地址，例如："mac_address": "fa:16:3e:9e:ff:55"</p>
<p id="p12370211145658"><a name="p12370211145658"></a><a name="p12370211145658"></a>【使用说明】只支持系统动态分配，不支持指定</p>
</td>
</tr>
<tr id="row59425565145624"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p25296431145658"><a name="p25296431145658"></a><a name="p25296431145658"></a>fixed_ips</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p20543120103319"><a name="p20543120103319"></a><a name="p20543120103319"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p35745048145658"><a name="p35745048145658"></a><a name="p35745048145658"></a>List(fixed_ips)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p9667745145658"><a name="p9667745145658"></a><a name="p9667745145658"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p44889842145658"><a name="p44889842145658"></a><a name="p44889842145658"></a>从地址池自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p12198580145658"><a name="p12198580145658"></a><a name="p12198580145658"></a>一个端口只支持一个fixed_ip</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p48560910145658"><a name="p48560910145658"></a><a name="p48560910145658"></a>端口IP，参见“fixed_ips对象”表。例如："fixed_ips": [{"subnet_id": "4dc70db6-cb7f-4200-9790-a6a910776bba", "ip_address": "192.169.25.79"}]</p>
</td>
</tr>
<tr id="row52336547145624"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p42357933145658"><a name="p42357933145658"></a><a name="p42357933145658"></a>device_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p20544102014338"><a name="p20544102014338"></a><a name="p20544102014338"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p8440512145658"><a name="p8440512145658"></a><a name="p8440512145658"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p12592909145658"><a name="p12592909145658"></a><a name="p12592909145658"></a>CRUD</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p13392698145658"><a name="p13392698145658"></a><a name="p13392698145658"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p11066735145658"><a name="p11066735145658"></a><a name="p11066735145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p23990357145658"><a name="p23990357145658"></a><a name="p23990357145658"></a>设备ID</p>
<p id="p14586626145658"><a name="p14586626145658"></a><a name="p14586626145658"></a>【使用说明】不支持设置和更新，由系统自动维护，该字段非空的端口不允许删除</p>
</td>
</tr>
<tr id="row8304195145630"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p30450002145658"><a name="p30450002145658"></a><a name="p30450002145658"></a>device_owner</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p12544102013339"><a name="p12544102013339"></a><a name="p12544102013339"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p50531130145658"><a name="p50531130145658"></a><a name="p50531130145658"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p66489714145658"><a name="p66489714145658"></a><a name="p66489714145658"></a>CRD</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p16957730145658"><a name="p16957730145658"></a><a name="p16957730145658"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p31398899145658"><a name="p31398899145658"></a><a name="p31398899145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p60282892145658"><a name="p60282892145658"></a><a name="p60282892145658"></a>设备所属（DHCP/Router/ Nova等）</p>
<p id="p2837225125711"><a name="p2837225125711"></a><a name="p2837225125711"></a>【使用说明】不支持更新，只允许用户在创建虚拟IP端口时，为虚拟IP端口设置device_owner为neutron:VIP_PORT，当端口的该字段不为空时，仅支持该字段为neutron:VIP_PORT时的端口删除。</p>
<p id="p1458812975819"><a name="p1458812975819"></a><a name="p1458812975819"></a>该字段非空的端口不允许删除。</p>
</td>
</tr>
<tr id="row47218120145630"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p43524921145658"><a name="p43524921145658"></a><a name="p43524921145658"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p15544162010339"><a name="p15544162010339"></a><a name="p15544162010339"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p35857692145658"><a name="p35857692145658"></a><a name="p35857692145658"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p18791911145658"><a name="p18791911145658"></a><a name="p18791911145658"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p45749827145658"><a name="p45749827145658"></a><a name="p45749827145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p14748503145658"><a name="p14748503145658"></a><a name="p14748503145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p53778124145658"><a name="p53778124145658"></a><a name="p53778124145658"></a>项目ID。</p>
</td>
</tr>
<tr id="row925022145630"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p12676379145658"><a name="p12676379145658"></a><a name="p12676379145658"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p18544142093312"><a name="p18544142093312"></a><a name="p18544142093312"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p20153784145658"><a name="p20153784145658"></a><a name="p20153784145658"></a>String(16)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p21843826145658"><a name="p21843826145658"></a><a name="p21843826145658"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p24519472145658"><a name="p24519472145658"></a><a name="p24519472145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p39920219145658"><a name="p39920219145658"></a><a name="p39920219145658"></a>ACTIVE，BUILD，DOWN</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p12312282145658"><a name="p12312282145658"></a><a name="p12312282145658"></a>端口状态，可以为ACTIVE，BUILD，DOWN；</p>
<p id="p43701677145658"><a name="p43701677145658"></a><a name="p43701677145658"></a>【使用说明】Hana硬直通虚拟机端口状态总为DOWN</p>
</td>
</tr>
<tr id="row36940776145630"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p48921078145658"><a name="p48921078145658"></a><a name="p48921078145658"></a>security_groups</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p85444208332"><a name="p85444208332"></a><a name="p85444208332"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p3184354145658"><a name="p3184354145658"></a><a name="p3184354145658"></a>List(String)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p56606147145658"><a name="p56606147145658"></a><a name="p56606147145658"></a>CRUD</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p21695233145658"><a name="p21695233145658"></a><a name="p21695233145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p12483459145658"><a name="p12483459145658"></a><a name="p12483459145658"></a>SG 的uuid或者不设置</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p4527282145658"><a name="p4527282145658"></a><a name="p4527282145658"></a>扩展属性：安全组的UUID,例如："security_groups": ["a0608cbf-d047-4f54-8b28-cd7b59853fff"]</p>
<p id="p103001912487"><a name="p103001912487"></a><a name="p103001912487"></a>【使用说明】不支持更新为空。</p>
</td>
</tr>
<tr id="row17626705145630"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p41382197145658"><a name="p41382197145658"></a><a name="p41382197145658"></a>allowed_address_pairs</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p154410206339"><a name="p154410206339"></a><a name="p154410206339"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p63623641145658"><a name="p63623641145658"></a><a name="p63623641145658"></a>List(allow_address_pair)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p53241290145658"><a name="p53241290145658"></a><a name="p53241290145658"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p17577199145658"><a name="p17577199145658"></a><a name="p17577199145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p14466992145658"><a name="p14466992145658"></a><a name="p14466992145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p30975735145658"><a name="p30975735145658"></a><a name="p30975735145658"></a>扩展属性：IP/Mac对列表，allow_address_pair参见“allow_address_pair对象”表</p>
<p id="p7136530194312"><a name="p7136530194312"></a><a name="p7136530194312"></a>【使用说明】</p>
<a name="ul18386852174311"></a><a name="ul18386852174311"></a><ul id="ul18386852174311"><li>IP地址不允许为 “0.0.0.0”</li><li>如果allowed_address_pairs配置地址池较大的CIDR（掩码小于24位），建议为该port配置一个单独的安全组</li><li>硬件SDN环境不支持ip_address属性配置为CIDR格式</li><li>为虚拟IP配置后端ECS场景，allowed_address_pairs中配置的IP地址，必须为ECS网卡已有的IP地址，否则可能会导致虚拟IP通信异常。</li></ul>
</td>
</tr>
<tr id="row938573145630"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p34089655145658"><a name="p34089655145658"></a><a name="p34089655145658"></a>extra_dhcp_opts</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p1544120193314"><a name="p1544120193314"></a><a name="p1544120193314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p9798680145658"><a name="p9798680145658"></a><a name="p9798680145658"></a>List(extra_dhcp_opt)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p55495617145658"><a name="p55495617145658"></a><a name="p55495617145658"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p65960027145658"><a name="p65960027145658"></a><a name="p65960027145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p41161998145658"><a name="p41161998145658"></a><a name="p41161998145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p45787521145658"><a name="p45787521145658"></a><a name="p45787521145658"></a>扩展属性：DHCP的扩展Option</p>
</td>
</tr>
<tr id="row46629855145636"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p62371645145658"><a name="p62371645145658"></a><a name="p62371645145658"></a>binding:vif_details</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p854412014330"><a name="p854412014330"></a><a name="p854412014330"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p18938488145658"><a name="p18938488145658"></a><a name="p18938488145658"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p57622535145658"><a name="p57622535145658"></a><a name="p57622535145658"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p36913747145658"><a name="p36913747145658"></a><a name="p36913747145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p37223491145658"><a name="p37223491145658"></a><a name="p37223491145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p62312767145658"><a name="p62312767145658"></a><a name="p62312767145658"></a>vif的详细信息， "ovs_hybrid_plug": 是否为ovs/bridge混合模式</p>
</td>
</tr>
<tr id="row35771758145636"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p7522524145658"><a name="p7522524145658"></a><a name="p7522524145658"></a>binding:profile</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p1754412201333"><a name="p1754412201333"></a><a name="p1754412201333"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p5344685145658"><a name="p5344685145658"></a><a name="p5344685145658"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p30266372145658"><a name="p30266372145658"></a><a name="p30266372145658"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p35657030145658"><a name="p35657030145658"></a><a name="p35657030145658"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p2538333145658"><a name="p2538333145658"></a><a name="p2538333145658"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p4278449145658"><a name="p4278449145658"></a><a name="p4278449145658"></a>扩展属性：提供用户设置自定义信息</p>
<p id="p38506045145658"><a name="p38506045145658"></a><a name="p38506045145658"></a>【使用说明】</p>
<a name="ul11010089145658"></a><a name="ul11010089145658"></a><ul id="ul11010089145658"><li>internal_elb字段，布尔类型，普通租户可见。只有在创建内网ELB的虚拟IP的网卡时设置为true。普通租户没有权限更改该字段，由系统维护。<p id="p041674418210"><a name="p041674418210"></a><a name="p041674418210"></a>举例：</p>
<p id="p1774284092111"><a name="p1774284092111"></a><a name="p1774284092111"></a>{"internal_elb": true}</p>
</li><li>disable_security_groups字段，布尔类型，普通租户可见。默认为false高性能通信场景下，允许指定为true普通租户可见。仅支持创建port和读取时指定。当前仅支持指定为true，不支持指定为false<p id="p19402030145658"><a name="p19402030145658"></a><a name="p19402030145658"></a>举例：</p>
<p id="p40400544145658"><a name="p40400544145658"></a><a name="p40400544145658"></a>{"disable_security_groups"：true }，</p>
<p id="p28060583145658"><a name="p28060583145658"></a><a name="p28060583145658"></a>当前仅支持指定为true，不支持指定为false，指定为true时，FWaaS<span>功能不生效</span>。</p>
</li></ul>
<a name="ul51218659145658"></a><a name="ul51218659145658"></a><ul id="ul51218659145658"><li>仅对于消费者云：udp_srvports和tcp_srvports字段，字符串类型，默认不设置udp_srvports和tcp_srvports字段。允许指定udp_srvports和tcp_srvports字段为端口号，表示这些端口的tcp报文和udp报文可支持高并发连接，但是此类报文不受ACL和安全组规则的限制。udp_srvports和tcp_srvports字段同时支持更新操作。<a name="ul119701359152919"></a><a name="ul119701359152919"></a><ul id="ul119701359152919"><li>格式：<p id="p7108830192916"><a name="p7108830192916"></a><a name="p7108830192916"></a>{"tcp_srvports": "port1 port2 port3", "udp_srvports": "port1 port2 port3"}</p>
<p id="p47335481297"><a name="p47335481297"></a><a name="p47335481297"></a>端口号之间以空格间隔，最多允许指定的端口号总共为13个，端口号范围是1到65535。</p>
</li><li>示例：<p id="p10852165018293"><a name="p10852165018293"></a><a name="p10852165018293"></a>{"tcp_srvports": "80 443", "udp_srvports": "53"}</p>
<p id="p78371519293"><a name="p78371519293"></a><a name="p78371519293"></a>示例表示入方向目的端口为80或者443，出方向源端口为80或者443的tcp报文可支持高并发连接。入方向目的端口为53，出方向源端口为53的udp报文可支持高并发连接。但是此类报文不受ACL和安全组规则的限制。</p>
</li></ul>
</li></ul>
</td>
</tr>
<tr id="row63233200145636"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p4700493145658"><a name="p4700493145658"></a><a name="p4700493145658"></a>binding:vnic_type</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p95441420173311"><a name="p95441420173311"></a><a name="p95441420173311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p45195649145658"><a name="p45195649145658"></a><a name="p45195649145658"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p36968982145658"><a name="p36968982145658"></a><a name="p36968982145658"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p41697588145658"><a name="p41697588145658"></a><a name="p41697588145658"></a>normal</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p22061442145658"><a name="p22061442145658"></a><a name="p22061442145658"></a>normal</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p42146344145658"><a name="p42146344145658"></a><a name="p42146344145658"></a>绑定的vNIC类型</p>
<p id="p43772780145658"><a name="p43772780145658"></a><a name="p43772780145658"></a>normal: 软交换</p>
</td>
</tr>
<tr id="row37613242198"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p20178562198"><a name="p20178562198"></a><a name="p20178562198"></a>port_security_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p11544520173313"><a name="p11544520173313"></a><a name="p11544520173313"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p532005162198"><a name="p532005162198"></a><a name="p532005162198"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p314352982198"><a name="p314352982198"></a><a name="p314352982198"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p512735382198"><a name="p512735382198"></a><a name="p512735382198"></a>true</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p350334832198"><a name="p350334832198"></a><a name="p350334832198"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p184376702198"><a name="p184376702198"></a><a name="p184376702198"></a>端口安全使能标记，如果不使能则安全组和dhcp防欺骗不生效</p>
</td>
</tr>
<tr id="row167271926144411"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p117281926144417"><a name="p117281926144417"></a><a name="p117281926144417"></a>dns_assignment</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p954415204331"><a name="p954415204331"></a><a name="p954415204331"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p1272862616446"><a name="p1272862616446"></a><a name="p1272862616446"></a>List(Dict)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p107287268440"><a name="p107287268440"></a><a name="p107287268440"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p1572818263446"><a name="p1572818263446"></a><a name="p1572818263446"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p12729102614411"><a name="p12729102614411"></a><a name="p12729102614411"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p1472919269447"><a name="p1472919269447"></a><a name="p1472919269447"></a>扩展属性：主网卡默认内网域名信息</p>
<p id="p1834325274510"><a name="p1834325274510"></a><a name="p1834325274510"></a>【使用说明】不支持设置和更新，由系统自动维护</p>
<a name="ul1766216288464"></a><a name="ul1766216288464"></a><ul id="ul1766216288464"><li>hostname：与端口dns_name一致</li><li>ip_address：端口ipv4私有地址</li><li>fqdn：为端口创建默认内网fqdn</li></ul>
</td>
</tr>
<tr id="row119851851490"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p39859518498"><a name="p39859518498"></a><a name="p39859518498"></a>dns_name</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p95441920173311"><a name="p95441920173311"></a><a name="p95441920173311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p139852519498"><a name="p139852519498"></a><a name="p139852519498"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p1598585154910"><a name="p1598585154910"></a><a name="p1598585154910"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p69854584920"><a name="p69854584920"></a><a name="p69854584920"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p398512594918"><a name="p398512594918"></a><a name="p398512594918"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p098555164915"><a name="p098555164915"></a><a name="p098555164915"></a>扩展属性：主网卡默认内网DNS名称</p>
<p id="p11538191913508"><a name="p11538191913508"></a><a name="p11538191913508"></a>【使用说明】不支持设置和更新，由系统自动维护,访问该默认内网域名前，请确保子网使用当前系统提供的DNS</p>
</td>
</tr>
<tr id="row8784124710810"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p17700201411911"><a name="p17700201411911"></a><a name="p17700201411911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p759775317217"><a name="p759775317217"></a><a name="p759775317217"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p17000141292"><a name="p17000141292"></a><a name="p17000141292"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p1470010141396"><a name="p1470010141396"></a><a name="p1470010141396"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p870017141892"><a name="p870017141892"></a><a name="p870017141892"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p7700714691"><a name="p7700714691"></a><a name="p7700714691"></a>资源project_id</p>
</td>
</tr>
<tr id="row19797526919"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p6953241598"><a name="p6953241598"></a><a name="p6953241598"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p6953441993"><a name="p6953441993"></a><a name="p6953441993"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p11953164120911"><a name="p11953164120911"></a><a name="p11953164120911"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p595314119912"><a name="p595314119912"></a><a name="p595314119912"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间</p>
</td>
</tr>
<tr id="row124097610917"><td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.8431372549019605%" headers="mcps1.2.8.1.2 "><p id="p33972541493"><a name="p33972541493"></a><a name="p33972541493"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.686274509803921%" headers="mcps1.2.8.1.3 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="8.823529411764705%" headers="mcps1.2.8.1.4 "><p id="p339716540919"><a name="p339716540919"></a><a name="p339716540919"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.725490196078432%" headers="mcps1.2.8.1.5 "><p id="p1739717541895"><a name="p1739717541895"></a><a name="p1739717541895"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="14.705882352941178%" headers="mcps1.2.8.1.6 "><p id="p12397054697"><a name="p12397054697"></a><a name="p12397054697"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.52941176470588%" headers="mcps1.2.8.1.7 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间</p>
</td>
</tr>
</tbody>
</table>

**表 2**  fixed\_ip对象

<a name="table4290920914597"></a>
<table><thead align="left"><tr id="row3523499914597"><th class="cellrowborder" valign="top" width="18.4981501849815%" id="mcps1.2.7.1.1"><p id="p6174509115118"><a name="p6174509115118"></a><a name="p6174509115118"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="18.4981501849815%" id="mcps1.2.7.1.2"><p id="p3529643715118"><a name="p3529643715118"></a><a name="p3529643715118"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.28907109289071%" id="mcps1.2.7.1.3"><p id="p4043916415118"><a name="p4043916415118"></a><a name="p4043916415118"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="11.918808119188082%" id="mcps1.2.7.1.4"><p id="p5434688015118"><a name="p5434688015118"></a><a name="p5434688015118"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="7.519248075192481%" id="mcps1.2.7.1.5"><p id="p4002116015118"><a name="p4002116015118"></a><a name="p4002116015118"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="34.27657234276572%" id="mcps1.2.7.1.6"><p id="p2048854115118"><a name="p2048854115118"></a><a name="p2048854115118"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2319879914597"><td class="cellrowborder" valign="top" width="18.4981501849815%" headers="mcps1.2.7.1.1 "><p id="p626497215118"><a name="p626497215118"></a><a name="p626497215118"></a>subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.4981501849815%" headers="mcps1.2.7.1.2 "><p id="p3770069415118"><a name="p3770069415118"></a><a name="p3770069415118"></a>Uuid-Str</p>
</td>
<td class="cellrowborder" valign="top" width="9.28907109289071%" headers="mcps1.2.7.1.3 "><p id="p3385735615118"><a name="p3385735615118"></a><a name="p3385735615118"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.918808119188082%" headers="mcps1.2.7.1.4 "><p id="p5809135215118"><a name="p5809135215118"></a><a name="p5809135215118"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.7.1.5 "><p id="p777903915118"><a name="p777903915118"></a><a name="p777903915118"></a>存在的子网id</p>
</td>
<td class="cellrowborder" valign="top" width="34.27657234276572%" headers="mcps1.2.7.1.6 "><p id="p2612244315118"><a name="p2612244315118"></a><a name="p2612244315118"></a>所属子网ID</p>
<p id="p3377540315118"><a name="p3377540315118"></a><a name="p3377540315118"></a>【使用说明】不支持更新</p>
</td>
</tr>
<tr id="row636738414597"><td class="cellrowborder" valign="top" width="18.4981501849815%" headers="mcps1.2.7.1.1 "><p id="p6042468915118"><a name="p6042468915118"></a><a name="p6042468915118"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="18.4981501849815%" headers="mcps1.2.7.1.2 "><p id="p6256165915118"><a name="p6256165915118"></a><a name="p6256165915118"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.28907109289071%" headers="mcps1.2.7.1.3 "><p id="p3432960915118"><a name="p3432960915118"></a><a name="p3432960915118"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.918808119188082%" headers="mcps1.2.7.1.4 "><p id="p2923494815118"><a name="p2923494815118"></a><a name="p2923494815118"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.7.1.5 "><p id="p1922056315118"><a name="p1922056315118"></a><a name="p1922056315118"></a>合法的IP地址</p>
</td>
<td class="cellrowborder" valign="top" width="34.27657234276572%" headers="mcps1.2.7.1.6 "><p id="p1336175915118"><a name="p1336175915118"></a><a name="p1336175915118"></a>端口IP地址</p>
<p id="p5314696715118"><a name="p5314696715118"></a><a name="p5314696715118"></a>【使用说明】不支持更新</p>
</td>
</tr>
</tbody>
</table>

**表 3**  allow\_address\_pair对象

<a name="zh-cn_topic_0062207355_table57914257"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207355_row41852331"><th class="firstcol" valign="top" width="17.53%" id="mcps1.2.7.1.1"><p id="zh-cn_topic_0062207355_p34595685"><a name="zh-cn_topic_0062207355_p34595685"></a><a name="zh-cn_topic_0062207355_p34595685"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="12.370000000000001%" id="mcps1.2.7.1.2"><p id="zh-cn_topic_0062207355_p50787128"><a name="zh-cn_topic_0062207355_p50787128"></a><a name="zh-cn_topic_0062207355_p50787128"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.31%" id="mcps1.2.7.1.3"><p id="zh-cn_topic_0062207355_p20116683"><a name="zh-cn_topic_0062207355_p20116683"></a><a name="zh-cn_topic_0062207355_p20116683"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="10.31%" id="mcps1.2.7.1.4"><p id="zh-cn_topic_0062207355_p18838598"><a name="zh-cn_topic_0062207355_p18838598"></a><a name="zh-cn_topic_0062207355_p18838598"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="16.49%" id="mcps1.2.7.1.5"><p id="zh-cn_topic_0062207355_p49531474"><a name="zh-cn_topic_0062207355_p49531474"></a><a name="zh-cn_topic_0062207355_p49531474"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="32.99%" id="mcps1.2.7.1.6"><p id="zh-cn_topic_0062207355_p52626454"><a name="zh-cn_topic_0062207355_p52626454"></a><a name="zh-cn_topic_0062207355_p52626454"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207355_row34884411"><th class="firstcol" valign="top" width="17.53%" id="mcps1.2.8.1.1" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0062207355_p7065065"><a name="zh-cn_topic_0062207355_p7065065"></a><a name="zh-cn_topic_0062207355_p7065065"></a>ip_address</p>
</th>
<td class="cellrowborder" valign="top" width="12.370000000000001%" headers="mcps1.2.8.1.1 mcps1.2.7.1.2 "><p id="zh-cn_topic_0062207355_p35399367"><a name="zh-cn_topic_0062207355_p35399367"></a><a name="zh-cn_topic_0062207355_p35399367"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.8.1.1 mcps1.2.7.1.3 "><p id="zh-cn_topic_0062207355_p48776445"><a name="zh-cn_topic_0062207355_p48776445"></a><a name="zh-cn_topic_0062207355_p48776445"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.8.1.1 mcps1.2.7.1.4 "><p id="zh-cn_topic_0062207355_p58577972"><a name="zh-cn_topic_0062207355_p58577972"></a><a name="zh-cn_topic_0062207355_p58577972"></a>None</p>
</td>
<td class="cellrowborder" valign="top" width="16.49%" headers="mcps1.2.8.1.1 mcps1.2.7.1.5 "><p id="zh-cn_topic_0062207355_p47195283"><a name="zh-cn_topic_0062207355_p47195283"></a><a name="zh-cn_topic_0062207355_p47195283"></a>不能为空</p>
</td>
<td class="cellrowborder" valign="top" width="32.99%" headers="mcps1.2.8.1.1 mcps1.2.7.1.6 "><p id="zh-cn_topic_0062207355_p64721603"><a name="zh-cn_topic_0062207355_p64721603"></a><a name="zh-cn_topic_0062207355_p64721603"></a>IP地址</p>
<p id="zh-cn_topic_0062207355_p45623521"><a name="zh-cn_topic_0062207355_p45623521"></a><a name="zh-cn_topic_0062207355_p45623521"></a>【使用说明】不支持0.0.0.0</p>
</td>
</tr>
<tr id="zh-cn_topic_0062207355_row7958508"><th class="firstcol" valign="top" width="17.53%" id="mcps1.2.8.2.1" headers="mcps1.2.7.1.1 "><p id="zh-cn_topic_0062207355_p40659381"><a name="zh-cn_topic_0062207355_p40659381"></a><a name="zh-cn_topic_0062207355_p40659381"></a>mac_address</p>
</th>
<td class="cellrowborder" valign="top" width="12.370000000000001%" headers="mcps1.2.8.2.1 mcps1.2.7.1.2 "><p id="zh-cn_topic_0062207355_p5075526"><a name="zh-cn_topic_0062207355_p5075526"></a><a name="zh-cn_topic_0062207355_p5075526"></a>String(32)</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.8.2.1 mcps1.2.7.1.3 "><p id="zh-cn_topic_0062207355_p8464456"><a name="zh-cn_topic_0062207355_p8464456"></a><a name="zh-cn_topic_0062207355_p8464456"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.8.2.1 mcps1.2.7.1.4 "><p id="zh-cn_topic_0062207355_p14532322"><a name="zh-cn_topic_0062207355_p14532322"></a><a name="zh-cn_topic_0062207355_p14532322"></a>None</p>
</td>
<td class="cellrowborder" valign="top" width="16.49%" headers="mcps1.2.8.2.1 mcps1.2.7.1.5 "><p id="zh-cn_topic_0062207355_p36267453"><a name="zh-cn_topic_0062207355_p36267453"></a><a name="zh-cn_topic_0062207355_p36267453"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="32.99%" headers="mcps1.2.8.2.1 mcps1.2.7.1.6 "><p id="zh-cn_topic_0062207355_p51982593"><a name="zh-cn_topic_0062207355_p51982593"></a><a name="zh-cn_topic_0062207355_p51982593"></a>MAC地址</p>
</td>
</tr>
</tbody>
</table>

**表 4**  extra\_dhcp\_opt对象

<a name="table5056075615524"></a>
<table><thead align="left"><tr id="row739480215524"><th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.1"><p id="p3368663215532"><a name="p3368663215532"></a><a name="p3368663215532"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.2"><p id="p4426268215532"><a name="p4426268215532"></a><a name="p4426268215532"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.3"><p id="p2850751315532"><a name="p2850751315532"></a><a name="p2850751315532"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.4"><p id="p2740721215532"><a name="p2740721215532"></a><a name="p2740721215532"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.5"><p id="p539170815532"><a name="p539170815532"></a><a name="p539170815532"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="16.666666666666664%" id="mcps1.2.7.1.6"><p id="p3407518415532"><a name="p3407518415532"></a><a name="p3407518415532"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2636755215524"><td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.1 "><p id="p2765891815532"><a name="p2765891815532"></a><a name="p2765891815532"></a>opt_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.2 "><p id="p2577986315532"><a name="p2577986315532"></a><a name="p2577986315532"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.3 "><p id="p779419015532"><a name="p779419015532"></a><a name="p779419015532"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.4 "><p id="p2734961615532"><a name="p2734961615532"></a><a name="p2734961615532"></a>None</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.5 "><p id="p72643915532"><a name="p72643915532"></a><a name="p72643915532"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.6 "><p id="p5884162715532"><a name="p5884162715532"></a><a name="p5884162715532"></a>Option名称</p>
</td>
</tr>
<tr id="row3942590315524"><td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.1 "><p id="p1298235215532"><a name="p1298235215532"></a><a name="p1298235215532"></a>opt_value</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.2 "><p id="p4493762615532"><a name="p4493762615532"></a><a name="p4493762615532"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.3 "><p id="p1606911715532"><a name="p1606911715532"></a><a name="p1606911715532"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.4 "><p id="p2653008015532"><a name="p2653008015532"></a><a name="p2653008015532"></a>None</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.5 "><p id="p145284315532"><a name="p145284315532"></a><a name="p145284315532"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="16.666666666666664%" headers="mcps1.2.7.1.6 "><p id="p5057146315532"><a name="p5057146315532"></a><a name="p5057146315532"></a>Option值</p>
</td>
</tr>
</tbody>
</table>

