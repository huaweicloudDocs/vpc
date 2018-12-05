# 子网API简介<a name="ZH-CN_TOPIC_0062160177"></a>

## 对象简介<a name="section66933755"></a>

对子网资源进行管理和操作，包括查询子网列表、创建子网、查询指定子网、删除子网以及更新子网等接口。

## 对象模型<a name="section65532886"></a>

**表 1**  subnet对象

<a name="table12211980105515"></a>
<table><thead align="left"><tr id="row32722637105515"><th class="cellrowborder" valign="top" width="15.568443155684433%" id="mcps1.2.8.1.1"><p id="p60075710105815"><a name="p60075710105815"></a><a name="p60075710105815"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="7.519248075192481%" id="mcps1.2.8.1.2"><p id="p194182022104514"><a name="p194182022104514"></a><a name="p194182022104514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.568443155684433%" id="mcps1.2.8.1.3"><p id="p34294369105815"><a name="p34294369105815"></a><a name="p34294369105815"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.239176082391761%" id="mcps1.2.8.1.4"><p id="p26380484105815"><a name="p26380484105815"></a><a name="p26380484105815"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="15.568443155684433%" id="mcps1.2.8.1.5"><p id="p56444431105815"><a name="p56444431105815"></a><a name="p56444431105815"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="13.728627137286272%" id="mcps1.2.8.1.6"><p id="p8596203105815"><a name="p8596203105815"></a><a name="p8596203105815"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="23.807619238076192%" id="mcps1.2.8.1.7"><p id="p25203839105815"><a name="p25203839105815"></a><a name="p25203839105815"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row28303131105515"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p2014344105614"><a name="p2014344105614"></a><a name="p2014344105614"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p17418122211459"><a name="p17418122211459"></a><a name="p17418122211459"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p28944191105614"><a name="p28944191105614"></a><a name="p28944191105614"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p62778163105614"><a name="p62778163105614"></a><a name="p62778163105614"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p51866443105614"><a name="p51866443105614"></a><a name="p51866443105614"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p40432368105614"><a name="p40432368105614"></a><a name="p40432368105614"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p53796361105614"><a name="p53796361105614"></a><a name="p53796361105614"></a>子网的id</p>
<p id="p2677113954519"><a name="p2677113954519"></a><a name="p2677113954519"></a>【使用说明】在查询子网列表时非必选</p>
</td>
</tr>
<tr id="row43081158105515"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p54833166105624"><a name="p54833166105624"></a><a name="p54833166105624"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p11418162219452"><a name="p11418162219452"></a><a name="p11418162219452"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p12301465105624"><a name="p12301465105624"></a><a name="p12301465105624"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p56894584105624"><a name="p56894584105624"></a><a name="p56894584105624"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p45058580105624"><a name="p45058580105624"></a><a name="p45058580105624"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p25866324105624"><a name="p25866324105624"></a><a name="p25866324105624"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p14797472105624"><a name="p14797472105624"></a><a name="p14797472105624"></a>子网的名称</p>
</td>
</tr>
<tr id="row9772661105515"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p49939441105624"><a name="p49939441105624"></a><a name="p49939441105624"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p841892219451"><a name="p841892219451"></a><a name="p841892219451"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p18562940105624"><a name="p18562940105624"></a><a name="p18562940105624"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p27203184105624"><a name="p27203184105624"></a><a name="p27203184105624"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p55974259105624"><a name="p55974259105624"></a><a name="p55974259105624"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p37621168105624"><a name="p37621168105624"></a><a name="p37621168105624"></a>4或6</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p27415757105624"><a name="p27415757105624"></a><a name="p27415757105624"></a>IP版本</p>
<p id="p45415223105624"><a name="p45415223105624"></a><a name="p45415223105624"></a>【使用说明】只支持IPv4</p>
</td>
</tr>
<tr id="row49397935105515"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p23027912105624"><a name="p23027912105624"></a><a name="p23027912105624"></a>ipv6_address_mode</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p3418622124511"><a name="p3418622124511"></a><a name="p3418622124511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p53321590105624"><a name="p53321590105624"></a><a name="p53321590105624"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p24081573105624"><a name="p24081573105624"></a><a name="p24081573105624"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p4450429105624"><a name="p4450429105624"></a><a name="p4450429105624"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p24940453105624"><a name="p24940453105624"></a><a name="p24940453105624"></a>"dhcpv6-stateful'、'dhcpv6-stateless'、'slaac'</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p6910789105624"><a name="p6910789105624"></a><a name="p6910789105624"></a>IPv6寻址模式</p>
<p id="p62197106105624"><a name="p62197106105624"></a><a name="p62197106105624"></a>【使用说明】不支持</p>
</td>
</tr>
<tr id="row25915264105515"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p43207439105624"><a name="p43207439105624"></a><a name="p43207439105624"></a>ipv6_ra_mode</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p541812294510"><a name="p541812294510"></a><a name="p541812294510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p10141705105624"><a name="p10141705105624"></a><a name="p10141705105624"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p16171804105624"><a name="p16171804105624"></a><a name="p16171804105624"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p34847727105624"><a name="p34847727105624"></a><a name="p34847727105624"></a>N/A""</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p4093610105624"><a name="p4093610105624"></a><a name="p4093610105624"></a>"dhcpv6-stateful'、'dhcpv6-stateless'、'slaac'</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p63146998105624"><a name="p63146998105624"></a><a name="p63146998105624"></a>IPv6路由广播模式</p>
<p id="p31452074105624"><a name="p31452074105624"></a><a name="p31452074105624"></a>【使用说明】不支持</p>
</td>
</tr>
<tr id="row25349309105515"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p4452630910577"><a name="p4452630910577"></a><a name="p4452630910577"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p641822254515"><a name="p641822254515"></a><a name="p641822254515"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p4986127810577"><a name="p4986127810577"></a><a name="p4986127810577"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p1223175210577"><a name="p1223175210577"></a><a name="p1223175210577"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p5124788310577"><a name="p5124788310577"></a><a name="p5124788310577"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p5743783810577"><a name="p5743783810577"></a><a name="p5743783810577"></a>存在的网络id</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p2195327310577"><a name="p2195327310577"></a><a name="p2195327310577"></a>所属网络的id</p>
</td>
</tr>
<tr id="row8244803105515"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p3202678510577"><a name="p3202678510577"></a><a name="p3202678510577"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p2418122234515"><a name="p2418122234515"></a><a name="p2418122234515"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p4403276010577"><a name="p4403276010577"></a><a name="p4403276010577"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p988382810577"><a name="p988382810577"></a><a name="p988382810577"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p6239263710577"><a name="p6239263710577"></a><a name="p6239263710577"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p2063884210577"><a name="p2063884210577"></a><a name="p2063884210577"></a>合法的CIDR格式</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p6113352410577"><a name="p6113352410577"></a><a name="p6113352410577"></a>CIDR格式</p>
<p id="p1333080710577"><a name="p1333080710577"></a><a name="p1333080710577"></a>【使用说明】只支持10.0.0.0/8,172.16.0.0/12,192.168.0.0/16三个网段内的地址，掩码长度不能大于28。</p>
</td>
</tr>
<tr id="row62757710105647"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p5097986810577"><a name="p5097986810577"></a><a name="p5097986810577"></a>gateway_ip</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p1841872219452"><a name="p1841872219452"></a><a name="p1841872219452"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p3572863210577"><a name="p3572863210577"></a><a name="p3572863210577"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p833804010577"><a name="p833804010577"></a><a name="p833804010577"></a>CRUD</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p429261210577"><a name="p429261210577"></a><a name="p429261210577"></a>CIDR中的第一个IP</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p1215731710577"><a name="p1215731710577"></a><a name="p1215731710577"></a>合法的IP地址或者空值</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p1242857210116"><a name="p1242857210116"></a><a name="p1242857210116"></a>网关IP不允许和allocation_pools地址块冲突。</p>
<p id="p854120544319"><a name="p854120544319"></a><a name="p854120544319"></a>【使用说明】不支持修改。</p>
</td>
</tr>
<tr id="row2545218105647"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p1395064410577"><a name="p1395064410577"></a><a name="p1395064410577"></a>allocation_pools</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p19418122284515"><a name="p19418122284515"></a><a name="p19418122284515"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p5626034310577"><a name="p5626034310577"></a><a name="p5626034310577"></a>List(allocation_pool)</p>
<p id="p3658104710577"><a name="p3658104710577"></a><a name="p3658104710577"></a></p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p1027483910577"><a name="p1027483910577"></a><a name="p1027483910577"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p2695561110577"><a name="p2695561110577"></a><a name="p2695561110577"></a>CIDR中的地址除了网关和广播地址的所有IP</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p3592087610577"><a name="p3592087610577"></a><a name="p3592087610577"></a>范围的起止IP必须是合法IP地址</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p2390980910577"><a name="p2390980910577"></a><a name="p2390980910577"></a>可用的IP池，allocation_pool对象参见<a href="#ZH-CN_TOPIC_0062160177__table24611730">表2</a></p>
<p id="p1386169010577"><a name="p1386169010577"></a><a name="p1386169010577"></a>例如：[ { "start": "10.0.0.2", "end": "10.0.0.251"} ]</p>
<p id="p1961191927"><a name="p1961191927"></a><a name="p1961191927"></a>每个子网的第1个和最后3个IP地址为系统保留地址。以192.168.1.0/24为例，192.168.1.0、 192.168.1.253、192.168.1.254和192.168.1.255这些地址是系统保留地址。系统预留地址默认不在allocation_pool范围内。</p>
<p id="p5764635410577"><a name="p5764635410577"></a><a name="p5764635410577"></a>约束：更新时allocation_pool范围不能包含网关和广播地址的所有IP</p>
</td>
</tr>
<tr id="row22360302105653"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p1404384110577"><a name="p1404384110577"></a><a name="p1404384110577"></a>dns_nameservers</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p2418922154512"><a name="p2418922154512"></a><a name="p2418922154512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p6380932110577"><a name="p6380932110577"></a><a name="p6380932110577"></a>List(String)</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p117248910577"><a name="p117248910577"></a><a name="p117248910577"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p2786279410577"><a name="p2786279410577"></a><a name="p2786279410577"></a>空列表</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p4229384310577"><a name="p4229384310577"></a><a name="p4229384310577"></a>最大为5个</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p324929310577"><a name="p324929310577"></a><a name="p324929310577"></a>dns服务器</p>
<p id="p2924364410577"><a name="p2924364410577"></a><a name="p2924364410577"></a>例如："dns_nameservers": ["8.xx.xx.8","8.xx.xx.4"]</p>
</td>
</tr>
<tr id="row17847900105653"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p4510693110577"><a name="p4510693110577"></a><a name="p4510693110577"></a>host_routes</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p3418112264518"><a name="p3418112264518"></a><a name="p3418112264518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p2978276610577"><a name="p2978276610577"></a><a name="p2978276610577"></a>List(host_route)</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p6359385010577"><a name="p6359385010577"></a><a name="p6359385010577"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p5082822210577"><a name="p5082822210577"></a><a name="p5082822210577"></a>空列表</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p2344534710577"><a name="p2344534710577"></a><a name="p2344534710577"></a>最大个数为20个</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p2002497710577"><a name="p2002497710577"></a><a name="p2002497710577"></a>虚拟机静态路由，参见“host_route对象”表</p>
<p id="p4600706610577"><a name="p4600706610577"></a><a name="p4600706610577"></a>【使用说明】不支持，忽略输入信息</p>
</td>
</tr>
<tr id="row42017779105653"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p5182838910577"><a name="p5182838910577"></a><a name="p5182838910577"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p184189229458"><a name="p184189229458"></a><a name="p184189229458"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p3734998010577"><a name="p3734998010577"></a><a name="p3734998010577"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p544953110577"><a name="p544953110577"></a><a name="p544953110577"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p3875889110577"><a name="p3875889110577"></a><a name="p3875889110577"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p5246248410577"><a name="p5246248410577"></a><a name="p5246248410577"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p2160278110577"><a name="p2160278110577"></a><a name="p2160278110577"></a>项目ID。</p>
</td>
</tr>
<tr id="row21625046105653"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p4495318510577"><a name="p4495318510577"></a><a name="p4495318510577"></a>enable_dhcp</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p1041812214516"><a name="p1041812214516"></a><a name="p1041812214516"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p1732939410577"><a name="p1732939410577"></a><a name="p1732939410577"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p6150371210577"><a name="p6150371210577"></a><a name="p6150371210577"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p1574478610577"><a name="p1574478610577"></a><a name="p1574478610577"></a>true</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p25931310577"><a name="p25931310577"></a><a name="p25931310577"></a>true或false</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p2100438810577"><a name="p2100438810577"></a><a name="p2100438810577"></a>是否启动dhcp，false表示不提供dhcp服务的能力</p>
<p id="p5482176910577"><a name="p5482176910577"></a><a name="p5482176910577"></a>【使用说明】只支持true</p>
</td>
</tr>
<tr id="row63315321123"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p17700201411911"><a name="p17700201411911"></a><a name="p17700201411911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p45641422124917"><a name="p45641422124917"></a><a name="p45641422124917"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p17000141292"><a name="p17000141292"></a><a name="p17000141292"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p1470010141396"><a name="p1470010141396"></a><a name="p1470010141396"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p870017141892"><a name="p870017141892"></a><a name="p870017141892"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p7700714691"><a name="p7700714691"></a><a name="p7700714691"></a>资源project_id</p>
</td>
</tr>
<tr id="row126291040191211"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p6953241598"><a name="p6953241598"></a><a name="p6953241598"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p6953441993"><a name="p6953441993"></a><a name="p6953441993"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p11953164120911"><a name="p11953164120911"></a><a name="p11953164120911"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p595314119912"><a name="p595314119912"></a><a name="p595314119912"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间</p>
</td>
</tr>
<tr id="row1084513362123"><td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p33972541493"><a name="p33972541493"></a><a name="p33972541493"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.3 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="8.239176082391761%" headers="mcps1.2.8.1.4 "><p id="p339716540919"><a name="p339716540919"></a><a name="p339716540919"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="15.568443155684433%" headers="mcps1.2.8.1.5 "><p id="p1739717541895"><a name="p1739717541895"></a><a name="p1739717541895"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.728627137286272%" headers="mcps1.2.8.1.6 "><p id="p12397054697"><a name="p12397054697"></a><a name="p12397054697"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="23.807619238076192%" headers="mcps1.2.8.1.7 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间</p>
</td>
</tr>
</tbody>
</table>

