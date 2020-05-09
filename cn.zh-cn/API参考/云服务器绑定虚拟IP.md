# 云服务器绑定虚拟IP<a name="vpc_vip_0002"></a>

## 使用工具<a name="section84221635191520"></a>

Postman或者JMeter。

## 涉及接口<a name="section1186811971613"></a>

涉及5个API接口的调用，具体如下：

<a name="table168745398162"></a>
<table><thead align="left"><tr id="row19436398160"><th class="cellrowborder" valign="top" width="11.551155115511552%" id="mcps1.1.5.1.1"><p id="p179435399163"><a name="p179435399163"></a><a name="p179435399163"></a>序号</p>
</th>
<th class="cellrowborder" valign="top" width="11.551155115511552%" id="mcps1.1.5.1.2"><p id="p1594333913163"><a name="p1594333913163"></a><a name="p1594333913163"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="39.39393939393939%" id="mcps1.1.5.1.3"><p id="p1594313393168"><a name="p1594313393168"></a><a name="p1594313393168"></a>URI</p>
</th>
<th class="cellrowborder" valign="top" width="37.503750375037505%" id="mcps1.1.5.1.4"><p id="p1394314392161"><a name="p1394314392161"></a><a name="p1394314392161"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row169431839161613"><td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.1 "><p id="p8943113916168"><a name="p8943113916168"></a><a name="p8943113916168"></a>1</p>
</td>
<td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.2 "><p id="p1294419392161"><a name="p1294419392161"></a><a name="p1294419392161"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.5.1.3 "><p id="p109441639171611"><a name="p109441639171611"></a><a name="p109441639171611"></a>/v3/auth/tokens</p>
</td>
<td class="cellrowborder" valign="top" width="37.503750375037505%" headers="mcps1.1.5.1.4 "><p id="p17145201412357"><a name="p17145201412357"></a><a name="p17145201412357"></a>获取Token，参见<a href="https://support.huaweicloud.com/api-iam/iam_30_0001.html" target="_blank" rel="noopener noreferrer">获取用户Token</a></p>
</td>
</tr>
<tr id="row119449396168"><td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.1 "><p id="p1694413961611"><a name="p1694413961611"></a><a name="p1694413961611"></a>2</p>
</td>
<td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.2 "><p id="p6944173951611"><a name="p6944173951611"></a><a name="p6944173951611"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.5.1.3 "><p id="p1394413916168"><a name="p1394413916168"></a><a name="p1394413916168"></a>/v2.0/ports</p>
</td>
<td class="cellrowborder" valign="top" width="37.503750375037505%" headers="mcps1.1.5.1.4 "><p id="p1043655243511"><a name="p1043655243511"></a><a name="p1043655243511"></a>创建VIP Port，参见<a href="创建端口-openstack.md">创建端口</a></p>
</td>
</tr>
<tr id="row109441939121617"><td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.1 "><p id="p8944339151619"><a name="p8944339151619"></a><a name="p8944339151619"></a>3</p>
</td>
<td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.2 "><p id="p11944143981610"><a name="p11944143981610"></a><a name="p11944143981610"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.5.1.3 "><p id="p189448392169"><a name="p189448392169"></a><a name="p189448392169"></a>/v2.0/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="37.503750375037505%" headers="mcps1.1.5.1.4 "><p id="p1794453901617"><a name="p1794453901617"></a><a name="p1794453901617"></a>将云服务器与虚拟IP绑定，参见<a href="更新端口-openstack.md">更新端口</a></p>
</td>
</tr>
<tr id="row1594423941613"><td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.1 "><p id="p79441139181620"><a name="p79441139181620"></a><a name="p79441139181620"></a>4</p>
</td>
<td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.2 "><p id="p694413971616"><a name="p694413971616"></a><a name="p694413971616"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.5.1.3 "><p id="p179441439101616"><a name="p179441439101616"></a><a name="p179441439101616"></a>/v2/{project_id}/servers/{server_id}/os-interface</p>
</td>
<td class="cellrowborder" valign="top" width="37.503750375037505%" headers="mcps1.1.5.1.4 "><p id="p139447393169"><a name="p139447393169"></a><a name="p139447393169"></a>配置绑定了虚拟IP的云服务器网卡的allowed-address-pairs，</p>
</td>
</tr>
</tbody>
</table>

## 操作步骤<a name="section9913818131612"></a>

