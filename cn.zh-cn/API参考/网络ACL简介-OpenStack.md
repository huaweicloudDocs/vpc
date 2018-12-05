# 网络ACLAPI简介<a name="ZH-CN_TOPIC_0060573712"></a>

## 对象简介<a name="section17132110121127"></a>

利用FWaaS API 2.0对网络ACL各对象模型进行管理和操作， 包括查询、创建、更新以及删除防火墙规则，查询、创建、更新以及删除防火墙策略，查询、创建、更新以及删除防火墙组等接口。

>![](public_sys-resources/icon-note.gif) **说明：**   
>网络ACL默认拒绝弹性云服务器所有出入子网的流量，这个默认的规则不允许查询和修改。  

## 对象模型<a name="section52827914121127"></a>

**表 1**  Firewall Rule对象

<a name="table38646929121127"></a>
<table><thead align="left"><tr id="row18263398121127"><th class="cellrowborder" valign="top" width="19.191919191919194%" id="mcps1.2.7.1.1"><p id="p2027461121127"><a name="p2027461121127"></a><a name="p2027461121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="12.121212121212121%" id="mcps1.2.7.1.2"><p id="p51747644121127"><a name="p51747644121127"></a><a name="p51747644121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.101010101010102%" id="mcps1.2.7.1.3"><p id="p11799274121127"><a name="p11799274121127"></a><a name="p11799274121127"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="10.101010101010102%" id="mcps1.2.7.1.4"><p id="p5535215121127"><a name="p5535215121127"></a><a name="p5535215121127"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="21.21212121212121%" id="mcps1.2.7.1.5"><p id="p13528938121127"><a name="p13528938121127"></a><a name="p13528938121127"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="27.272727272727277%" id="mcps1.2.7.1.6"><p id="p12805757121127"><a name="p12805757121127"></a><a name="p12805757121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row39528007121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p7362024121127"><a name="p7362024121127"></a><a name="p7362024121127"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p53278848121127"><a name="p53278848121127"></a><a name="p53278848121127"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p35056942121127"><a name="p35056942121127"></a><a name="p35056942121127"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p25980692121127"><a name="p25980692121127"></a><a name="p25980692121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p28349777121127"><a name="p28349777121127"></a><a name="p28349777121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p13095685121127"><a name="p13095685121127"></a><a name="p13095685121127"></a>网络ACL规则的uuid标识。</p>
</td>
</tr>
<tr id="row3417421121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p16296528121127"><a name="p16296528121127"></a><a name="p16296528121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p52887833121127"><a name="p52887833121127"></a><a name="p52887833121127"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p8244937121127"><a name="p8244937121127"></a><a name="p8244937121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p52909184121127"><a name="p52909184121127"></a><a name="p52909184121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p12447583121127"><a name="p12447583121127"></a><a name="p12447583121127"></a>最长255个字符</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p29399172121127"><a name="p29399172121127"></a><a name="p29399172121127"></a>网络ACL规则名称。</p>
</td>
</tr>
<tr id="row33772147121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p62102623121127"><a name="p62102623121127"></a><a name="p62102623121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p30062050121127"><a name="p30062050121127"></a><a name="p30062050121127"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p66726428121127"><a name="p66726428121127"></a><a name="p66726428121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p15622188121127"><a name="p15622188121127"></a><a name="p15622188121127"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p32185140121127"><a name="p32185140121127"></a><a name="p32185140121127"></a>最长255个字符</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p64485971121127"><a name="p64485971121127"></a><a name="p64485971121127"></a>网络ACL规则描述。</p>
</td>
</tr>
<tr id="row39157453121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p40485546121127"><a name="p40485546121127"></a><a name="p40485546121127"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p20366062121127"><a name="p20366062121127"></a><a name="p20366062121127"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p7409850121127"><a name="p7409850121127"></a><a name="p7409850121127"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p59988268121127"><a name="p59988268121127"></a><a name="p59988268121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p9626981121127"><a name="p9626981121127"></a><a name="p9626981121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p50600582121127"><a name="p50600582121127"></a><a name="p50600582121127"></a>项目ID</p>
</td>
</tr>
<tr id="row13612334121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p3945861121127"><a name="p3945861121127"></a><a name="p3945861121127"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p53059091121127"><a name="p53059091121127"></a><a name="p53059091121127"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p47556088121127"><a name="p47556088121127"></a><a name="p47556088121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p42688595121127"><a name="p42688595121127"></a><a name="p42688595121127"></a>false</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p32488518121127"><a name="p32488518121127"></a><a name="p32488518121127"></a>true或false</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p46007536121127"><a name="p46007536121127"></a><a name="p46007536121127"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row66347377121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p7361769121127"><a name="p7361769121127"></a><a name="p7361769121127"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p50019959121127"><a name="p50019959121127"></a><a name="p50019959121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p29808957121127"><a name="p29808957121127"></a><a name="p29808957121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p56212570121127"><a name="p56212570121127"></a><a name="p56212570121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p49011438121127"><a name="p49011438121127"></a><a name="p49011438121127"></a>支持TCP,UDP,ICMP, 或者0-255</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p36897817121127"><a name="p36897817121127"></a><a name="p36897817121127"></a>IP协议。</p>
</td>
</tr>
<tr id="row8703753121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p5943474121127"><a name="p5943474121127"></a><a name="p5943474121127"></a>source_port</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p59206978121127"><a name="p59206978121127"></a><a name="p59206978121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p32556505121127"><a name="p32556505121127"></a><a name="p32556505121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p41719704121127"><a name="p41719704121127"></a><a name="p41719704121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p8739741121127"><a name="p8739741121127"></a><a name="p8739741121127"></a>位于[1,65535]中一个整数或者一段端口范围a:b</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p62826249121127"><a name="p62826249121127"></a><a name="p62826249121127"></a>源端口号或者一段端口范围。</p>
</td>
</tr>
<tr id="row52935496121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p12876203121127"><a name="p12876203121127"></a><a name="p12876203121127"></a>destination_port</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p66631365121127"><a name="p66631365121127"></a><a name="p66631365121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p9722293121127"><a name="p9722293121127"></a><a name="p9722293121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p59680157121127"><a name="p59680157121127"></a><a name="p59680157121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p34781596121127"><a name="p34781596121127"></a><a name="p34781596121127"></a>位于[1,65535]中一个整数或者一段端口范围a:b</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p66851026121127"><a name="p66851026121127"></a><a name="p66851026121127"></a>目的端口号或者一段端口范围。</p>
</td>
</tr>
<tr id="row37973187121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p18090983121127"><a name="p18090983121127"></a><a name="p18090983121127"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p15064211121127"><a name="p15064211121127"></a><a name="p15064211121127"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p20909029121127"><a name="p20909029121127"></a><a name="p20909029121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p28336894121127"><a name="p28336894121127"></a><a name="p28336894121127"></a>4</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p49923839121127"><a name="p49923839121127"></a><a name="p49923839121127"></a>IPv4/IPv6</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p10402054121127"><a name="p10402054121127"></a><a name="p10402054121127"></a>IP协议版本。</p>
</td>
</tr>
<tr id="row34581454121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p61377852121127"><a name="p61377852121127"></a><a name="p61377852121127"></a>source_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p36483585121127"><a name="p36483585121127"></a><a name="p36483585121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p56274236121127"><a name="p56274236121127"></a><a name="p56274236121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p31125007121127"><a name="p31125007121127"></a><a name="p31125007121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p16531353121127"><a name="p16531353121127"></a><a name="p16531353121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p31475962121127"><a name="p31475962121127"></a><a name="p31475962121127"></a>源地址或者CIDR。</p>
</td>
</tr>
<tr id="row13949121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p43901244121127"><a name="p43901244121127"></a><a name="p43901244121127"></a>destination_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p14651426121127"><a name="p14651426121127"></a><a name="p14651426121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p51666000121127"><a name="p51666000121127"></a><a name="p51666000121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p43023076121127"><a name="p43023076121127"></a><a name="p43023076121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p8502527121127"><a name="p8502527121127"></a><a name="p8502527121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p53743554121127"><a name="p53743554121127"></a><a name="p53743554121127"></a>目的地址或者CIDR。</p>
</td>
</tr>
<tr id="row33223843121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p40131900121127"><a name="p40131900121127"></a><a name="p40131900121127"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p952780121127"><a name="p952780121127"></a><a name="p952780121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p19347827121127"><a name="p19347827121127"></a><a name="p19347827121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p24676176121127"><a name="p24676176121127"></a><a name="p24676176121127"></a>DENY</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p13986437121127"><a name="p13986437121127"></a><a name="p13986437121127"></a>DENY/ALLOW</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p16135729121127"><a name="p16135729121127"></a><a name="p16135729121127"></a>对通过网络ACL的流量执行的操作。</p>
</td>
</tr>
<tr id="row11398101121127"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p50347088121127"><a name="p50347088121127"></a><a name="p50347088121127"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p46161809121127"><a name="p46161809121127"></a><a name="p46161809121127"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p22993593121127"><a name="p22993593121127"></a><a name="p22993593121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p3919593121127"><a name="p3919593121127"></a><a name="p3919593121127"></a>true</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p53180735121127"><a name="p53180735121127"></a><a name="p53180735121127"></a>true/false</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p57324252121127"><a name="p57324252121127"></a><a name="p57324252121127"></a>是否使能网络ACL规则。</p>
</td>
</tr>
<tr id="row1574912215580"><td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.2.7.1.1 "><p id="p1312116475819"><a name="p1312116475819"></a><a name="p1312116475819"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.7.1.2 "><p id="p5125543583"><a name="p5125543583"></a><a name="p5125543583"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p31304475810"><a name="p31304475810"></a><a name="p31304475810"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.4 "><p id="p31326414587"><a name="p31326414587"></a><a name="p31326414587"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.7.1.5 "><p id="p21381447583"><a name="p21381447583"></a><a name="p21381447583"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.2.7.1.6 "><p id="p414013495814"><a name="p414013495814"></a><a name="p414013495814"></a>资源project_id</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Firewall Policy对象

