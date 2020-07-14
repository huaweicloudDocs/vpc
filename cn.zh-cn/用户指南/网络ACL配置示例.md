# 网络ACL配置示例<a name="acl_0002"></a>

介绍常见的网络ACL配置示例。

-   [拒绝特定端口访问](#section11312173319432)
-   [允许某些协议端口的访问](#section61291659102216)

## 拒绝特定端口访问<a name="section11312173319432"></a>

在本示例中，假设要防止勒索病毒Wanna Cry的攻击，需要隔离具有漏洞的应用端口，例如TCP 445端口。您可以在子网层级添加网络ACL拒绝规则，拒绝所有对TCP 445端口的入站访问。

**网络ACL配置**

需要添加的入方向规则如[表1](#table553618145582)所示。

**表 1**  网络ACL规则

<a name="table553618145582"></a>
<table><thead align="left"><tr id="row1536191465810"><th class="cellrowborder" valign="top" width="7.26%" id="mcps1.2.9.1.1"><p id="p6536131425817"><a name="p6536131425817"></a><a name="p6536131425817"></a>方向</p>
</th>
<th class="cellrowborder" valign="top" width="5.779999999999999%" id="mcps1.2.9.1.2"><p id="p1253641416587"><a name="p1253641416587"></a><a name="p1253641416587"></a>动作</p>
</th>
<th class="cellrowborder" valign="top" width="6.859999999999999%" id="mcps1.2.9.1.3"><p id="p5536171415817"><a name="p5536171415817"></a><a name="p5536171415817"></a>协议</p>
</th>
<th class="cellrowborder" valign="top" width="8.93%" id="mcps1.2.9.1.4"><p id="p853691455815"><a name="p853691455815"></a><a name="p853691455815"></a>源地址</p>
</th>
<th class="cellrowborder" valign="top" width="13.950000000000001%" id="mcps1.2.9.1.5"><p id="p8536114165813"><a name="p8536114165813"></a><a name="p8536114165813"></a>源端口范围</p>
</th>
<th class="cellrowborder" valign="top" width="15.75%" id="mcps1.2.9.1.6"><p id="p15536181495819"><a name="p15536181495819"></a><a name="p15536181495819"></a>目的地址</p>
</th>
<th class="cellrowborder" valign="top" width="14.06%" id="mcps1.2.9.1.7"><p id="p135361214105818"><a name="p135361214105818"></a><a name="p135361214105818"></a>目的端口范围</p>
</th>
<th class="cellrowborder" valign="top" width="27.41%" id="mcps1.2.9.1.8"><p id="p85369147584"><a name="p85369147584"></a><a name="p85369147584"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row12341947141113"><td class="cellrowborder" valign="top" width="7.26%" headers="mcps1.2.9.1.1 "><p id="p173271575112"><a name="p173271575112"></a><a name="p173271575112"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="5.779999999999999%" headers="mcps1.2.9.1.2 "><p id="p09375481311"><a name="p09375481311"></a><a name="p09375481311"></a>允许</p>
</td>
<td class="cellrowborder" valign="top" width="6.859999999999999%" headers="mcps1.2.9.1.3 "><p id="p234294719114"><a name="p234294719114"></a><a name="p234294719114"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="8.93%" headers="mcps1.2.9.1.4 "><p id="p441232491318"><a name="p441232491318"></a><a name="p441232491318"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="13.950000000000001%" headers="mcps1.2.9.1.5 "><p id="p14135242137"><a name="p14135242137"></a><a name="p14135242137"></a>1-65535</p>
</td>
<td class="cellrowborder" valign="top" width="15.75%" headers="mcps1.2.9.1.6 "><p id="p13413152415134"><a name="p13413152415134"></a><a name="p13413152415134"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="14.06%" headers="mcps1.2.9.1.7 "><p id="p434204741117"><a name="p434204741117"></a><a name="p434204741117"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="27.41%" headers="mcps1.2.9.1.8 "><p id="p153421247191118"><a name="p153421247191118"></a><a name="p153421247191118"></a>放通所有入站流量</p>
</td>
</tr>
<tr id="row20536131455815"><td class="cellrowborder" valign="top" width="7.26%" headers="mcps1.2.9.1.1 "><p id="p175361814165817"><a name="p175361814165817"></a><a name="p175361814165817"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="5.779999999999999%" headers="mcps1.2.9.1.2 "><p id="p1053616146583"><a name="p1053616146583"></a><a name="p1053616146583"></a>拒绝</p>
</td>
<td class="cellrowborder" valign="top" width="6.859999999999999%" headers="mcps1.2.9.1.3 "><p id="p453651419586"><a name="p453651419586"></a><a name="p453651419586"></a>TCP</p>
</td>
<td class="cellrowborder" valign="top" width="8.93%" headers="mcps1.2.9.1.4 "><p id="p153691419583"><a name="p153691419583"></a><a name="p153691419583"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="13.950000000000001%" headers="mcps1.2.9.1.5 "><p id="p5536181412589"><a name="p5536181412589"></a><a name="p5536181412589"></a>1-65535</p>
</td>
<td class="cellrowborder" valign="top" width="15.75%" headers="mcps1.2.9.1.6 "><p id="p8536171495815"><a name="p8536171495815"></a><a name="p8536171495815"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="14.06%" headers="mcps1.2.9.1.7 "><p id="p65360144584"><a name="p65360144584"></a><a name="p65360144584"></a>445</p>
</td>
<td class="cellrowborder" valign="top" width="27.41%" headers="mcps1.2.9.1.8 "><p id="p13536614155813"><a name="p13536614155813"></a><a name="p13536614155813"></a>拒绝所有IP地址通过TCP 445端口入站访问</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>网络ACL默认拒绝所有入站流量，需先放通所有入站流量。

## 允许某些协议端口的访问<a name="section61291659102216"></a>

在本示例中，假设子网内的某个弹性云服务器做Web服务器，入方向需要放通HTTP 80和HTTPS 443端口，出方向全部放通。当子网开启网络ACL时，需要同时配置网络ACL和安全组规则。

**网络ACL配置**

需要添加的网络ACL入方向、出方向规则如[表2](#table195634095313)所示。

**表 2**  网络ACL规则

<a name="table195634095313"></a>
<table><thead align="left"><tr id="row56214055319"><th class="cellrowborder" valign="top" width="7.26%" id="mcps1.2.9.1.1"><p id="p16212405538"><a name="p16212405538"></a><a name="p16212405538"></a>方向</p>
</th>
<th class="cellrowborder" valign="top" width="5.779999999999999%" id="mcps1.2.9.1.2"><p id="p1863340165319"><a name="p1863340165319"></a><a name="p1863340165319"></a>动作</p>
</th>
<th class="cellrowborder" valign="top" width="6.859999999999999%" id="mcps1.2.9.1.3"><p id="p10631640155318"><a name="p10631640155318"></a><a name="p10631640155318"></a>协议</p>
</th>
<th class="cellrowborder" valign="top" width="8.93%" id="mcps1.2.9.1.4"><p id="p66324013535"><a name="p66324013535"></a><a name="p66324013535"></a>源地址</p>
</th>
<th class="cellrowborder" valign="top" width="13.950000000000001%" id="mcps1.2.9.1.5"><p id="p1659407534"><a name="p1659407534"></a><a name="p1659407534"></a>源端口范围</p>
</th>
<th class="cellrowborder" valign="top" width="15.75%" id="mcps1.2.9.1.6"><p id="p56554075310"><a name="p56554075310"></a><a name="p56554075310"></a>目的地址</p>
</th>
<th class="cellrowborder" valign="top" width="14.06%" id="mcps1.2.9.1.7"><p id="p106694013537"><a name="p106694013537"></a><a name="p106694013537"></a>目的端口范围</p>
</th>
<th class="cellrowborder" valign="top" width="27.41%" id="mcps1.2.9.1.8"><p id="p66717405533"><a name="p66717405533"></a><a name="p66717405533"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row196712405536"><td class="cellrowborder" valign="top" width="7.26%" headers="mcps1.2.9.1.1 "><p id="p069124055316"><a name="p069124055316"></a><a name="p069124055316"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="5.779999999999999%" headers="mcps1.2.9.1.2 "><p id="p1670204016533"><a name="p1670204016533"></a><a name="p1670204016533"></a>允许</p>
</td>
<td class="cellrowborder" valign="top" width="6.859999999999999%" headers="mcps1.2.9.1.3 "><p id="p117112409536"><a name="p117112409536"></a><a name="p117112409536"></a>TCP</p>
</td>
<td class="cellrowborder" valign="top" width="8.93%" headers="mcps1.2.9.1.4 "><p id="p10721240185320"><a name="p10721240185320"></a><a name="p10721240185320"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="13.950000000000001%" headers="mcps1.2.9.1.5 "><p id="p7742404539"><a name="p7742404539"></a><a name="p7742404539"></a>1-65535</p>
</td>
<td class="cellrowborder" valign="top" width="15.75%" headers="mcps1.2.9.1.6 "><p id="p177484025315"><a name="p177484025315"></a><a name="p177484025315"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="14.06%" headers="mcps1.2.9.1.7 "><p id="p1211320362012"><a name="p1211320362012"></a><a name="p1211320362012"></a>80</p>
</td>
<td class="cellrowborder" valign="top" width="27.41%" headers="mcps1.2.9.1.8 "><p id="p3772407536"><a name="p3772407536"></a><a name="p3772407536"></a>允许所有IP地址通过HTTP协议入站访问子网内的弹性云服务器的80端口</p>
</td>
</tr>
<tr id="row160981135413"><td class="cellrowborder" valign="top" width="7.26%" headers="mcps1.2.9.1.1 "><p id="p11609119544"><a name="p11609119544"></a><a name="p11609119544"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="5.779999999999999%" headers="mcps1.2.9.1.2 "><p id="p960910113543"><a name="p960910113543"></a><a name="p960910113543"></a>允许</p>
</td>
<td class="cellrowborder" valign="top" width="6.859999999999999%" headers="mcps1.2.9.1.3 "><p id="p96091313540"><a name="p96091313540"></a><a name="p96091313540"></a>TCP</p>
</td>
<td class="cellrowborder" valign="top" width="8.93%" headers="mcps1.2.9.1.4 "><p id="p12609616544"><a name="p12609616544"></a><a name="p12609616544"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="13.950000000000001%" headers="mcps1.2.9.1.5 "><p id="p1760910165412"><a name="p1760910165412"></a><a name="p1760910165412"></a>1-65535</p>
</td>
<td class="cellrowborder" valign="top" width="15.75%" headers="mcps1.2.9.1.6 "><p id="p136093175411"><a name="p136093175411"></a><a name="p136093175411"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="14.06%" headers="mcps1.2.9.1.7 "><p id="p9208174116114"><a name="p9208174116114"></a><a name="p9208174116114"></a>443</p>
</td>
<td class="cellrowborder" valign="top" width="27.41%" headers="mcps1.2.9.1.8 "><p id="p36241816183320"><a name="p36241816183320"></a><a name="p36241816183320"></a>允许所有IP地址通过HTTPS协议入站访问子网内的弹性云服务器的443端口</p>
</td>
</tr>
<tr id="row27210235717"><td class="cellrowborder" valign="top" width="7.26%" headers="mcps1.2.9.1.1 "><p id="p1372192105711"><a name="p1372192105711"></a><a name="p1372192105711"></a>出方向</p>
</td>
<td class="cellrowborder" valign="top" width="5.779999999999999%" headers="mcps1.2.9.1.2 "><p id="p16721823575"><a name="p16721823575"></a><a name="p16721823575"></a>允许</p>
</td>
<td class="cellrowborder" valign="top" width="6.859999999999999%" headers="mcps1.2.9.1.3 "><p id="p1372192145710"><a name="p1372192145710"></a><a name="p1372192145710"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="8.93%" headers="mcps1.2.9.1.4 "><p id="p204401137135716"><a name="p204401137135716"></a><a name="p204401137135716"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="13.950000000000001%" headers="mcps1.2.9.1.5 "><p id="p37211215719"><a name="p37211215719"></a><a name="p37211215719"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="15.75%" headers="mcps1.2.9.1.6 "><p id="p99971040195713"><a name="p99971040195713"></a><a name="p99971040195713"></a>0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="14.06%" headers="mcps1.2.9.1.7 "><p id="p1972114217575"><a name="p1972114217575"></a><a name="p1972114217575"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="27.41%" headers="mcps1.2.9.1.8 "><p id="p207214210578"><a name="p207214210578"></a><a name="p207214210578"></a>允许子网内所有出站流量的数据报文通过</p>
</td>
</tr>
</tbody>
</table>

**安全组配置**

需要添加的安全组入方向、出方向规则如[表3](#table30323767195135)所示。

**表 3**  安全组规则

<a name="table30323767195135"></a>
<table><thead align="left"><tr id="row15770184195135"><th class="cellrowborder" valign="top" width="10%" id="mcps1.2.6.1.1"><p id="p1235112172119"><a name="p1235112172119"></a><a name="p1235112172119"></a>方向</p>
</th>
<th class="cellrowborder" valign="top" width="14.330000000000002%" id="mcps1.2.6.1.2"><p id="p2316559195135"><a name="p2316559195135"></a><a name="p2316559195135"></a>协议/应用</p>
</th>
<th class="cellrowborder" valign="top" width="15.879999999999999%" id="mcps1.2.6.1.3"><p id="p32340552195135"><a name="p32340552195135"></a><a name="p32340552195135"></a>端口</p>
</th>
<th class="cellrowborder" valign="top" width="24.759999999999998%" id="mcps1.2.6.1.4"><p id="p2339084195135"><a name="p2339084195135"></a><a name="p2339084195135"></a>源地址/目的地址</p>
</th>
<th class="cellrowborder" valign="top" width="35.03%" id="mcps1.2.6.1.5"><p id="p1096519542911"><a name="p1096519542911"></a><a name="p1096519542911"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row55248116195135"><td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.6.1.1 "><p id="p153542182110"><a name="p153542182110"></a><a name="p153542182110"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="14.330000000000002%" headers="mcps1.2.6.1.2 "><p id="p45912425195135"><a name="p45912425195135"></a><a name="p45912425195135"></a>TCP</p>
</td>
<td class="cellrowborder" valign="top" width="15.879999999999999%" headers="mcps1.2.6.1.3 "><p id="p46840856195135"><a name="p46840856195135"></a><a name="p46840856195135"></a>80</p>
</td>
<td class="cellrowborder" valign="top" width="24.759999999999998%" headers="mcps1.2.6.1.4 "><p id="p36012962195135"><a name="p36012962195135"></a><a name="p36012962195135"></a>源地址：0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="35.03%" headers="mcps1.2.6.1.5 "><p id="p1616504613311"><a name="p1616504613311"></a><a name="p1616504613311"></a>允许所有IP地址通过HTTP协议入站访问安全组内的弹性云服务器的80端口</p>
</td>
</tr>
<tr id="row5566305020026"><td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.6.1.1 "><p id="p1335112162119"><a name="p1335112162119"></a><a name="p1335112162119"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="14.330000000000002%" headers="mcps1.2.6.1.2 "><p id="p3120540920026"><a name="p3120540920026"></a><a name="p3120540920026"></a>TCP</p>
</td>
<td class="cellrowborder" valign="top" width="15.879999999999999%" headers="mcps1.2.6.1.3 "><p id="p5665449220026"><a name="p5665449220026"></a><a name="p5665449220026"></a>443</p>
</td>
<td class="cellrowborder" valign="top" width="24.759999999999998%" headers="mcps1.2.6.1.4 "><p id="p2561110020026"><a name="p2561110020026"></a><a name="p2561110020026"></a>源地址：0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="35.03%" headers="mcps1.2.6.1.5 "><p id="p11273949183317"><a name="p11273949183317"></a><a name="p11273949183317"></a>允许所有IP地址通过HTTPS协议入站访问安全组内的弹性云服务器的443端口</p>
</td>
</tr>
<tr id="row711437142712"><td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.6.1.1 "><p id="p31141071272"><a name="p31141071272"></a><a name="p31141071272"></a>出方向</p>
</td>
<td class="cellrowborder" valign="top" width="14.330000000000002%" headers="mcps1.2.6.1.2 "><p id="p711457182715"><a name="p711457182715"></a><a name="p711457182715"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="15.879999999999999%" headers="mcps1.2.6.1.3 "><p id="p1011487182717"><a name="p1011487182717"></a><a name="p1011487182717"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="24.759999999999998%" headers="mcps1.2.6.1.4 "><p id="p20126774286"><a name="p20126774286"></a><a name="p20126774286"></a>目的地址：0.0.0.0/0</p>
</td>
<td class="cellrowborder" valign="top" width="35.03%" headers="mcps1.2.6.1.5 "><p id="p20965751299"><a name="p20965751299"></a><a name="p20965751299"></a>允许安全组内所有出站流量的数据报文通过</p>
</td>
</tr>
</tbody>
</table>

网络ACL相当于一个额外的保护层，就算不小心配置了比较宽松的安全组规则，网络ACL规则也仅允许HTTP 80和HTTPS 443的访问，拒绝其他的入站访问流量。