1.  获取token。

    <a name="table16457194412177"></a>
    <table><thead align="left"><tr id="row164541444181716"><th class="cellrowborder" valign="top" width="30.53%" id="mcps1.1.3.1.1"><p id="p12454104411178"><a name="p12454104411178"></a><a name="p12454104411178"></a>方法</p>
    </th>
    <th class="cellrowborder" valign="top" width="69.47%" id="mcps1.1.3.1.2"><p id="p1445424413176"><a name="p1445424413176"></a><a name="p1445424413176"></a>POST</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1145611441173"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p2456124401714"><a name="p2456124401714"></a><a name="p2456124401714"></a>url</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p9456144413177"><a name="p9456144413177"></a><a name="p9456144413177"></a>iam地址:端口/v3/auth/tokens</p>
    </td>
    </tr>
    <tr id="row124575445176"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p1745694471716"><a name="p1745694471716"></a><a name="p1745694471716"></a>body体（样例）</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p7456444181714"><a name="p7456444181714"></a><a name="p7456444181714"></a>{</p>
    <p id="p1745620445176"><a name="p1745620445176"></a><a name="p1745620445176"></a>"auth":{</p>
    <p id="p745619441179"><a name="p745619441179"></a><a name="p745619441179"></a>"identity":{</p>
    <p id="p24561444173"><a name="p24561444173"></a><a name="p24561444173"></a>"methods": ["password"],</p>
    <p id="p54561944181720"><a name="p54561944181720"></a><a name="p54561944181720"></a>"password":{</p>
    <p id="p12456114415175"><a name="p12456114415175"></a><a name="p12456114415175"></a>"user":{</p>
    <p id="p1145694417174"><a name="p1145694417174"></a><a name="p1145694417174"></a>"name": "<em id="i11456134491717"><a name="i11456134491717"></a><a name="i11456134491717"></a>user_name</em>",</p>
    <p id="p13456444191717"><a name="p13456444191717"></a><a name="p13456444191717"></a>"domain":{</p>
    <p id="p12456644141713"><a name="p12456644141713"></a><a name="p12456644141713"></a>"name":"<em id="i1445684401718"><a name="i1445684401718"></a><a name="i1445684401718"></a>domain_name</em>"</p>
    <p id="p845618441175"><a name="p845618441175"></a><a name="p845618441175"></a>},</p>
    <p id="p18456144415173"><a name="p18456144415173"></a><a name="p18456144415173"></a>"password":"<em id="i104569447179"><a name="i104569447179"></a><a name="i104569447179"></a>user_password</em>"</p>
    <p id="p1745604471712"><a name="p1745604471712"></a><a name="p1745604471712"></a>}</p>
    <p id="p7456204413171"><a name="p7456204413171"></a><a name="p7456204413171"></a>}</p>
    <p id="p0457154412173"><a name="p0457154412173"></a><a name="p0457154412173"></a>},</p>
    <p id="p54573440175"><a name="p54573440175"></a><a name="p54573440175"></a>"scope":{</p>
    <p id="p15457344191719"><a name="p15457344191719"></a><a name="p15457344191719"></a>"project":{</p>
    <p id="p10457114451715"><a name="p10457114451715"></a><a name="p10457114451715"></a>"name":"<em id="i194571044191719"><a name="i194571044191719"></a><a name="i194571044191719"></a>project_name</em>"</p>
    <p id="p6457104441710"><a name="p6457104441710"></a><a name="p6457104441710"></a>}</p>
    <p id="p12457044101712"><a name="p12457044101712"></a><a name="p12457044101712"></a>}</p>
    <p id="p16457114420175"><a name="p16457114420175"></a><a name="p16457114420175"></a>}</p>
    <p id="p18457144441710"><a name="p18457144441710"></a><a name="p18457144441710"></a>}</p>
    </td>
    </tr>
    </tbody>
    </table>

