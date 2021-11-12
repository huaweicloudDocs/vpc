# 创建网络ACL组<a name="vpc_firewall_0015"></a>

## 功能介绍<a name="section28317954132753"></a>

创建网络ACL组。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=NeutronCreateFirewallGroup)中直接运行调试该接口。

## URI<a name="section55587849132753"></a>

POST /v2.0/fwaas/firewall\_groups

## 请求消息<a name="section28981251132753"></a>

**表 1**  请求参数

<a name="table23322114132753"></a>
<table><thead align="left"><tr id="row65935357132753"><th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.1"><p id="p47877448132753"><a name="p47877448132753"></a><a name="p47877448132753"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p52491337132753"><a name="p52491337132753"></a><a name="p52491337132753"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p45667362132753"><a name="p45667362132753"></a><a name="p45667362132753"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p17633266132753"><a name="p17633266132753"></a><a name="p17633266132753"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8939225132753"><td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.1 "><p id="p59896822132753"><a name="p59896822132753"></a><a name="p59896822132753"></a>firewall_group</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p49917547132753"><a name="p49917547132753"></a><a name="p49917547132753"></a><a href="#table31629250121127">firewall_group </a>object</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p64285015132753"><a name="p64285015132753"></a><a name="p64285015132753"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p48871362132652"><a name="p48871362132652"></a><a name="p48871362132652"></a>firewall group对象列表。请参见<a href="#table31629250121127">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Firewall Group对象