**表 2**  allocation\_pool对象

<a name="table24611730"></a>
<table><thead align="left"><tr id="row15154020"><th class="cellrowborder" valign="top" width="16.491649164916492%" id="mcps1.2.6.1.1"><p id="p19516075"><a name="p19516075"></a><a name="p19516075"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="17.16171617161716%" id="mcps1.2.6.1.2"><p id="p37298263"><a name="p37298263"></a><a name="p37298263"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="15.831583158315832%" id="mcps1.2.6.1.3"><p id="p1260496"><a name="p1260496"></a><a name="p1260496"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="14.431443144314432%" id="mcps1.2.6.1.4"><p id="p34991357"><a name="p34991357"></a><a name="p34991357"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="36.08360836083608%" id="mcps1.2.6.1.5"><p id="p15727687"><a name="p15727687"></a><a name="p15727687"></a>备注</p>
</th>
</tr>
</thead>
<tbody><tr id="row7331458"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.6.1.1 "><p id="p56977217"><a name="p56977217"></a><a name="p56977217"></a>start</p>
</td>
<td class="cellrowborder" valign="top" width="17.16171617161716%" headers="mcps1.2.6.1.2 "><p id="p51751889"><a name="p51751889"></a><a name="p51751889"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="15.831583158315832%" headers="mcps1.2.6.1.3 "><p id="p31153498"><a name="p31153498"></a><a name="p31153498"></a>合法的IP地址</p>
</td>
<td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.6.1.4 "><p id="p40405379"><a name="p40405379"></a><a name="p40405379"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="36.08360836083608%" headers="mcps1.2.6.1.5 "><p id="p51610228"><a name="p51610228"></a><a name="p51610228"></a>网络池起始IP</p>
</td>
</tr>
<tr id="row61838871"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.6.1.1 "><p id="p42892680"><a name="p42892680"></a><a name="p42892680"></a>end</p>
</td>
<td class="cellrowborder" valign="top" width="17.16171617161716%" headers="mcps1.2.6.1.2 "><p id="p51755094"><a name="p51755094"></a><a name="p51755094"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="15.831583158315832%" headers="mcps1.2.6.1.3 "><p id="p31413096"><a name="p31413096"></a><a name="p31413096"></a>合法的IP地址</p>
</td>
<td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.6.1.4 "><p id="p61432871"><a name="p61432871"></a><a name="p61432871"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="36.08360836083608%" headers="mcps1.2.6.1.5 "><p id="p10006650"><a name="p10006650"></a><a name="p10006650"></a>网络池结束IP</p>
</td>
</tr>
</tbody>
</table>

