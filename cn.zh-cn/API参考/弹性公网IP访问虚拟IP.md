# 弹性公网IP访问虚拟IP<a name="vpc_vip_0003"></a>

## 使用工具<a name="section84221635191520"></a>

Postman或者JMeter。

## 前提条件<a name="section14439239153017"></a>

已经参考[典型组网](虚拟IP简介.md#zh-cn_topic_0095139658_section4160174715811)进行云服务器组网配置，确保云服务器已经绑定虚拟IP。

## 涉及接口<a name="section1186811971613"></a>

涉及2个API接口的调用，具体如下：

<a name="table72072528317"></a>
<table><thead align="left"><tr id="row112761952173116"><th class="cellrowborder" valign="top" width="11.551155115511552%" id="mcps1.1.5.1.1"><p id="p182763520319"><a name="p182763520319"></a><a name="p182763520319"></a>序号</p>
</th>
<th class="cellrowborder" valign="top" width="11.551155115511552%" id="mcps1.1.5.1.2"><p id="p1027655263119"><a name="p1027655263119"></a><a name="p1027655263119"></a>方法</p>
</th>
<th class="cellrowborder" valign="top" width="39.39393939393939%" id="mcps1.1.5.1.3"><p id="p127825211313"><a name="p127825211313"></a><a name="p127825211313"></a>URI</p>
</th>
<th class="cellrowborder" valign="top" width="37.503750375037505%" id="mcps1.1.5.1.4"><p id="p8278135243114"><a name="p8278135243114"></a><a name="p8278135243114"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row127817520314"><td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.1 "><p id="p5278552193119"><a name="p5278552193119"></a><a name="p5278552193119"></a>1</p>
</td>
<td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.2 "><p id="p14278155283111"><a name="p14278155283111"></a><a name="p14278155283111"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.5.1.3 "><p id="p227814526319"><a name="p227814526319"></a><a name="p227814526319"></a>/v3/auth/tokens</p>
</td>
<td class="cellrowborder" valign="top" width="37.503750375037505%" headers="mcps1.1.5.1.4 "><p id="p7278352113111"><a name="p7278352113111"></a><a name="p7278352113111"></a>获取Token，参见<a href="https://support.huaweicloud.com/api-iam/iam_30_0001.html" target="_blank" rel="noopener noreferrer">获取用户Token</a></p>
</td>
</tr>
<tr id="row527895243115"><td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.1 "><p id="p72781552183112"><a name="p72781552183112"></a><a name="p72781552183112"></a>2</p>
</td>
<td class="cellrowborder" valign="top" width="11.551155115511552%" headers="mcps1.1.5.1.2 "><p id="p1527885273110"><a name="p1527885273110"></a><a name="p1527885273110"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.5.1.3 "><p id="p52781952103115"><a name="p52781952103115"></a><a name="p52781952103115"></a>/v2.0/floatingips</p>
</td>
<td class="cellrowborder" valign="top" width="37.503750375037505%" headers="mcps1.1.5.1.4 "><p id="p5278952173117"><a name="p5278952173117"></a><a name="p5278952173117"></a>创建弹性公网IP，参见<a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0008.html" target="_blank" rel="noopener noreferrer">创建浮动IP</a></p>
</td>
</tr>
</tbody>
</table>

## 操作步骤<a name="section1294414993011"></a>

1.  获取token。

    <a name="vpc_vip_0002_table16457194412177"></a>
    <table><thead align="left"><tr id="vpc_vip_0002_row164541444181716"><th class="cellrowborder" valign="top" width="30.53%" id="mcps1.1.3.1.1"><p id="vpc_vip_0002_p12454104411178"><a name="vpc_vip_0002_p12454104411178"></a><a name="vpc_vip_0002_p12454104411178"></a>方法</p>
    </th>
    <th class="cellrowborder" valign="top" width="69.47%" id="mcps1.1.3.1.2"><p id="vpc_vip_0002_p1445424413176"><a name="vpc_vip_0002_p1445424413176"></a><a name="vpc_vip_0002_p1445424413176"></a>POST</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="vpc_vip_0002_row1145611441173"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="vpc_vip_0002_p2456124401714"><a name="vpc_vip_0002_p2456124401714"></a><a name="vpc_vip_0002_p2456124401714"></a>url</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="vpc_vip_0002_p9456144413177"><a name="vpc_vip_0002_p9456144413177"></a><a name="vpc_vip_0002_p9456144413177"></a>iam地址:端口/v3/auth/tokens</p>
    </td>
    </tr>
    <tr id="vpc_vip_0002_row124575445176"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="vpc_vip_0002_p1745694471716"><a name="vpc_vip_0002_p1745694471716"></a><a name="vpc_vip_0002_p1745694471716"></a>body体（样例）</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="vpc_vip_0002_p7456444181714"><a name="vpc_vip_0002_p7456444181714"></a><a name="vpc_vip_0002_p7456444181714"></a>{</p>
    <p id="vpc_vip_0002_p1745620445176"><a name="vpc_vip_0002_p1745620445176"></a><a name="vpc_vip_0002_p1745620445176"></a>"auth":{</p>
    <p id="vpc_vip_0002_p745619441179"><a name="vpc_vip_0002_p745619441179"></a><a name="vpc_vip_0002_p745619441179"></a>"identity":{</p>
    <p id="vpc_vip_0002_p24561444173"><a name="vpc_vip_0002_p24561444173"></a><a name="vpc_vip_0002_p24561444173"></a>"methods": ["password"],</p>
    <p id="vpc_vip_0002_p54561944181720"><a name="vpc_vip_0002_p54561944181720"></a><a name="vpc_vip_0002_p54561944181720"></a>"password":{</p>
    <p id="vpc_vip_0002_p12456114415175"><a name="vpc_vip_0002_p12456114415175"></a><a name="vpc_vip_0002_p12456114415175"></a>"user":{</p>
    <p id="vpc_vip_0002_p1145694417174"><a name="vpc_vip_0002_p1145694417174"></a><a name="vpc_vip_0002_p1145694417174"></a>"name": "<em id="vpc_vip_0002_i11456134491717"><a name="vpc_vip_0002_i11456134491717"></a><a name="vpc_vip_0002_i11456134491717"></a>user_name</em>",</p>
    <p id="vpc_vip_0002_p13456444191717"><a name="vpc_vip_0002_p13456444191717"></a><a name="vpc_vip_0002_p13456444191717"></a>"domain":{</p>
    <p id="vpc_vip_0002_p12456644141713"><a name="vpc_vip_0002_p12456644141713"></a><a name="vpc_vip_0002_p12456644141713"></a>"name":"<em id="vpc_vip_0002_i1445684401718"><a name="vpc_vip_0002_i1445684401718"></a><a name="vpc_vip_0002_i1445684401718"></a>domain_name</em>"</p>
    <p id="vpc_vip_0002_p845618441175"><a name="vpc_vip_0002_p845618441175"></a><a name="vpc_vip_0002_p845618441175"></a>},</p>
    <p id="vpc_vip_0002_p18456144415173"><a name="vpc_vip_0002_p18456144415173"></a><a name="vpc_vip_0002_p18456144415173"></a>"password":"<em id="vpc_vip_0002_i104569447179"><a name="vpc_vip_0002_i104569447179"></a><a name="vpc_vip_0002_i104569447179"></a>user_password</em>"</p>
    <p id="vpc_vip_0002_p1745604471712"><a name="vpc_vip_0002_p1745604471712"></a><a name="vpc_vip_0002_p1745604471712"></a>}</p>
    <p id="vpc_vip_0002_p7456204413171"><a name="vpc_vip_0002_p7456204413171"></a><a name="vpc_vip_0002_p7456204413171"></a>}</p>
    <p id="vpc_vip_0002_p0457154412173"><a name="vpc_vip_0002_p0457154412173"></a><a name="vpc_vip_0002_p0457154412173"></a>},</p>
    <p id="vpc_vip_0002_p54573440175"><a name="vpc_vip_0002_p54573440175"></a><a name="vpc_vip_0002_p54573440175"></a>"scope":{</p>
    <p id="vpc_vip_0002_p15457344191719"><a name="vpc_vip_0002_p15457344191719"></a><a name="vpc_vip_0002_p15457344191719"></a>"project":{</p>
    <p id="vpc_vip_0002_p10457114451715"><a name="vpc_vip_0002_p10457114451715"></a><a name="vpc_vip_0002_p10457114451715"></a>"name":"<em id="vpc_vip_0002_i194571044191719"><a name="vpc_vip_0002_i194571044191719"></a><a name="vpc_vip_0002_i194571044191719"></a>project_name</em>"</p>
    <p id="vpc_vip_0002_p6457104441710"><a name="vpc_vip_0002_p6457104441710"></a><a name="vpc_vip_0002_p6457104441710"></a>}</p>
    <p id="vpc_vip_0002_p12457044101712"><a name="vpc_vip_0002_p12457044101712"></a><a name="vpc_vip_0002_p12457044101712"></a>}</p>
    <p id="vpc_vip_0002_p16457114420175"><a name="vpc_vip_0002_p16457114420175"></a><a name="vpc_vip_0002_p16457114420175"></a>}</p>
    <p id="vpc_vip_0002_p18457144441710"><a name="vpc_vip_0002_p18457144441710"></a><a name="vpc_vip_0002_p18457144441710"></a>}</p>
    </td>
    </tr>
    </tbody>
    </table>

2.  创建弹性公网IP绑定虚拟IP。

    <a name="table77261142183613"></a>
    <table><thead align="left"><tr id="row1576384211365"><th class="cellrowborder" valign="top" width="30.53%" id="mcps1.1.3.1.1"><p id="p6763154213612"><a name="p6763154213612"></a><a name="p6763154213612"></a>方法</p>
    </th>
    <th class="cellrowborder" valign="top" width="69.47%" id="mcps1.1.3.1.2"><p id="p15763042203617"><a name="p15763042203617"></a><a name="p15763042203617"></a>POST</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row16763114273613"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p147632426363"><a name="p147632426363"></a><a name="p147632426363"></a>url</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p13763242183610"><a name="p13763242183610"></a><a name="p13763242183610"></a>vpc地址:端口/v2.0/floatingips</p>
    </td>
    </tr>
    <tr id="row176304293619"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p117632042123612"><a name="p117632042123612"></a><a name="p117632042123612"></a>body体（样例）</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p4763342163620"><a name="p4763342163620"></a><a name="p4763342163620"></a>{</p>
    <p id="p97631242163611"><a name="p97631242163611"></a><a name="p97631242163611"></a>"floatingip": {</p>
    <p id="p1776314223614"><a name="p1776314223614"></a><a name="p1776314223614"></a>"floating_network_id": "<em id="i1776344215364"><a name="i1776344215364"></a><a name="i1776344215364"></a>${admin_external_net}</em>",</p>
    <p id="p476394219366"><a name="p476394219366"></a><a name="p476394219366"></a>"port_id": "4b9246da-aa12-4959-b17e-84038b8a0a96"</p>
    <p id="p18763142123618"><a name="p18763142123618"></a><a name="p18763142123618"></a>}</p>
    <p id="p7763164211366"><a name="p7763164211366"></a><a name="p7763164211366"></a>}</p>
    </td>
    </tr>
    <tr id="row97631421365"><td class="cellrowborder" valign="top" width="30.53%" headers="mcps1.1.3.1.1 "><p id="p2076304218369"><a name="p2076304218369"></a><a name="p2076304218369"></a>说明</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.47%" headers="mcps1.1.3.1.2 "><p id="p147631842163611"><a name="p147631842163611"></a><a name="p147631842163611"></a>body体中的参数port_id为云服务器绑定的虚拟IP对应的VIP Port的ID</p>
    </td>
    </tr>
    </tbody>
    </table>