<a name="table31629250121127"></a>
<table><thead align="left"><tr id="row45711693121127"><th class="cellrowborder" valign="top" width="26.897310268973108%" id="mcps1.2.5.1.1"><p id="p46819705121127"><a name="p46819705121127"></a><a name="p46819705121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="13.268673132686734%" id="mcps1.2.5.1.2"><p id="p8500055165416"><a name="p8500055165416"></a><a name="p8500055165416"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.948005199480054%" id="mcps1.2.5.1.3"><p id="p35064605121127"><a name="p35064605121127"></a><a name="p35064605121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.88601139886011%" id="mcps1.2.5.1.4"><p id="p11952850121127"><a name="p11952850121127"></a><a name="p11952850121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row34896104121127"><td class="cellrowborder" valign="top" width="26.897310268973108%" headers="mcps1.2.5.1.1 "><p id="p52608071121127"><a name="p52608071121127"></a><a name="p52608071121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.268673132686734%" headers="mcps1.2.5.1.2 "><p id="p1500355195417"><a name="p1500355195417"></a><a name="p1500355195417"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.948005199480054%" headers="mcps1.2.5.1.3 "><p id="p59846605121127"><a name="p59846605121127"></a><a name="p59846605121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.88601139886011%" headers="mcps1.2.5.1.4 "><p id="p28604909121127"><a name="p28604909121127"></a><a name="p28604909121127"></a><span id="text1856811267512"><a name="text1856811267512"></a><a name="text1856811267512"></a>网络ACL</span><span id="text356842645110"><a name="text356842645110"></a><a name="text356842645110"></a></span>组名称。</p>
<p id="p83231610195414"><a name="p83231610195414"></a><a name="p83231610195414"></a>使用说明：最长255个字符</p>
</td>
</tr>
<tr id="row11129246121127"><td class="cellrowborder" valign="top" width="26.897310268973108%" headers="mcps1.2.5.1.1 "><p id="p39887063121127"><a name="p39887063121127"></a><a name="p39887063121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13.268673132686734%" headers="mcps1.2.5.1.2 "><p id="p1450085505420"><a name="p1450085505420"></a><a name="p1450085505420"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.948005199480054%" headers="mcps1.2.5.1.3 "><p id="p28745735121127"><a name="p28745735121127"></a><a name="p28745735121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.88601139886011%" headers="mcps1.2.5.1.4 "><p id="p35639020121127"><a name="p35639020121127"></a><a name="p35639020121127"></a><span id="text11660929105113"><a name="text11660929105113"></a><a name="text11660929105113"></a>网络ACL</span><span id="text15661122911516"><a name="text15661122911516"></a><a name="text15661122911516"></a></span>组描述。</p>
<p id="p11817162215413"><a name="p11817162215413"></a><a name="p11817162215413"></a>使用说明：最长255个字符</p>
</td>
</tr>
<tr id="row38137474121127"><td class="cellrowborder" valign="top" width="26.897310268973108%" headers="mcps1.2.5.1.1 "><p id="p35500294121127"><a name="p35500294121127"></a><a name="p35500294121127"></a>ingress_firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.268673132686734%" headers="mcps1.2.5.1.2 "><p id="p3500155520543"><a name="p3500155520543"></a><a name="p3500155520543"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.948005199480054%" headers="mcps1.2.5.1.3 "><p id="p49995809121127"><a name="p49995809121127"></a><a name="p49995809121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.88601139886011%" headers="mcps1.2.5.1.4 "><p id="p56499442121127"><a name="p56499442121127"></a><a name="p56499442121127"></a>入方向<span id="text18036326518"><a name="text18036326518"></a><a name="text18036326518"></a>网络ACL</span><span id="text1880319322517"><a name="text1880319322517"></a><a name="text1880319322517"></a></span>策略。</p>
</td>
</tr>
<tr id="row9094936121127"><td class="cellrowborder" valign="top" width="26.897310268973108%" headers="mcps1.2.5.1.1 "><p id="p34911245121127"><a name="p34911245121127"></a><a name="p34911245121127"></a>egress_firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.268673132686734%" headers="mcps1.2.5.1.2 "><p id="p1950085514546"><a name="p1950085514546"></a><a name="p1950085514546"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.948005199480054%" headers="mcps1.2.5.1.3 "><p id="p44624490121127"><a name="p44624490121127"></a><a name="p44624490121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.88601139886011%" headers="mcps1.2.5.1.4 "><p id="p37100641121127"><a name="p37100641121127"></a><a name="p37100641121127"></a>出方向<span id="text14841435175115"><a name="text14841435175115"></a><a name="text14841435175115"></a>网络ACL</span><span id="text084163505119"><a name="text084163505119"></a><a name="text084163505119"></a></span>策略。</p>
</td>
</tr>
<tr id="row31622902121127"><td class="cellrowborder" valign="top" width="26.897310268973108%" headers="mcps1.2.5.1.1 "><p id="p65911012121127"><a name="p65911012121127"></a><a name="p65911012121127"></a>ports</p>
</td>
<td class="cellrowborder" valign="top" width="13.268673132686734%" headers="mcps1.2.5.1.2 "><p id="p8500855175412"><a name="p8500855175412"></a><a name="p8500855175412"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.948005199480054%" headers="mcps1.2.5.1.3 "><p id="p5459978121127"><a name="p5459978121127"></a><a name="p5459978121127"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="39.88601139886011%" headers="mcps1.2.5.1.4 "><p id="p61002567121127"><a name="p61002567121127"></a><a name="p61002567121127"></a><span id="text4597143820518"><a name="text4597143820518"></a><a name="text4597143820518"></a>网络ACL</span><span id="text105974382513"><a name="text105974382513"></a><a name="text105974382513"></a></span>组绑定的端口列表。</p>
<p id="p10668102685116"><a name="p10668102685116"></a><a name="p10668102685116"></a>使用说明：必须为分布式router端口的id</p>
</td>
</tr>
<tr id="row59833296121127"><td class="cellrowborder" valign="top" width="26.897310268973108%" headers="mcps1.2.5.1.1 "><p id="p44051842121127"><a name="p44051842121127"></a><a name="p44051842121127"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="13.268673132686734%" headers="mcps1.2.5.1.2 "><p id="p3500455195415"><a name="p3500455195415"></a><a name="p3500455195415"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.948005199480054%" headers="mcps1.2.5.1.3 "><p id="p58587899121127"><a name="p58587899121127"></a><a name="p58587899121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="39.88601139886011%" headers="mcps1.2.5.1.4 "><p id="p3428646121127"><a name="p3428646121127"></a><a name="p3428646121127"></a><span id="text1660615480515"><a name="text1660615480515"></a><a name="text1660615480515"></a>网络ACL</span><span id="text160604815112"><a name="text160604815112"></a><a name="text160604815112"></a></span>是否受管理员控制。</p>
<p id="p19344243185411"><a name="p19344243185411"></a><a name="p19344243185411"></a>取值范围：true/false</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section47249684132753"></a>