2.  在云服务器所在的VPC子网内，创建VIP Port。

    要求VIP Port与云服务器同子网，并指定“device\_owner”参数为“neutron:VIP\_PORT”。

    <a name="table798125810210"></a>
    <table><thead align="left"><tr id="row11361158162114"><th class="cellrowborder" valign="top" width="30.53%" id="mcps1.1.3.1.1"><p id="p01361558102115"><a name="p01361558102115"></a><a name="p01361558102115"></a>方法</p>
    </th>
    <th class="cellrowborder" valign="top" width="69.47%" id="mcps1.1.3.1.2"><p id="p15136155819216"><a name="p15136155819216"></a><a name="p15136155819216"></a>POST</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row9136165842119"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p91361458162116"><a name="p91361458162116"></a><a name="p91361458162116"></a>url</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p161366587218"><a name="p161366587218"></a><a name="p161366587218"></a>vpc地址:端口/v2.0/ports</p>
    </td>
    </tr>
    <tr id="row6136155812212"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p19136358112116"><a name="p19136358112116"></a><a name="p19136358112116"></a>body体（样例）</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p2136145814216"><a name="p2136145814216"></a><a name="p2136145814216"></a>{</p>
    <p id="p1113616584215"><a name="p1113616584215"></a><a name="p1113616584215"></a>"port": {</p>
    <p id="p61361658142113"><a name="p61361658142113"></a><a name="p61361658142113"></a>"network_id": "a54e1b19-ce78-4b7e-b28b-d2d716cdc161",</p>
    <p id="p1813655810219"><a name="p1813655810219"></a><a name="p1813655810219"></a>"device_owner": "neutron:VIP_PORT",</p>
    <p id="p913612589211"><a name="p913612589211"></a><a name="p913612589211"></a>"name": "vip_port_test"</p>
    <p id="p2136258152114"><a name="p2136258152114"></a><a name="p2136258152114"></a>}</p>
    <p id="p15136125810211"><a name="p15136125810211"></a><a name="p15136125810211"></a>}</p>
    </td>
    </tr>
    <tr id="row6136155822110"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p1513618580215"><a name="p1513618580215"></a><a name="p1513618580215"></a>说明</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p1713614586213"><a name="p1713614586213"></a><a name="p1713614586213"></a>body体中的network_id为云服务器所在的网络ID</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  将云服务器与虚拟IP绑定。

    更新vip port的allowed-address-pairs，指定ip\_address为需要绑定的云服务器的网卡的IP地址。

    <a name="table1079115092213"></a>
    <table><thead align="left"><tr id="row16869850122218"><th class="cellrowborder" valign="top" width="31%" id="mcps1.1.3.1.1"><p id="p11869950132211"><a name="p11869950132211"></a><a name="p11869950132211"></a>方法</p>
    </th>
    <th class="cellrowborder" valign="top" width="69%" id="mcps1.1.3.1.2"><p id="p586925017225"><a name="p586925017225"></a><a name="p586925017225"></a>PUT</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row286912506222"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.1.3.1.1 "><p id="p1386925017228"><a name="p1386925017228"></a><a name="p1386925017228"></a>url</p>
    </td>
    <td class="cellrowborder" valign="top" width="69%" headers="mcps1.1.3.1.2 "><p id="p13869135013220"><a name="p13869135013220"></a><a name="p13869135013220"></a>vpc地址:端口/v2.0/ports/{port_id}</p>
    </td>
    </tr>
    <tr id="row2869145062215"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.1.3.1.1 "><p id="p108691508222"><a name="p108691508222"></a><a name="p108691508222"></a>body体（样例）</p>
    </td>
    <td class="cellrowborder" valign="top" width="69%" headers="mcps1.1.3.1.2 "><p id="p188691501220"><a name="p188691501220"></a><a name="p188691501220"></a>{</p>
    <p id="p1686995018227"><a name="p1686995018227"></a><a name="p1686995018227"></a>"port": {</p>
    <p id="p118696509229"><a name="p118696509229"></a><a name="p118696509229"></a>"allowed_address_pairs": [</p>
    <p id="p178691450152216"><a name="p178691450152216"></a><a name="p178691450152216"></a>{"ip_address":"192.168.22.221"},</p>
    <p id="p138691250132218"><a name="p138691250132218"></a><a name="p138691250132218"></a>{"ip_address":"192.168.22.203"}</p>
    <p id="p486919505229"><a name="p486919505229"></a><a name="p486919505229"></a>]</p>
    <p id="p188691950142218"><a name="p188691950142218"></a><a name="p188691950142218"></a>}</p>
    <p id="p9869650102213"><a name="p9869650102213"></a><a name="p9869650102213"></a>}</p>
    </td>
    </tr>
    <tr id="row13869145016221"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.1.3.1.1 "><p id="p28691050122211"><a name="p28691050122211"></a><a name="p28691050122211"></a>说明</p>
    </td>
    <td class="cellrowborder" valign="top" width="69%" headers="mcps1.1.3.1.2 "><a name="ul68971018182320"></a><a name="ul68971018182320"></a><ul id="ul68971018182320"><li>url中{port_id}是上一步中创建的vip port的ID</li><li>body体中ip_address就是需要绑定的云服务器网卡的IP地址</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

