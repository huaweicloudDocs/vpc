# 更新弹性公网IP<a name="ZH-CN_TOPIC_0020090600"></a>

## 功能介绍<a name="section43589445"></a>

更新弹性公网IP，将弹性公网IP跟一个网卡绑定或者解绑定，转换IP地址版本类型。

## URI<a name="section56760689"></a>

PUT /v1/\{project\_id\}/publicips/\{publicip\_id\}

**表 1**  参数说明

<a name="table25231885"></a>
<table><thead align="left"><tr id="row34804713"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p609510"><a name="p609510"></a><a name="p609510"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p49370368"><a name="p49370368"></a><a name="p49370368"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p39576862"><a name="p39576862"></a><a name="p39576862"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row51609257"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p19600264"><a name="p19600264"></a><a name="p19600264"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p44117540"><a name="p44117540"></a><a name="p44117540"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p16750948"><a name="p16750948"></a><a name="p16750948"></a>项目ID</p>
</td>
</tr>
<tr id="row16540805"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p64736823"><a name="p64736823"></a><a name="p64736823"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p9191297"><a name="p9191297"></a><a name="p9191297"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p6297612"><a name="p6297612"></a><a name="p6297612"></a>弹性公网IP唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section41084157"></a>

-   请求参数

    **表 2**  请求参数

    <a name="table46814673152226"></a>
    <table><thead align="left"><tr id="row46264343152226"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="p56424328152226"><a name="p56424328152226"></a><a name="p56424328152226"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="p6967894152226"><a name="p6967894152226"></a><a name="p6967894152226"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="p27528552152226"><a name="p27528552152226"></a><a name="p27528552152226"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.18%" id="mcps1.2.5.1.4"><p id="p15220263152226"><a name="p15220263152226"></a><a name="p15220263152226"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row24881786152226"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p2158794152226"><a name="p2158794152226"></a><a name="p2158794152226"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p40644606152226"><a name="p40644606152226"></a><a name="p40644606152226"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p3878783152226"><a name="p3878783152226"></a><a name="p3878783152226"></a><em id="i34909047152226"><a name="i34909047152226"></a><a name="i34909047152226"></a>字典数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p9060565152226"><a name="p9060565152226"></a><a name="p9060565152226"></a>弹性公网IP对象</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicip字段说明

    <a name="table23403840"></a>
    <table><thead align="left"><tr id="row4798296"><th class="cellrowborder" valign="top" width="30.830000000000002%" id="mcps1.2.5.1.1"><p id="p53117702"><a name="p53117702"></a><a name="p53117702"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.05%" id="mcps1.2.5.1.2"><p id="p7566645"><a name="p7566645"></a><a name="p7566645"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.29%" id="mcps1.2.5.1.3"><p id="p3809944218819"><a name="p3809944218819"></a><a name="p3809944218819"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.830000000000002%" id="mcps1.2.5.1.4"><p id="p8918541"><a name="p8918541"></a><a name="p8918541"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row51313205"><td class="cellrowborder" valign="top" width="30.830000000000002%" headers="mcps1.2.5.1.1 "><p id="p62728917"><a name="p62728917"></a><a name="p62728917"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.05%" headers="mcps1.2.5.1.2 "><p id="p47877526"><a name="p47877526"></a><a name="p47877526"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.29%" headers="mcps1.2.5.1.3 "><p id="p6615596018819"><a name="p6615596018819"></a><a name="p6615596018819"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.830000000000002%" headers="mcps1.2.5.1.4 "><a name="ul1580299162914"></a><a name="ul1580299162914"></a><ul id="ul1580299162914"><li>功能说明：端口id。</li><li>约束：必须是存在的端口id，如果不带该参数或者值为空时为解除绑定弹性公网IP，如果该端口不存在或端口已绑定弹性公网IP则会提示出错，和ip_version字段互斥，不能同时更新。</li></ul>
    </td>
    </tr>
    <tr id="row126751018141713"><td class="cellrowborder" valign="top" width="30.830000000000002%" headers="mcps1.2.5.1.1 "><p id="p23901530141713"><a name="p23901530141713"></a><a name="p23901530141713"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.05%" headers="mcps1.2.5.1.2 "><p id="p17391163017175"><a name="p17391163017175"></a><a name="p17391163017175"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.29%" headers="mcps1.2.5.1.3 "><p id="p13391130151713"><a name="p13391130151713"></a><a name="p13391130151713"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.830000000000002%" headers="mcps1.2.5.1.4 "><a name="ul181841019112919"></a><a name="ul181841019112919"></a><ul id="ul181841019112919"><li>功能说明：IP版本信息，取值范围是4和6</li><li>约束：必须是系统支持的IP版本类型，和port_id互斥，不能同时更新。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例1

    ```
    {
        "publicip": {
            "port_id": "f588ccfa-8750-4d7c-bf5d-2ede24414706"
        }
    }
    ```


-   请求样例2

    ```
    {
        "publicip": {
            "ip_version ": 6 
        }
    }
    ```


## 响应消息<a name="section34213098"></a>