<a name="table17002720121127"></a>
<table><thead align="left"><tr id="row16929792121127"><th class="cellrowborder" valign="top" width="17.351735173517348%" id="mcps1.2.7.1.1"><p id="p18873879121127"><a name="p18873879121127"></a><a name="p18873879121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="12.241224122412241%" id="mcps1.2.7.1.2"><p id="p12638309121127"><a name="p12638309121127"></a><a name="p12638309121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.2010201020102%" id="mcps1.2.7.1.3"><p id="p48863754121127"><a name="p48863754121127"></a><a name="p48863754121127"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="11.221122112211221%" id="mcps1.2.7.1.4"><p id="p30168613121127"><a name="p30168613121127"></a><a name="p30168613121127"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="24.492449244924494%" id="mcps1.2.7.1.5"><p id="p18152408121127"><a name="p18152408121127"></a><a name="p18152408121127"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="24.492449244924494%" id="mcps1.2.7.1.6"><p id="p61199938121127"><a name="p61199938121127"></a><a name="p61199938121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46402691121127"><td class="cellrowborder" valign="top" width="17.351735173517348%" headers="mcps1.2.7.1.1 "><p id="p11805115121127"><a name="p11805115121127"></a><a name="p11805115121127"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="12.241224122412241%" headers="mcps1.2.7.1.2 "><p id="p13006089121127"><a name="p13006089121127"></a><a name="p13006089121127"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="10.2010201020102%" headers="mcps1.2.7.1.3 "><p id="p47432079121127"><a name="p47432079121127"></a><a name="p47432079121127"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.221122112211221%" headers="mcps1.2.7.1.4 "><p id="p2727532121127"><a name="p2727532121127"></a><a name="p2727532121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.5 "><p id="p65470144121127"><a name="p65470144121127"></a><a name="p65470144121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.6 "><p id="p13152683121127"><a name="p13152683121127"></a><a name="p13152683121127"></a>网络ACL策略uuid标识。</p>
</td>
</tr>
<tr id="row9858171121127"><td class="cellrowborder" valign="top" width="17.351735173517348%" headers="mcps1.2.7.1.1 "><p id="p49865700121127"><a name="p49865700121127"></a><a name="p49865700121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="12.241224122412241%" headers="mcps1.2.7.1.2 "><p id="p6225460121127"><a name="p6225460121127"></a><a name="p6225460121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.2010201020102%" headers="mcps1.2.7.1.3 "><p id="p36011147121127"><a name="p36011147121127"></a><a name="p36011147121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.221122112211221%" headers="mcps1.2.7.1.4 "><p id="p63519754121127"><a name="p63519754121127"></a><a name="p63519754121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.5 "><p id="p6010319121127"><a name="p6010319121127"></a><a name="p6010319121127"></a>最长255个字符</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.6 "><p id="p40337147121127"><a name="p40337147121127"></a><a name="p40337147121127"></a>网络ACL策略名称。</p>
</td>
</tr>
<tr id="row61803802121127"><td class="cellrowborder" valign="top" width="17.351735173517348%" headers="mcps1.2.7.1.1 "><p id="p39621949121127"><a name="p39621949121127"></a><a name="p39621949121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.241224122412241%" headers="mcps1.2.7.1.2 "><p id="p66053143121127"><a name="p66053143121127"></a><a name="p66053143121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.2010201020102%" headers="mcps1.2.7.1.3 "><p id="p8380615121127"><a name="p8380615121127"></a><a name="p8380615121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.221122112211221%" headers="mcps1.2.7.1.4 "><p id="p40554095121127"><a name="p40554095121127"></a><a name="p40554095121127"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.5 "><p id="p23252014121127"><a name="p23252014121127"></a><a name="p23252014121127"></a>最长255个字符</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.6 "><p id="p15357220121127"><a name="p15357220121127"></a><a name="p15357220121127"></a>网络ACL策略描述。</p>
</td>
</tr>
<tr id="row57644277121127"><td class="cellrowborder" valign="top" width="17.351735173517348%" headers="mcps1.2.7.1.1 "><p id="p9761241121127"><a name="p9761241121127"></a><a name="p9761241121127"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.241224122412241%" headers="mcps1.2.7.1.2 "><p id="p20138053121127"><a name="p20138053121127"></a><a name="p20138053121127"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="10.2010201020102%" headers="mcps1.2.7.1.3 "><p id="p48743767121127"><a name="p48743767121127"></a><a name="p48743767121127"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.221122112211221%" headers="mcps1.2.7.1.4 "><p id="p41562672121127"><a name="p41562672121127"></a><a name="p41562672121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.5 "><p id="p16872433121127"><a name="p16872433121127"></a><a name="p16872433121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.6 "><p id="p24644536121127"><a name="p24644536121127"></a><a name="p24644536121127"></a>项目ID</p>
</td>
</tr>
<tr id="row33369184121127"><td class="cellrowborder" valign="top" width="17.351735173517348%" headers="mcps1.2.7.1.1 "><p id="p16940942121127"><a name="p16940942121127"></a><a name="p16940942121127"></a>firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="12.241224122412241%" headers="mcps1.2.7.1.2 "><p id="p27024915121127"><a name="p27024915121127"></a><a name="p27024915121127"></a>List</p>
</td>
<td class="cellrowborder" valign="top" width="10.2010201020102%" headers="mcps1.2.7.1.3 "><p id="p7363342121127"><a name="p7363342121127"></a><a name="p7363342121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.221122112211221%" headers="mcps1.2.7.1.4 "><p id="p3007905121127"><a name="p3007905121127"></a><a name="p3007905121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.5 "><p id="p21678315121127"><a name="p21678315121127"></a><a name="p21678315121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.6 "><p id="p53455884121127"><a name="p53455884121127"></a><a name="p53455884121127"></a>策略引用的网络ACL规则链。</p>
</td>
</tr>
<tr id="row717167121127"><td class="cellrowborder" valign="top" width="17.351735173517348%" headers="mcps1.2.7.1.1 "><p id="p30704110121127"><a name="p30704110121127"></a><a name="p30704110121127"></a>audited</p>
</td>
<td class="cellrowborder" valign="top" width="12.241224122412241%" headers="mcps1.2.7.1.2 "><p id="p10804884121127"><a name="p10804884121127"></a><a name="p10804884121127"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="10.2010201020102%" headers="mcps1.2.7.1.3 "><p id="p58859650121127"><a name="p58859650121127"></a><a name="p58859650121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.221122112211221%" headers="mcps1.2.7.1.4 "><p id="p26705110121127"><a name="p26705110121127"></a><a name="p26705110121127"></a>false</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.5 "><p id="p17417393121127"><a name="p17417393121127"></a><a name="p17417393121127"></a>true/false</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.6 "><p id="p3925300121127"><a name="p3925300121127"></a><a name="p3925300121127"></a>审计标记。</p>
</td>
</tr>
<tr id="row40905717121127"><td class="cellrowborder" valign="top" width="17.351735173517348%" headers="mcps1.2.7.1.1 "><p id="p16821838121127"><a name="p16821838121127"></a><a name="p16821838121127"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="12.241224122412241%" headers="mcps1.2.7.1.2 "><p id="p49691806121127"><a name="p49691806121127"></a><a name="p49691806121127"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="10.2010201020102%" headers="mcps1.2.7.1.3 "><p id="p366085121127"><a name="p366085121127"></a><a name="p366085121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.221122112211221%" headers="mcps1.2.7.1.4 "><p id="p44029346121127"><a name="p44029346121127"></a><a name="p44029346121127"></a>false</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.5 "><p id="p39776919121127"><a name="p39776919121127"></a><a name="p39776919121127"></a>true或false</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.6 "><p id="p31604739121127"><a name="p31604739121127"></a><a name="p31604739121127"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row109594223354"><td class="cellrowborder" valign="top" width="17.351735173517348%" headers="mcps1.2.7.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.241224122412241%" headers="mcps1.2.7.1.2 "><p id="p17700201411911"><a name="p17700201411911"></a><a name="p17700201411911"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="10.2010201020102%" headers="mcps1.2.7.1.3 "><p id="p15700614790"><a name="p15700614790"></a><a name="p15700614790"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.221122112211221%" headers="mcps1.2.7.1.4 "><p id="p17000141292"><a name="p17000141292"></a><a name="p17000141292"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.5 "><p id="p1470010141396"><a name="p1470010141396"></a><a name="p1470010141396"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="24.492449244924494%" headers="mcps1.2.7.1.6 "><p id="p7700714691"><a name="p7700714691"></a><a name="p7700714691"></a>资源project_id</p>
</td>
</tr>
</tbody>
</table>