4.  配置绑定了虚拟IP的云服务器网卡的allowed-address-pairs。
    1.  获取绑定了虚拟IP的云服务器网卡信息。

        <a name="table541261532510"></a>
        <table><thead align="left"><tr id="row12447191512252"><th class="cellrowborder" valign="top" width="30.53%" id="mcps1.1.3.1.1"><p id="p74471415122518"><a name="p74471415122518"></a><a name="p74471415122518"></a>方法</p>
        </th>
        <th class="cellrowborder" valign="top" width="69.47%" id="mcps1.1.3.1.2"><p id="p944731515252"><a name="p944731515252"></a><a name="p944731515252"></a>GET</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="row114471215172520"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p1744741532513"><a name="p1744741532513"></a><a name="p1744741532513"></a>url</p>
        </td>
        <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p11447101510259"><a name="p11447101510259"></a><a name="p11447101510259"></a>ecs地址:端口/v2/{tenant_id}/servers/{server_id}/os-interface</p>
        </td>
        </tr>
        <tr id="row244713153255"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p15447161518259"><a name="p15447161518259"></a><a name="p15447161518259"></a>body体</p>
        </td>
        <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p164471715102513"><a name="p164471715102513"></a><a name="p164471715102513"></a>不涉及</p>
        </td>
        </tr>
        <tr id="row184471815172517"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p2044711519258"><a name="p2044711519258"></a><a name="p2044711519258"></a>说明</p>
        </td>
        <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p3448181513253"><a name="p3448181513253"></a><a name="p3448181513253"></a>url中{tenant_id}是项目ID，{server_id}是云服务器的ID</p>
        </td>
        </tr>
        </tbody>
        </table>

    2.  更新云服务器网卡的allowed-address-pairs为1.1.1.1/0，关闭源/目的检查。

        <a name="table424494318250"></a>
        <table><thead align="left"><tr id="row122889436257"><th class="cellrowborder" valign="top" width="30.53%" id="mcps1.1.3.1.1"><p id="p72882043142512"><a name="p72882043142512"></a><a name="p72882043142512"></a>方法</p>
        </th>
        <th class="cellrowborder" valign="top" width="69.47%" id="mcps1.1.3.1.2"><p id="p328864362516"><a name="p328864362516"></a><a name="p328864362516"></a>PUT</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="row15288104318254"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p15288543202512"><a name="p15288543202512"></a><a name="p15288543202512"></a>url</p>
        </td>
        <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p828824332512"><a name="p828824332512"></a><a name="p828824332512"></a>vpc地址:端口/v2.0/ports/{port_id}</p>
        </td>
        </tr>
        <tr id="row1528816430253"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p1228864382510"><a name="p1228864382510"></a><a name="p1228864382510"></a>body体</p>
        </td>
        <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p9288164342517"><a name="p9288164342517"></a><a name="p9288164342517"></a>{</p>
        <p id="p1529016438258"><a name="p1529016438258"></a><a name="p1529016438258"></a>"port": {</p>
        <p id="p19290643152519"><a name="p19290643152519"></a><a name="p19290643152519"></a>"allowed_address_pairs": [</p>
        <p id="p0290174313251"><a name="p0290174313251"></a><a name="p0290174313251"></a>{"ip_address":"1.1.1.1/0"}</p>
        <p id="p4290143192512"><a name="p4290143192512"></a><a name="p4290143192512"></a>]</p>
        <p id="p3290134372513"><a name="p3290134372513"></a><a name="p3290134372513"></a>}</p>
        <p id="p8290943122517"><a name="p8290943122517"></a><a name="p8290943122517"></a>}</p>
        </td>
        </tr>
        <tr id="row929054311259"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p14290154362517"><a name="p14290154362517"></a><a name="p14290154362517"></a>说明</p>
        </td>
        <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p72901143142512"><a name="p72901143142512"></a><a name="p72901143142512"></a>url中{port_id}是绑定了虚拟IP的云服务器网卡的ID</p>
        </td>
        </tr>
        </tbody>
        </table>