**表 3**  响应参数

<a name="table22528036132753"></a>
<table><thead align="left"><tr id="row54420002132753"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p43836262132753"><a name="p43836262132753"></a><a name="p43836262132753"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p57315890132753"><a name="p57315890132753"></a><a name="p57315890132753"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p55101661132753"><a name="p55101661132753"></a><a name="p55101661132753"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row23789310132753"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p30981925132753"><a name="p30981925132753"></a><a name="p30981925132753"></a>firewall_group</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p1451635132753"><a name="p1451635132753"></a><a name="p1451635132753"></a><a href="#table7886851182616">firewall_group </a>object</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p47442693132753"><a name="p47442693132753"></a><a name="p47442693132753"></a>firewall group对象列表。请参见<a href="#table7886851182616">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  Firewall Group对象

<a name="table7886851182616"></a>
<table><thead align="left"><tr id="row388711511267"><th class="cellrowborder" valign="top" width="35.3%" id="mcps1.2.4.1.1"><p id="p4887205152611"><a name="p4887205152611"></a><a name="p4887205152611"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="21.57%" id="mcps1.2.4.1.2"><p id="p288711516264"><a name="p288711516264"></a><a name="p288711516264"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.13%" id="mcps1.2.4.1.3"><p id="p12887651122618"><a name="p12887651122618"></a><a name="p12887651122618"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row20395689121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p50168503121127"><a name="p50168503121127"></a><a name="p50168503121127"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p47513116121127"><a name="p47513116121127"></a><a name="p47513116121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p62072725121127"><a name="p62072725121127"></a><a name="p62072725121127"></a><span id="text15331135615518"><a name="text15331135615518"></a><a name="text15331135615518"></a>网络ACL</span><span id="text83311656195111"><a name="text83311656195111"></a><a name="text83311656195111"></a></span>组的uuid标识。</p>
</td>
</tr>
<tr id="row788715512269"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p6887105192617"><a name="p6887105192617"></a><a name="p6887105192617"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p12887175111264"><a name="p12887175111264"></a><a name="p12887175111264"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p4889105118269"><a name="p4889105118269"></a><a name="p4889105118269"></a><span id="text679152165211"><a name="text679152165211"></a><a name="text679152165211"></a>网络ACL</span><span id="text107910216527"><a name="text107910216527"></a><a name="text107910216527"></a></span>组名称。</p>
</td>
</tr>
<tr id="row1288910518269"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p148891451162617"><a name="p148891451162617"></a><a name="p148891451162617"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p15889125111262"><a name="p15889125111262"></a><a name="p15889125111262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p688975152619"><a name="p688975152619"></a><a name="p688975152619"></a><span id="text111312685215"><a name="text111312685215"></a><a name="text111312685215"></a>网络ACL</span><span id="text313186125212"><a name="text313186125212"></a><a name="text313186125212"></a></span>组描述。</p>
</td>
</tr>
<tr id="row677472121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p60717947121127"><a name="p60717947121127"></a><a name="p60717947121127"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p65871708121127"><a name="p65871708121127"></a><a name="p65871708121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row16889175115261"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p6889155182616"><a name="p6889155182616"></a><a name="p6889155182616"></a>ingress_firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p198896511262"><a name="p198896511262"></a><a name="p198896511262"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p7890105182610"><a name="p7890105182610"></a><a name="p7890105182610"></a>入方向<span id="text450191018521"><a name="text450191018521"></a><a name="text450191018521"></a>网络ACL</span><span id="text45012100527"><a name="text45012100527"></a><a name="text45012100527"></a></span>策略。</p>
</td>
</tr>
<tr id="row118901051122618"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p189075119263"><a name="p189075119263"></a><a name="p189075119263"></a>egress_firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p1989075152620"><a name="p1989075152620"></a><a name="p1989075152620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p489045192610"><a name="p489045192610"></a><a name="p489045192610"></a>出方向<span id="text199135135523"><a name="text199135135523"></a><a name="text199135135523"></a>网络ACL</span><span id="text17913513165220"><a name="text17913513165220"></a><a name="text17913513165220"></a></span>策略。</p>
</td>
</tr>
<tr id="row11890165162618"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p889075115268"><a name="p889075115268"></a><a name="p889075115268"></a>ports</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p38902051102616"><a name="p38902051102616"></a><a name="p38902051102616"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p148906511265"><a name="p148906511265"></a><a name="p148906511265"></a><span id="text82802017175214"><a name="text82802017175214"></a><a name="text82802017175214"></a>网络ACL</span><span id="text62801617175215"><a name="text62801617175215"></a><a name="text62801617175215"></a></span>组绑定的端口列表。</p>
</td>
</tr>
<tr id="row48186031121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p33368479121127"><a name="p33368479121127"></a><a name="p33368479121127"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p7938198121127"><a name="p7938198121127"></a><a name="p7938198121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p56166201121127"><a name="p56166201121127"></a><a name="p56166201121127"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row60912436121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p66273781121127"><a name="p66273781121127"></a><a name="p66273781121127"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p7141533121127"><a name="p7141533121127"></a><a name="p7141533121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p6468335121127"><a name="p6468335121127"></a><a name="p6468335121127"></a><span id="text3644182385210"><a name="text3644182385210"></a><a name="text3644182385210"></a>网络ACL</span><span id="text26441623105214"><a name="text26441623105214"></a><a name="text26441623105214"></a></span>策略的状态。</p>
</td>
</tr>
<tr id="row9890155162614"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p1889085142618"><a name="p1889085142618"></a><a name="p1889085142618"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p10890551152617"><a name="p10890551152617"></a><a name="p10890551152617"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p5890115118263"><a name="p5890115118263"></a><a name="p5890115118263"></a><span id="text14443827165214"><a name="text14443827165214"></a><a name="text14443827165214"></a>网络ACL</span><span id="text8443122705220"><a name="text8443122705220"></a><a name="text8443122705220"></a></span>是否受管理员控制。</p>
</td>
</tr>
<tr id="row7228115213486"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p53071912134918"><a name="p53071912134918"></a><a name="p53071912134918"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p1731011220498"><a name="p1731011220498"></a><a name="p1731011220498"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p555515419297"><a name="p555515419297"></a><a name="p555515419297"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row1933393255913"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间，UTC时间</p>
<p id="p65980291419"><a name="p65980291419"></a><a name="p65980291419"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row62318369590"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间，UTC时间</p>
<p id="p15297192516128"><a name="p15297192516128"></a><a name="p15297192516128"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section59424075132753"></a>

请求样例

```
POST https://{Endpoint}/v2.0/fwaas/firewall_groups

{
    "firewall_group": {
        "ingress_firewall_policy_id": "afc52ce9-5305-4ec9-9feb-44feb8330341", 
        "ports": [
            "c133f2bf-6937-4416-bb17-012e1be5cd2d"
        ]
    }
}
```

响应样例

```
{
    "firewall_group": {
        "status": "PENDING_CREATE", 
        "public": false, 
        "egress_firewall_policy_id": null, 
        "name": "", 
        "admin_state_up": true, 
        "ports": [
            "c133f2bf-6937-4416-bb17-012e1be5cd2d"
        ], 
        "tenant_id": "23c8a121505047b6869edf39f3062712", 
        "id": "0415f554-26ed-44e7-a881-bdf4e6216e38", 
        "ingress_firewall_policy_id": "afc52ce9-5305-4ec9-9feb-44feb8330341", 
        "description": "",
        "project_id": "23c8a121505047b6869edf39f3062712",
        "created_at": "2018-09-12T08:24:14",
        "updated_at": "2018-09-12T08:24:14"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