**表 3**  Firewall Group对象

<a name="table31629250121127"></a>
<table><thead align="left"><tr id="row45711693121127"><th class="cellrowborder" valign="top" width="18.56%" id="mcps1.2.7.1.1"><p id="p46819705121127"><a name="p46819705121127"></a><a name="p46819705121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="11.34%" id="mcps1.2.7.1.2"><p id="p35064605121127"><a name="p35064605121127"></a><a name="p35064605121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.31%" id="mcps1.2.7.1.3"><p id="p56718680121127"><a name="p56718680121127"></a><a name="p56718680121127"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="10.31%" id="mcps1.2.7.1.4"><p id="p1971018121127"><a name="p1971018121127"></a><a name="p1971018121127"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="26.8%" id="mcps1.2.7.1.5"><p id="p2108435121127"><a name="p2108435121127"></a><a name="p2108435121127"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="22.68%" id="mcps1.2.7.1.6"><p id="p11952850121127"><a name="p11952850121127"></a><a name="p11952850121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row20395689121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p50168503121127"><a name="p50168503121127"></a><a name="p50168503121127"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p47513116121127"><a name="p47513116121127"></a><a name="p47513116121127"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p30850039121127"><a name="p30850039121127"></a><a name="p30850039121127"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p62237546121127"><a name="p62237546121127"></a><a name="p62237546121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p8066964121127"><a name="p8066964121127"></a><a name="p8066964121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p62072725121127"><a name="p62072725121127"></a><a name="p62072725121127"></a>网络ACL组的uuid标识。</p>
</td>
</tr>
<tr id="row34896104121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p52608071121127"><a name="p52608071121127"></a><a name="p52608071121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p59846605121127"><a name="p59846605121127"></a><a name="p59846605121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p12676251121127"><a name="p12676251121127"></a><a name="p12676251121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p63580111121127"><a name="p63580111121127"></a><a name="p63580111121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p38515338121127"><a name="p38515338121127"></a><a name="p38515338121127"></a>最长255个字符</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p28604909121127"><a name="p28604909121127"></a><a name="p28604909121127"></a>网络ACL组名称。</p>
</td>
</tr>
<tr id="row11129246121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p39887063121127"><a name="p39887063121127"></a><a name="p39887063121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p28745735121127"><a name="p28745735121127"></a><a name="p28745735121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p35917390121127"><a name="p35917390121127"></a><a name="p35917390121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p7177931121127"><a name="p7177931121127"></a><a name="p7177931121127"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p51413152121127"><a name="p51413152121127"></a><a name="p51413152121127"></a>最长255个字符</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p35639020121127"><a name="p35639020121127"></a><a name="p35639020121127"></a>网络ACL组描述。</p>
</td>
</tr>
<tr id="row677472121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p60717947121127"><a name="p60717947121127"></a><a name="p60717947121127"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p65871708121127"><a name="p65871708121127"></a><a name="p65871708121127"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p40453924121127"><a name="p40453924121127"></a><a name="p40453924121127"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p19239924121127"><a name="p19239924121127"></a><a name="p19239924121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p56148714121127"><a name="p56148714121127"></a><a name="p56148714121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p38939943121127"><a name="p38939943121127"></a><a name="p38939943121127"></a>项目ID。</p>
</td>
</tr>
<tr id="row38137474121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p35500294121127"><a name="p35500294121127"></a><a name="p35500294121127"></a>ingress_firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p49995809121127"><a name="p49995809121127"></a><a name="p49995809121127"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p56977139121127"><a name="p56977139121127"></a><a name="p56977139121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p13896860121127"><a name="p13896860121127"></a><a name="p13896860121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p13169723121127"><a name="p13169723121127"></a><a name="p13169723121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p56499442121127"><a name="p56499442121127"></a><a name="p56499442121127"></a>入方向网络ACL策略。</p>
</td>
</tr>
<tr id="row9094936121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p34911245121127"><a name="p34911245121127"></a><a name="p34911245121127"></a>egress_firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p44624490121127"><a name="p44624490121127"></a><a name="p44624490121127"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p55860045121127"><a name="p55860045121127"></a><a name="p55860045121127"></a>CRUkua</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p43914199121127"><a name="p43914199121127"></a><a name="p43914199121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p45858089121127"><a name="p45858089121127"></a><a name="p45858089121127"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p37100641121127"><a name="p37100641121127"></a><a name="p37100641121127"></a>出方向网络ACL策略。</p>
</td>
</tr>
<tr id="row31622902121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p65911012121127"><a name="p65911012121127"></a><a name="p65911012121127"></a>ports</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p5459978121127"><a name="p5459978121127"></a><a name="p5459978121127"></a>List</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p59466631121127"><a name="p59466631121127"></a><a name="p59466631121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p59729531121127"><a name="p59729531121127"></a><a name="p59729531121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p61253638121127"><a name="p61253638121127"></a><a name="p61253638121127"></a>必须为分布式router的端口id</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p61002567121127"><a name="p61002567121127"></a><a name="p61002567121127"></a>网络ACL组绑定的端口列表。</p>
</td>
</tr>
<tr id="row48186031121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p33368479121127"><a name="p33368479121127"></a><a name="p33368479121127"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p7938198121127"><a name="p7938198121127"></a><a name="p7938198121127"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p28476597121127"><a name="p28476597121127"></a><a name="p28476597121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p21843738121127"><a name="p21843738121127"></a><a name="p21843738121127"></a>false</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p18257126121127"><a name="p18257126121127"></a><a name="p18257126121127"></a>true或false</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p56166201121127"><a name="p56166201121127"></a><a name="p56166201121127"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row60912436121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p66273781121127"><a name="p66273781121127"></a><a name="p66273781121127"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p7141533121127"><a name="p7141533121127"></a><a name="p7141533121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p56408141121127"><a name="p56408141121127"></a><a name="p56408141121127"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p63225379121127"><a name="p63225379121127"></a><a name="p63225379121127"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p5235520121127"><a name="p5235520121127"></a><a name="p5235520121127"></a>取值范围：</p>
<p id="p54742923121127"><a name="p54742923121127"></a><a name="p54742923121127"></a>ACTIVE、CREATE、INACTIVE、PENDING_CREATE、PENDING_UPDATE、PENDING_DELETE、ERROR</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p6468335121127"><a name="p6468335121127"></a><a name="p6468335121127"></a>网络ACL策略的状态。</p>
</td>
</tr>
<tr id="row59833296121127"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p44051842121127"><a name="p44051842121127"></a><a name="p44051842121127"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p58587899121127"><a name="p58587899121127"></a><a name="p58587899121127"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p46385500121127"><a name="p46385500121127"></a><a name="p46385500121127"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p60725699121127"><a name="p60725699121127"></a><a name="p60725699121127"></a>true</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p30640465121127"><a name="p30640465121127"></a><a name="p30640465121127"></a>true/false</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p3428646121127"><a name="p3428646121127"></a><a name="p3428646121127"></a>网络ACL是否受管理员控制。</p>
</td>
</tr>
<tr id="row7228115213486"><td class="cellrowborder" valign="top" width="18.56%" headers="mcps1.2.7.1.1 "><p id="p53071912134918"><a name="p53071912134918"></a><a name="p53071912134918"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.34%" headers="mcps1.2.7.1.2 "><p id="p1731011220498"><a name="p1731011220498"></a><a name="p1731011220498"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.3 "><p id="p1731231211499"><a name="p1731231211499"></a><a name="p1731231211499"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="10.31%" headers="mcps1.2.7.1.4 "><p id="p6315412104917"><a name="p6315412104917"></a><a name="p6315412104917"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.2.7.1.5 "><p id="p7319712154912"><a name="p7319712154912"></a><a name="p7319712154912"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="22.68%" headers="mcps1.2.7.1.6 "><p id="p7321112124914"><a name="p7321112124914"></a><a name="p7321112124914"></a>资源project_id</p>
</td>
</tr>
</tbody>
</table>

