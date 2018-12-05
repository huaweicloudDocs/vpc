# 网络API简介<a name="ZH-CN_TOPIC_0062223940"></a>

## 对象简介<a name="section23215317204921"></a>

对网络资源进行管理和操作，包括查询网络列表、创建网络、查询指定网络、删除网络以及更新网络等接口。

## 对象模型<a name="section51721924204921"></a>

**表 1**  network对象

<a name="table49902238182444"></a>
<table><thead align="left"><tr id="row27727643182444"><th class="cellrowborder" valign="top" width="14.948505149485051%" id="mcps1.2.8.1.1"><p id="p31346634182444"><a name="p31346634182444"></a><a name="p31346634182444"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="7.519248075192481%" id="mcps1.2.8.1.2"><p id="p4702855164210"><a name="p4702855164210"></a><a name="p4702855164210"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.078692130786921%" id="mcps1.2.8.1.3"><p id="p56049421182444"><a name="p56049421182444"></a><a name="p56049421182444"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.339066093390661%" id="mcps1.2.8.1.4"><p id="p43709261182444"><a name="p43709261182444"></a><a name="p43709261182444"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="13.078692130786921%" id="mcps1.2.8.1.5"><p id="p50789233182444"><a name="p50789233182444"></a><a name="p50789233182444"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="13.078692130786921%" id="mcps1.2.8.1.6"><p id="p20287202182444"><a name="p20287202182444"></a><a name="p20287202182444"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="28.957104289571046%" id="mcps1.2.8.1.7"><p id="p32650631182444"><a name="p32650631182444"></a><a name="p32650631182444"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row27455432182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p9297551182444"><a name="p9297551182444"></a><a name="p9297551182444"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p1970212553428"><a name="p1970212553428"></a><a name="p1970212553428"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p14904129182444"><a name="p14904129182444"></a><a name="p14904129182444"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p66383816182444"><a name="p66383816182444"></a><a name="p66383816182444"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p8380044182444"><a name="p8380044182444"></a><a name="p8380044182444"></a>ACTIVE</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p7694964182444"><a name="p7694964182444"></a><a name="p7694964182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p19312361182444"><a name="p19312361182444"></a><a name="p19312361182444"></a>网络状态，可以为ACTIVE，BUILD，DOWN或ERROR。</p>
</td>
</tr>
<tr id="row39593523182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p52958822182444"><a name="p52958822182444"></a><a name="p52958822182444"></a>subnets</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p1702125513424"><a name="p1702125513424"></a><a name="p1702125513424"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p61806169182444"><a name="p61806169182444"></a><a name="p61806169182444"></a>List(Uuid-str)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p40243764182444"><a name="p40243764182444"></a><a name="p40243764182444"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p38519456182444"><a name="p38519456182444"></a><a name="p38519456182444"></a>空列表</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p33068228182444"><a name="p33068228182444"></a><a name="p33068228182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p61280841182444"><a name="p61280841182444"></a><a name="p61280841182444"></a>网络关联的子网ID列表。</p>
<p id="p14656663182444"><a name="p14656663182444"></a><a name="p14656663182444"></a>一个network仅支持关联一个 subnet。</p>
</td>
</tr>
<tr id="row64801111182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p14398613182444"><a name="p14398613182444"></a><a name="p14398613182444"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p070215513423"><a name="p070215513423"></a><a name="p070215513423"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p25436971182444"><a name="p25436971182444"></a><a name="p25436971182444"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p47128770182444"><a name="p47128770182444"></a><a name="p47128770182444"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p59334017182444"><a name="p59334017182444"></a><a name="p59334017182444"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p41326097182444"><a name="p41326097182444"></a><a name="p41326097182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p59079578182444"><a name="p59079578182444"></a><a name="p59079578182444"></a>网络名称。</p>
<p id="p61954155182444"><a name="p61954155182444"></a><a name="p61954155182444"></a>name不能为admin_external_net。</p>
</td>
</tr>
<tr id="row20716483182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p313524182444"><a name="p313524182444"></a><a name="p313524182444"></a>router:external</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p14702165515421"><a name="p14702165515421"></a><a name="p14702165515421"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p25395478182444"><a name="p25395478182444"></a><a name="p25395478182444"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p43767824182444"><a name="p43767824182444"></a><a name="p43767824182444"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p55532875182444"><a name="p55532875182444"></a><a name="p55532875182444"></a>false</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p1869039182444"><a name="p1869039182444"></a><a name="p1869039182444"></a>true或false</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p17174434182444"><a name="p17174434182444"></a><a name="p17174434182444"></a>扩展属性：是否外部网络</p>
</td>
</tr>
<tr id="row48951951182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p5685084182444"><a name="p5685084182444"></a><a name="p5685084182444"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p1702155104218"><a name="p1702155104218"></a><a name="p1702155104218"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p57838641182444"><a name="p57838641182444"></a><a name="p57838641182444"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p54418359182444"><a name="p54418359182444"></a><a name="p54418359182444"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p45810965182444"><a name="p45810965182444"></a><a name="p45810965182444"></a>true</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p19700724182444"><a name="p19700724182444"></a><a name="p19700724182444"></a>true或false</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p52254844182444"><a name="p52254844182444"></a><a name="p52254844182444"></a>管理状态。</p>
<p id="p531550182444"><a name="p531550182444"></a><a name="p531550182444"></a>只支持true。</p>
</td>
</tr>
<tr id="row4783956182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p51956132182444"><a name="p51956132182444"></a><a name="p51956132182444"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p1070215554422"><a name="p1070215554422"></a><a name="p1070215554422"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p47697173182444"><a name="p47697173182444"></a><a name="p47697173182444"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p38265806182444"><a name="p38265806182444"></a><a name="p38265806182444"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p12522616182444"><a name="p12522616182444"></a><a name="p12522616182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p7699003182444"><a name="p7699003182444"></a><a name="p7699003182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p19639486182444"><a name="p19639486182444"></a><a name="p19639486182444"></a>项目ID。</p>
</td>
</tr>
<tr id="row42537647182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p22997365182444"><a name="p22997365182444"></a><a name="p22997365182444"></a>shared</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p7702205534214"><a name="p7702205534214"></a><a name="p7702205534214"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p50847313182444"><a name="p50847313182444"></a><a name="p50847313182444"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p24991656182444"><a name="p24991656182444"></a><a name="p24991656182444"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p11058276182444"><a name="p11058276182444"></a><a name="p11058276182444"></a>false</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p23305197182444"><a name="p23305197182444"></a><a name="p23305197182444"></a>true或false</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p8672810182444"><a name="p8672810182444"></a><a name="p8672810182444"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row31409028182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p61103330182444"><a name="p61103330182444"></a><a name="p61103330182444"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p167024554425"><a name="p167024554425"></a><a name="p167024554425"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p50422701182444"><a name="p50422701182444"></a><a name="p50422701182444"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p57706956182444"><a name="p57706956182444"></a><a name="p57706956182444"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p43751848182444"><a name="p43751848182444"></a><a name="p43751848182444"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p54238760182444"><a name="p54238760182444"></a><a name="p54238760182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p31263412182444"><a name="p31263412182444"></a><a name="p31263412182444"></a>网络的id</p>
<p id="p311313148445"><a name="p311313148445"></a><a name="p311313148445"></a>【使用说明】在查询网络列表时候非必选</p>
</td>
</tr>
<tr id="row62882662182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p60330876182444"><a name="p60330876182444"></a><a name="p60330876182444"></a>provider:network_type</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p870218554422"><a name="p870218554422"></a><a name="p870218554422"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p54962794182444"><a name="p54962794182444"></a><a name="p54962794182444"></a>String(32)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p22801369182444"><a name="p22801369182444"></a><a name="p22801369182444"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p34971633182444"><a name="p34971633182444"></a><a name="p34971633182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p51363945173446"><a name="p51363945173446"></a><a name="p51363945173446"></a>使用以下网络类型中的一种：vlan、vxlan、flat、local、gre、geneve</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p3680057182444"><a name="p3680057182444"></a><a name="p3680057182444"></a>扩展属性：网络类型（支持vxlan, geneve）。</p>
<p id="p33120518182444"><a name="p33120518182444"></a><a name="p33120518182444"></a> 租户只能创建geneve类型网络。</p>
</td>
</tr>
<tr id="row8468164182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p14832653182444"><a name="p14832653182444"></a><a name="p14832653182444"></a>availability_zone_hints</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p107027557424"><a name="p107027557424"></a><a name="p107027557424"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p60594206182444"><a name="p60594206182444"></a><a name="p60594206182444"></a>List&lt;String&gt;</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p9183648182444"><a name="p9183648182444"></a><a name="p9183648182444"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p5678010182444"><a name="p5678010182444"></a><a name="p5678010182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p57265685182444"><a name="p57265685182444"></a><a name="p57265685182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p8008921182444"><a name="p8008921182444"></a><a name="p8008921182444"></a>本网络的候选可用域，当前版本不支持可用域调度。</p>
</td>
</tr>
<tr id="row44742828182444"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p290489182444"><a name="p290489182444"></a><a name="p290489182444"></a>availability_zones</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p1670415554424"><a name="p1670415554424"></a><a name="p1670415554424"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p23529638182444"><a name="p23529638182444"></a><a name="p23529638182444"></a>List&lt;String&gt;</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p26852507182444"><a name="p26852507182444"></a><a name="p26852507182444"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p27569473182444"><a name="p27569473182444"></a><a name="p27569473182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p18534847182444"><a name="p18534847182444"></a><a name="p18534847182444"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p24927678182444"><a name="p24927678182444"></a><a name="p24927678182444"></a>本网络的可用域。</p>
</td>
</tr>
<tr id="row25641034212156"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p53737204212156"><a name="p53737204212156"></a><a name="p53737204212156"></a>port_security_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p17040552426"><a name="p17040552426"></a><a name="p17040552426"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p31320715212156"><a name="p31320715212156"></a><a name="p31320715212156"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p46767607212156"><a name="p46767607212156"></a><a name="p46767607212156"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p37398945212156"><a name="p37398945212156"></a><a name="p37398945212156"></a>true</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p20456304212156"><a name="p20456304212156"></a><a name="p20456304212156"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p34506445212156"><a name="p34506445212156"></a><a name="p34506445212156"></a>端口安全使能标记，如果不能使，则network下所有虚机的安全组和dhcp防欺骗不生效</p>
</td>
</tr>
<tr id="row421706155213"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p14217767523"><a name="p14217767523"></a><a name="p14217767523"></a>dns_domain</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p16704355134216"><a name="p16704355134216"></a><a name="p16704355134216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p22172685219"><a name="p22172685219"></a><a name="p22172685219"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p182174616529"><a name="p182174616529"></a><a name="p182174616529"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p1221818695218"><a name="p1221818695218"></a><a name="p1221818695218"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p17218186145219"><a name="p17218186145219"></a><a name="p17218186145219"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p021812614525"><a name="p021812614525"></a><a name="p021812614525"></a>默认内网DNS域地址，系统自动生成维护，不支持设置和更新</p>
</td>
</tr>
<tr id="row1312882941114"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p17700201411911"><a name="p17700201411911"></a><a name="p17700201411911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p15700614790"><a name="p15700614790"></a><a name="p15700614790"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p17000141292"><a name="p17000141292"></a><a name="p17000141292"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p1470010141396"><a name="p1470010141396"></a><a name="p1470010141396"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p870017141892"><a name="p870017141892"></a><a name="p870017141892"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p7700714691"><a name="p7700714691"></a><a name="p7700714691"></a>资源project_id</p>
</td>
</tr>
<tr id="row9120034101119"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p6953241598"><a name="p6953241598"></a><a name="p6953241598"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p6953441993"><a name="p6953441993"></a><a name="p6953441993"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p11953164120911"><a name="p11953164120911"></a><a name="p11953164120911"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p595314119912"><a name="p595314119912"></a><a name="p595314119912"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间</p>
</td>
</tr>
<tr id="row1542863714112"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>update<em id="i1514353764017"><a name="i1514353764017"></a><a name="i1514353764017"></a>d_at</em></p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p33972541493"><a name="p33972541493"></a><a name="p33972541493"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p339716540919"><a name="p339716540919"></a><a name="p339716540919"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p1739717541895"><a name="p1739717541895"></a><a name="p1739717541895"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p12397054697"><a name="p12397054697"></a><a name="p12397054697"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间</p>
</td>
</tr>
</tbody>
</table>

