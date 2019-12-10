# 查询弹性公网IP<a name="zh-cn_topic_0020090597"></a>

## 功能介绍<a name="section40040492"></a>

查询指定弹性公网IP。

## URI<a name="section24820109"></a>

GET /v1/\{project\_id\}/publicips/\{publicip\_id\}

参数说明请参见[表1](#table57982344)。

**表 1**  参数说明

<a name="table57982344"></a>
<table><thead align="left"><tr id="row19130757"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p6087504"><a name="p6087504"></a><a name="p6087504"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p23325828"><a name="p23325828"></a><a name="p23325828"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p10343879"><a name="p10343879"></a><a name="p10343879"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row32547908"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p19134881"><a name="p19134881"></a><a name="p19134881"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p6421510"><a name="p6421510"></a><a name="p6421510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row50769665"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p18702178"><a name="p18702178"></a><a name="p18702178"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p38481481"><a name="p38481481"></a><a name="p38481481"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p29992219"><a name="p29992219"></a><a name="p29992219"></a>弹性公网IP唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section22054394"></a>

-   请求参数

    无

-   请求样例

    无


## 响应消息<a name="section64271818"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table64961662152123"></a>
    <table><thead align="left"><tr id="row7248731152123"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p50276345152123"><a name="p50276345152123"></a><a name="p50276345152123"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="p23039456152123"><a name="p23039456152123"></a><a name="p23039456152123"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="p54256632152123"><a name="p54256632152123"></a><a name="p54256632152123"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row32711048152123"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p32349241152123"><a name="p32349241152123"></a><a name="p32349241152123"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p45145628152123"><a name="p45145628152123"></a><a name="p45145628152123"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p27820057152123"><a name="p27820057152123"></a><a name="p27820057152123"></a>弹性公网IP对象，请参见<a href="#table3035698">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicip字段说明

    <a name="table3035698"></a>
    <table><thead align="left"><tr id="row64466590"><th class="cellrowborder" valign="top" width="36.046395360463954%" id="mcps1.2.4.1.1"><p id="p54411269"><a name="p54411269"></a><a name="p54411269"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.90720927907209%" id="mcps1.2.4.1.2"><p id="p3124580518523"><a name="p3124580518523"></a><a name="p3124580518523"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="36.046395360463954%" id="mcps1.2.4.1.3"><p id="p40293226"><a name="p40293226"></a><a name="p40293226"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row42525879"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p22044193"><a name="p22044193"></a><a name="p22044193"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p4788225318523"><a name="p4788225318523"></a><a name="p4788225318523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p44048571"><a name="p44048571"></a><a name="p44048571"></a>弹性公网IP唯一标识</p>
    </td>
    </tr>
    <tr id="row60892825"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p33371781"><a name="p33371781"></a><a name="p33371781"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p5325729418523"><a name="p5325729418523"></a><a name="p5325729418523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul1945793192"></a><a name="ul1945793192"></a><ul id="ul1945793192"><li>功能说明：弹性公网IP的状态</li><li>取值范围：<a name="ul4678228115815"></a><a name="ul4678228115815"></a><ul id="ul4678228115815"><li>FREEZED：冻结</li><li>BIND_ERROR：绑定失败</li><li>BINDING：绑定中</li><li>PENDING_DELETE：释放中</li><li>PENDING_CREATE：创建中</li><li>PENDING_UPDATE：更新中</li><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ELB：绑定ELB</li><li>ERROR：异常失败</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row17803202152320"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p09743162419"><a name="p09743162419"></a><a name="p09743162419"></a>profile</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p12971231132410"><a name="p12971231132410"></a><a name="p12971231132410"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p169773114242"><a name="p169773114242"></a><a name="p169773114242"></a>功能说明：额外参数，包括订单id、产品id等信息，详情请参见<a href="#table66651219193417">表4</a>。</p>
    <p id="p156320510335"><a name="p156320510335"></a><a name="p156320510335"></a>约束：如果profile不为空，说明是包周期的弹性公网IP</p>
    </td>
    </tr>
    <tr id="row1722212174296"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p15848707"><a name="p15848707"></a><a name="p15848707"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p3408038918330"><a name="p3408038918330"></a><a name="p3408038918330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul7176216121014"></a><a name="ul7176216121014"></a><ul id="ul7176216121014"><li>功能说明：弹性公网IP的类型</li><li>取值范围：<em id="i16850184017499"><a name="i16850184017499"></a><a name="i16850184017499"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="ul585004064911"></a><a name="ul585004064911"></a><ul id="ul585004064911"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li></ul>
    </li><li>约束：<a name="ul9738153015499"></a><a name="ul9738153015499"></a><ul id="ul9738153015499"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"publicip_type"字段未给定时，默认为5_bgp。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row16458145723915"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p175119718406"><a name="p175119718406"></a><a name="p175119718406"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p6512979403"><a name="p6512979403"></a><a name="p6512979403"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p115126714020"><a name="p115126714020"></a><a name="p115126714020"></a>IPv4时无此字段，IPv6时为申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="row180110932914"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p171101456172118"><a name="p171101456172118"></a><a name="p171101456172118"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p1811012569218"><a name="p1811012569218"></a><a name="p1811012569218"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p1211011564217"><a name="p1211011564217"></a><a name="p1211011564217"></a>IP版本信息，取值范围是4和6</p>
    <a name="ul13987110227"></a><a name="ul13987110227"></a><ul id="ul13987110227"><li>4：表示IPv4</li><li>6：表示IPv6</li></ul>
    </td>
    </tr>
    <tr id="row66070243"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p50089467"><a name="p50089467"></a><a name="p50089467"></a>private_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p1357258018523"><a name="p1357258018523"></a><a name="p1357258018523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul1693412582014"></a><a name="ul1693412582014"></a><ul id="ul1693412582014"><li>功能说明：绑定弹性公网IP的私有IP地址</li><li>约束：只有绑定了的弹性公网IP查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="row12246230153229"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p11971849153234"><a name="p11971849153234"></a><a name="p11971849153234"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p2563717518523"><a name="p2563717518523"></a><a name="p2563717518523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul420471472010"></a><a name="ul420471472010"></a><ul id="ul420471472010"><li>功能说明：端口id。</li><li>约束：只有绑定了的弹性公网IP查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="row7204713"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p46710863"><a name="p46710863"></a><a name="p46710863"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p6334526618523"><a name="p6334526618523"></a><a name="p6334526618523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p25354291121"><a name="p25354291121"></a><a name="p25354291121"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row55494360"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p65858198"><a name="p65858198"></a><a name="p65858198"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p3069292618523"><a name="p3069292618523"></a><a name="p3069292618523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p36292894"><a name="p36292894"></a><a name="p36292894"></a>弹性公网IP申请时间（UTC）</p>
    </td>
    </tr>
    <tr id="row58200593"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p16627584"><a name="p16627584"></a><a name="p16627584"></a>bandwidth_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p309907418523"><a name="p309907418523"></a><a name="p309907418523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p3934181618641"><a name="p3934181618641"></a><a name="p3934181618641"></a>弹性公网IP对应带宽ID</p>
    </td>
    </tr>
    <tr id="row51415138"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p3876622"><a name="p3876622"></a><a name="p3876622"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p4969847118523"><a name="p4969847118523"></a><a name="p4969847118523"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p2365466"><a name="p2365466"></a><a name="p2365466"></a>带宽大小，单位为Mbit/s。</p>
    </td>
    </tr>
    <tr id="row21289199"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p46703582"><a name="p46703582"></a><a name="p46703582"></a>bandwidth_share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p6615323718523"><a name="p6615323718523"></a><a name="p6615323718523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul2255712095"></a><a name="ul2255712095"></a><ul id="ul2255712095"><li>功能说明：弹性公网IP的带宽类型</li><li>取值范围：PER，WHOLE。<a name="ul729412507220"></a><a name="ul729412507220"></a><ul id="ul729412507220"><li>PER：独享带宽</li><li>WHOLE：共享带宽</li></ul>
    </li></ul>
    <a name="ul1369035014203"></a><a name="ul1369035014203"></a><ul id="ul1369035014203"><li>约束：其中IPv6暂不支持WHOLE类型带宽。</li></ul>
    </td>
    </tr>
    <tr id="row5951536918414"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p6587627918414"><a name="p6587627918414"></a><a name="p6587627918414"></a>bandwidth_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p3318647218414"><a name="p3318647218414"></a><a name="p3318647218414"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p374970718414"><a name="p374970718414"></a><a name="p374970718414"></a>带宽名称。</p>
    </td>
    </tr>
    <tr id="row1066119511342"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p19564181313543"><a name="p19564181313543"></a><a name="p19564181313543"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p13564413185412"><a name="p13564413185412"></a><a name="p13564413185412"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul184004104214"></a><a name="ul184004104214"></a><ul id="ul184004104214"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。</li><li>创建弹性公网IP时，给弹性公网IP绑定企业项目ID。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  profile字段说明

    <a name="table66651219193417"></a>
    <table><thead align="left"><tr id="row167319197349"><th class="cellrowborder" valign="top" width="37.35%" id="mcps1.2.4.1.1"><p id="p206761195347"><a name="p206761195347"></a><a name="p206761195347"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.3%" id="mcps1.2.4.1.2"><p id="p156812193344"><a name="p156812193344"></a><a name="p156812193344"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="37.35%" id="mcps1.2.4.1.3"><p id="p17684101933410"><a name="p17684101933410"></a><a name="p17684101933410"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row962259102216"><td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.1 "><p id="p962309182220"><a name="p962309182220"></a><a name="p962309182220"></a>order_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.2.4.1.2 "><p id="p136231597223"><a name="p136231597223"></a><a name="p136231597223"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.3 "><p id="p26235912225"><a name="p26235912225"></a><a name="p26235912225"></a>订单的id</p>
    </td>
    </tr>
    <tr id="row18686141920341"><td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.1 "><p id="p11688201923418"><a name="p11688201923418"></a><a name="p11688201923418"></a>product_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.2.4.1.2 "><p id="p169318196347"><a name="p169318196347"></a><a name="p169318196347"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.3 "><p id="p149921832153419"><a name="p149921832153419"></a><a name="p149921832153419"></a>产品的id</p>
    </td>
    </tr>
    <tr id="row167161319173418"><td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.1 "><p id="p5718101903412"><a name="p5718101903412"></a><a name="p5718101903412"></a>region_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.2.4.1.2 "><p id="p47241019143417"><a name="p47241019143417"></a><a name="p47241019143417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.3 "><p id="p09201951174716"><a name="p09201951174716"></a><a name="p09201951174716"></a>region的id</p>
    </td>
    </tr>
    <tr id="row1472971912347"><td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.1 "><p id="p187311719103415"><a name="p187311719103415"></a><a name="p187311719103415"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.2.4.1.2 "><p id="p9735141923418"><a name="p9735141923418"></a><a name="p9735141923418"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.3 "><p id="p09931918183013"><a name="p09931918183013"></a><a name="p09931918183013"></a>用户的id</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "publicip": {
            "id": "2ec9b78d-9368-46f3-8f29-d1a95622a568",
            "status": "DOWN",
            "profile": {
              "user_id": "35f2b308f5d64441a6fa7999fbcd4321",
              "product_id": "00301-48027-0--0",
              "region_id": "xxx",
              "order_id": "xxxxxxxxx"
            },
            "type": "5_bgp",
            "public_ip_address": "161.xx.xx.12",
            "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
            "private_ip_address": "192.168.10.5",
            "create_time": "2015-07-16 04:32:50",
            "bandwidth_id": "49c8825b-bed9-46ff-9416-704b96d876a2",
            "bandwidth_share_type": "PER",
            "bandwidth_size": 10,    //EIP的带宽大小为10Mbit/s
            "bandwidth_name": "bandwidth-test",
            "enterprise_project_id":"b261ac1f-2489-4bc7-b31b-c33c3346a439",
            "ip_version": 4
        }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

