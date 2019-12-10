# 更新网络ACL规则<a name="vpc_firewall_0004"></a>

## 功能介绍<a name="section48881744123249"></a>

更新网络ACL规则。

## URI<a name="section40985924123249"></a>

PUT /v2.0/fwaas/firewall\_rules/\{firewall\_rule\_id\}

## 请求消息<a name="section49242216123249"></a>

**表 1**  请求参数

<a name="table30921260123249"></a>
<table><thead align="left"><tr id="row39375977123249"><th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.1"><p id="p12242224123249"><a name="p12242224123249"></a><a name="p12242224123249"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p24418590123249"><a name="p24418590123249"></a><a name="p24418590123249"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p13201747123249"><a name="p13201747123249"></a><a name="p13201747123249"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p62761712123249"><a name="p62761712123249"></a><a name="p62761712123249"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row57358099123249"><td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.1 "><p id="p46539485123249"><a name="p46539485123249"></a><a name="p46539485123249"></a>firewall_rule</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p13703023123249"><a name="p13703023123249"></a><a name="p13703023123249"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p21092839123249"><a name="p21092839123249"></a><a name="p21092839123249"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p3044429312329"><a name="p3044429312329"></a><a name="p3044429312329"></a>firewall rule对象。请参见<a href="#table38646929121127">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Firewall Rule对象

<a name="table38646929121127"></a>
<table><thead align="left"><tr id="row18263398121127"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p2027461121127"><a name="p2027461121127"></a><a name="p2027461121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="14.46%" id="mcps1.2.5.1.2"><p id="p1123219257010"><a name="p1123219257010"></a><a name="p1123219257010"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.63%" id="mcps1.2.5.1.3"><p id="p51747644121127"><a name="p51747644121127"></a><a name="p51747644121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.91%" id="mcps1.2.5.1.4"><p id="p12805757121127"><a name="p12805757121127"></a><a name="p12805757121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3417421121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p16296528121127"><a name="p16296528121127"></a><a name="p16296528121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p32328254015"><a name="p32328254015"></a><a name="p32328254015"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p52887833121127"><a name="p52887833121127"></a><a name="p52887833121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p29399172121127"><a name="p29399172121127"></a><a name="p29399172121127"></a>网络ACL规则名称。</p>
<p id="p4331339102"><a name="p4331339102"></a><a name="p4331339102"></a>使用说明：最长255个字符</p>
</td>
</tr>
<tr id="row33772147121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p62102623121127"><a name="p62102623121127"></a><a name="p62102623121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p52321025502"><a name="p52321025502"></a><a name="p52321025502"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p30062050121127"><a name="p30062050121127"></a><a name="p30062050121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p64485971121127"><a name="p64485971121127"></a><a name="p64485971121127"></a>网络ACL规则描述。</p>
<p id="p7311252002"><a name="p7311252002"></a><a name="p7311252002"></a>使用说明：最长255个字符</p>
</td>
</tr>
<tr id="row66347377121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p7361769121127"><a name="p7361769121127"></a><a name="p7361769121127"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p19232525600"><a name="p19232525600"></a><a name="p19232525600"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p50019959121127"><a name="p50019959121127"></a><a name="p50019959121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p36897817121127"><a name="p36897817121127"></a><a name="p36897817121127"></a>IP协议。</p>
<p id="p1094663315110"><a name="p1094663315110"></a><a name="p1094663315110"></a>取值范围：支持TCP,UDP,ICMP, 或者0-255</p>
</td>
</tr>
<tr id="row8703753121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p5943474121127"><a name="p5943474121127"></a><a name="p5943474121127"></a>source_port</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p723213251802"><a name="p723213251802"></a><a name="p723213251802"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p59206978121127"><a name="p59206978121127"></a><a name="p59206978121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p62826249121127"><a name="p62826249121127"></a><a name="p62826249121127"></a>源端口号或者一段端口范围。</p>
<p id="p169804712119"><a name="p169804712119"></a><a name="p169804712119"></a>取值范围：位于[1,65535]中一个整数或者一段端口范围a:b</p>
</td>
</tr>
<tr id="row52935496121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p12876203121127"><a name="p12876203121127"></a><a name="p12876203121127"></a>destination_port</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p523252516015"><a name="p523252516015"></a><a name="p523252516015"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p66631365121127"><a name="p66631365121127"></a><a name="p66631365121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p66851026121127"><a name="p66851026121127"></a><a name="p66851026121127"></a>目的端口号或者一段端口范围。</p>
<p id="p193204108218"><a name="p193204108218"></a><a name="p193204108218"></a>取值范围：位于[1,65535]中一个整数或者一段端口范围a:b</p>
</td>
</tr>
<tr id="row37973187121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p18090983121127"><a name="p18090983121127"></a><a name="p18090983121127"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p10232925809"><a name="p10232925809"></a><a name="p10232925809"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p15064211121127"><a name="p15064211121127"></a><a name="p15064211121127"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p10402054121127"><a name="p10402054121127"></a><a name="p10402054121127"></a>IP协议版本。</p>
<p id="p650618131322"><a name="p650618131322"></a><a name="p650618131322"></a>取值范围：IPv4/IPv6</p>
</td>
</tr>
<tr id="row34581454121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p61377852121127"><a name="p61377852121127"></a><a name="p61377852121127"></a>source_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p72320251009"><a name="p72320251009"></a><a name="p72320251009"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p36483585121127"><a name="p36483585121127"></a><a name="p36483585121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p31475962121127"><a name="p31475962121127"></a><a name="p31475962121127"></a>源地址或者CIDR。</p>
</td>
</tr>
<tr id="row13949121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p43901244121127"><a name="p43901244121127"></a><a name="p43901244121127"></a>destination_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p1023222510013"><a name="p1023222510013"></a><a name="p1023222510013"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p14651426121127"><a name="p14651426121127"></a><a name="p14651426121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p53743554121127"><a name="p53743554121127"></a><a name="p53743554121127"></a>目的地址或者CIDR。</p>
</td>
</tr>
<tr id="row33223843121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p40131900121127"><a name="p40131900121127"></a><a name="p40131900121127"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p152322253011"><a name="p152322253011"></a><a name="p152322253011"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p952780121127"><a name="p952780121127"></a><a name="p952780121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p16135729121127"><a name="p16135729121127"></a><a name="p16135729121127"></a>对通过网络ACL的流量执行的操作。</p>
<p id="p053482914220"><a name="p053482914220"></a><a name="p053482914220"></a>取值范围：DENY（拒绝）/ALLOW（允许）</p>
</td>
</tr>
<tr id="row11398101121127"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p50347088121127"><a name="p50347088121127"></a><a name="p50347088121127"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="14.46%" headers="mcps1.2.5.1.2 "><p id="p52321525707"><a name="p52321525707"></a><a name="p52321525707"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.63%" headers="mcps1.2.5.1.3 "><p id="p46161809121127"><a name="p46161809121127"></a><a name="p46161809121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="41.91%" headers="mcps1.2.5.1.4 "><p id="p57324252121127"><a name="p57324252121127"></a><a name="p57324252121127"></a>是否使能网络ACL规则。</p>
<p id="p117941758725"><a name="p117941758725"></a><a name="p117941758725"></a>取值范围：true/false</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section9857292123249"></a>