**表 3**  host\_route对象

<a name="table5232330"></a>
<table><thead align="left"><tr id="row65973637"><th class="cellrowborder" valign="top" width="16.491649164916492%" id="mcps1.2.6.1.1"><p id="p42264412"><a name="p42264412"></a><a name="p42264412"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="16.971697169716972%" id="mcps1.2.6.1.2"><p id="p865310"><a name="p865310"></a><a name="p865310"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.021602160216023%" id="mcps1.2.6.1.3"><p id="p2981301"><a name="p2981301"></a><a name="p2981301"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="14.431443144314432%" id="mcps1.2.6.1.4"><p id="p40158857"><a name="p40158857"></a><a name="p40158857"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="36.08360836083608%" id="mcps1.2.6.1.5"><p id="p31641985"><a name="p31641985"></a><a name="p31641985"></a>备注</p>
</th>
</tr>
</thead>
<tbody><tr id="row16342414"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.6.1.1 "><p id="p48667192"><a name="p48667192"></a><a name="p48667192"></a>destination</p>
</td>
<td class="cellrowborder" valign="top" width="16.971697169716972%" headers="mcps1.2.6.1.2 "><p id="p49728507"><a name="p49728507"></a><a name="p49728507"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="16.021602160216023%" headers="mcps1.2.6.1.3 "><p id="p1477246"><a name="p1477246"></a><a name="p1477246"></a>合法的CIDR格式</p>
</td>
<td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.6.1.4 "><p id="p52548073"><a name="p52548073"></a><a name="p52548073"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="36.08360836083608%" headers="mcps1.2.6.1.5 "><p id="p28535525"><a name="p28535525"></a><a name="p28535525"></a>路由目的子网</p>
</td>
</tr>
<tr id="row55493137"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.6.1.1 "><p id="p65759080"><a name="p65759080"></a><a name="p65759080"></a>nexthop</p>
</td>
<td class="cellrowborder" valign="top" width="16.971697169716972%" headers="mcps1.2.6.1.2 "><p id="p24885284"><a name="p24885284"></a><a name="p24885284"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="16.021602160216023%" headers="mcps1.2.6.1.3 "><p id="p2442157"><a name="p2442157"></a><a name="p2442157"></a>合法的IP地址</p>
</td>
<td class="cellrowborder" valign="top" width="14.431443144314432%" headers="mcps1.2.6.1.4 "><p id="p63597034"><a name="p63597034"></a><a name="p63597034"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="36.08360836083608%" headers="mcps1.2.6.1.5 "><p id="p51086148"><a name="p51086148"></a><a name="p51086148"></a>路由下一跳IP</p>
</td>
</tr>
</tbody>
</table>