-   响应参数

    **表 4**  响应参数

    <a name="table32985183152250"></a>
    <table><thead align="left"><tr id="row10178394152250"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p19143548152250"><a name="p19143548152250"></a><a name="p19143548152250"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="p40138407152250"><a name="p40138407152250"></a><a name="p40138407152250"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="p29985535152250"><a name="p29985535152250"></a><a name="p29985535152250"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12909284152250"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p39019069152250"><a name="p39019069152250"></a><a name="p39019069152250"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p50907501152250"><a name="p50907501152250"></a><a name="p50907501152250"></a><em id="i55514327152250"><a name="i55514327152250"></a><a name="i55514327152250"></a>字典数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p366643152250"><a name="p366643152250"></a><a name="p366643152250"></a>弹性公网IP对象</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  publicip字段说明

    <a name="table8539194"></a>
    <table><thead align="left"><tr id="row42488815"><th class="cellrowborder" valign="top" width="38.86388638863886%" id="mcps1.2.4.1.1"><p id="p19042013"><a name="p19042013"></a><a name="p19042013"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.272227222722275%" id="mcps1.2.4.1.2"><p id="p2601150518848"><a name="p2601150518848"></a><a name="p2601150518848"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.86388638863886%" id="mcps1.2.4.1.3"><p id="p45052529"><a name="p45052529"></a><a name="p45052529"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row25376232"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p42208903"><a name="p42208903"></a><a name="p42208903"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p2655713518848"><a name="p2655713518848"></a><a name="p2655713518848"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><p id="p37460321"><a name="p37460321"></a><a name="p37460321"></a>弹性公网IP唯一标识</p>
    </td>
    </tr>
    <tr id="row1598569"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p62375226"><a name="p62375226"></a><a name="p62375226"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p364429318848"><a name="p364429318848"></a><a name="p364429318848"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><a name="ul5685133914309"></a><a name="ul5685133914309"></a><ul id="ul5685133914309"><li>取值范围：<a name="ul1489181419541"></a><a name="ul1489181419541"></a><ul id="ul1489181419541"><li>冻结FREEZED</li><li>绑定失败BIND_ERROR</li><li>绑定中BINDING</li><li>释放中PENDING_DELETE</li><li>创建PENDING_CREATE</li><li>创建中NOTIFYING</li><li>释放中NOTIFY_DELETE</li><li>更新中PENDING_UPDATE</li><li>未绑定DOWN</li><li>绑定ACTIVE</li><li>绑定ELB</li><li>失败ERROR</li></ul>
    </li><li>功能说明：弹性公网IP的状态</li></ul>
    </td>
    </tr>
    <tr id="row25167636"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p25312629"><a name="p25312629"></a><a name="p25312629"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p2675231618848"><a name="p2675231618848"></a><a name="p2675231618848"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><p id="p1917007318915"><a name="p1917007318915"></a><a name="p1917007318915"></a>弹性公网IP的类型</p>
    </td>
    </tr>
    <tr id="row1842185815373"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p59108624"><a name="p59108624"></a><a name="p59108624"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p904808818330"><a name="p904808818330"></a><a name="p904808818330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><p id="p40237373"><a name="p40237373"></a><a name="p40237373"></a>IPv4时是申请到的弹性公网IP地址，IPv6时是IPv6地址对应的IPv4地址。</p>
    </td>
    </tr>
    <tr id="row038222319203"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p528793342011"><a name="p528793342011"></a><a name="p528793342011"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p19287333172016"><a name="p19287333172016"></a><a name="p19287333172016"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><p id="p42871033202017"><a name="p42871033202017"></a><a name="p42871033202017"></a>IPv4时无此字段，IPv6时为申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="row14131451183718"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p171101456172118"><a name="p171101456172118"></a><a name="p171101456172118"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p1811012569218"><a name="p1811012569218"></a><a name="p1811012569218"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><p id="p1211011564217"><a name="p1211011564217"></a><a name="p1211011564217"></a>IP版本信息，取值范围是4和6</p>
    </td>
    </tr>
    <tr id="row39702100"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p59318092152759"><a name="p59318092152759"></a><a name="p59318092152759"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p3226849118848"><a name="p3226849118848"></a><a name="p3226849118848"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><p id="p61132152152759"><a name="p61132152152759"></a><a name="p61132152152759"></a>端口id</p>
    </td>
    </tr>
    <tr id="row24390923"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p29507743"><a name="p29507743"></a><a name="p29507743"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p6361099618848"><a name="p6361099618848"></a><a name="p6361099618848"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><p id="p58343698"><a name="p58343698"></a><a name="p58343698"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row55331235"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p52645056"><a name="p52645056"></a><a name="p52645056"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p5221702118848"><a name="p5221702118848"></a><a name="p5221702118848"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><p id="p21156092"><a name="p21156092"></a><a name="p21156092"></a>弹性公网IP申请时间（UTC时间）</p>
    </td>
    </tr>
    <tr id="row56187107"><td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.1 "><p id="p54861794"><a name="p54861794"></a><a name="p54861794"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.272227222722275%" headers="mcps1.2.4.1.2 "><p id="p172027018848"><a name="p172027018848"></a><a name="p172027018848"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.86388638863886%" headers="mcps1.2.4.1.3 "><p id="p55011311"><a name="p55011311"></a><a name="p55011311"></a>带宽大小</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例1

    ```
    {
        "publicip": {
            "id": "f588ccfa-8750-4d7c-bf5d-2ede24414706",
            "status": "PENDING_UPDATE",
            "type": "5_bgp",
            "public_ip_address": "161.xx.xx.7",
            "port_id": "f588ccfa-8750-4d7c-bf5d-2ede24414706",
            "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
            "create_time": "2015-07-16 04:10:52",
            "bandwidth_size": 6,
            "ip_version": 4
        }
    }
    ```


-   响应样例2

    ```
    {
        "publicip": {
            "id": "f588ccfa-8750-4d7c-bf5d-2ede24414706",
            "status": "PENDING_UPDATE",
            "type": "5_bgp",
            "public_ip_address": "161.xx.xx.7",
            "public_ipv6_address": "2a00:xx.xx.xx::x:4833",
            "port_id": "f588ccfa-8750-4d7c-bf5d-2ede24414706",
            "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
            "create_time": "2015-07-16 04:10:52",
            "bandwidth_size": 6,
            "ip_version": 6
        }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