**表 3**  响应参数

<a name="table38652922123249"></a>
<table><thead align="left"><tr id="row54513389123249"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p28336710123249"><a name="p28336710123249"></a><a name="p28336710123249"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p47571350123249"><a name="p47571350123249"></a><a name="p47571350123249"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p23002266123249"><a name="p23002266123249"></a><a name="p23002266123249"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row47557263123249"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p57698555123249"><a name="p57698555123249"></a><a name="p57698555123249"></a>firewall_rule</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p31745790123249"><a name="p31745790123249"></a><a name="p31745790123249"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p35727944123249"><a name="p35727944123249"></a><a name="p35727944123249"></a>firewall rule对象。请参见<a href="#table96821221510">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  Firewall Rule对象

<a name="table96821221510"></a>
<table><thead align="left"><tr id="row1568212181517"><th class="cellrowborder" valign="top" width="32.76%" id="mcps1.2.4.1.1"><p id="p8681812161514"><a name="p8681812161514"></a><a name="p8681812161514"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="20.69%" id="mcps1.2.4.1.2"><p id="p13681312131518"><a name="p13681312131518"></a><a name="p13681312131518"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="46.550000000000004%" id="mcps1.2.4.1.3"><p id="p116816121152"><a name="p116816121152"></a><a name="p116816121152"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row39528007121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p7362024121127"><a name="p7362024121127"></a><a name="p7362024121127"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p53278848121127"><a name="p53278848121127"></a><a name="p53278848121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p13095685121127"><a name="p13095685121127"></a><a name="p13095685121127"></a>网络ACL规则的uuid标识。</p>
</td>
</tr>
<tr id="row1870712181518"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p2070121214156"><a name="p2070121214156"></a><a name="p2070121214156"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p570161218158"><a name="p570161218158"></a><a name="p570161218158"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p2070171271514"><a name="p2070171271514"></a><a name="p2070171271514"></a>网络ACL规则名称。</p>
</td>
</tr>
<tr id="row47051241512"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p1970141281520"><a name="p1970141281520"></a><a name="p1970141281520"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p67031271510"><a name="p67031271510"></a><a name="p67031271510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p1270412111511"><a name="p1270412111511"></a><a name="p1270412111511"></a>网络ACL规则描述。</p>
</td>
</tr>
<tr id="row39157453121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p40485546121127"><a name="p40485546121127"></a><a name="p40485546121127"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p20366062121127"><a name="p20366062121127"></a><a name="p20366062121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row13612334121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p3945861121127"><a name="p3945861121127"></a><a name="p3945861121127"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p53059091121127"><a name="p53059091121127"></a><a name="p53059091121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p46007536121127"><a name="p46007536121127"></a><a name="p46007536121127"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row2070312131513"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p1570141241512"><a name="p1570141241512"></a><a name="p1570141241512"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p0701312161512"><a name="p0701312161512"></a><a name="p0701312161512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p17061201515"><a name="p17061201515"></a><a name="p17061201515"></a>IP协议。</p>
</td>
</tr>
<tr id="row1170181217153"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p12701112161517"><a name="p12701112161517"></a><a name="p12701112161517"></a>source_port</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p127021218159"><a name="p127021218159"></a><a name="p127021218159"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p137011241510"><a name="p137011241510"></a><a name="p137011241510"></a>源端口号或者一段端口范围。</p>
</td>
</tr>
<tr id="row8701112181514"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p470312191512"><a name="p470312191512"></a><a name="p470312191512"></a>destination_port</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p177081291516"><a name="p177081291516"></a><a name="p177081291516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p1770121217158"><a name="p1770121217158"></a><a name="p1770121217158"></a>目的端口号或者一段端口范围。</p>
</td>
</tr>
<tr id="row07071212159"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p1370912131514"><a name="p1370912131514"></a><a name="p1370912131514"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p770212111514"><a name="p770212111514"></a><a name="p770212111514"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p13701112161518"><a name="p13701112161518"></a><a name="p13701112161518"></a>IP协议版本。</p>
</td>
</tr>
<tr id="row1070171261513"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p1970412151510"><a name="p1970412151510"></a><a name="p1970412151510"></a>source_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p14701812161510"><a name="p14701812161510"></a><a name="p14701812161510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p19701412201516"><a name="p19701412201516"></a><a name="p19701412201516"></a>源地址或者CIDR。</p>
</td>
</tr>
<tr id="row167031212158"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p77061219153"><a name="p77061219153"></a><a name="p77061219153"></a>destination_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p1870712131519"><a name="p1870712131519"></a><a name="p1870712131519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p1470712111516"><a name="p1470712111516"></a><a name="p1470712111516"></a>目的地址或者CIDR。</p>
</td>
</tr>
<tr id="row17051231516"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p13701512171516"><a name="p13701512171516"></a><a name="p13701512171516"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p871161221515"><a name="p871161221515"></a><a name="p871161221515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p87131291511"><a name="p87131291511"></a><a name="p87131291511"></a>对通过网络ACL的流量执行的操作。</p>
</td>
</tr>
<tr id="row571121210154"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p1571712101514"><a name="p1571712101514"></a><a name="p1571712101514"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p137131218159"><a name="p137131218159"></a><a name="p137131218159"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p167121271512"><a name="p167121271512"></a><a name="p167121271512"></a>是否使能网络ACL规则。</p>
</td>
</tr>
<tr id="row1574912215580"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p1312116475819"><a name="p1312116475819"></a><a name="p1312116475819"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p5125543583"><a name="p5125543583"></a><a name="p5125543583"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p331433615284"><a name="p331433615284"></a><a name="p331433615284"></a>项目ID</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section10725923123249"></a>

请求样例

```
PUT https://{Endpoint}/v2.0/fwaas/firewall_rules/b94acf06-efc2-485d-ba67-a61acf2a7e28

{
    "firewall_rule": {
        "action": "deny"
    }
}
```

响应样例

```
{
    "firewall_rule": {
        "protocol": "tcp", 
        "description": "", 
        "source_ip_address": null, 
        "destination_ip_address": null, 
        "source_port": null, 
        "destination_port": "80", 
        "id": "b94acf06-efc2-485d-ba67-a61acf2a7e28", 
        "name": "ALLOW_HTTP", 
        "tenant_id": "23c8a121505047b6869edf39f3062712", 
        "enabled": true, 
        "action": "deny", 
        "ip_version": 4, 
        "public": false,
        "project_id": "23c8a121505047b6869edf39f3062712"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

