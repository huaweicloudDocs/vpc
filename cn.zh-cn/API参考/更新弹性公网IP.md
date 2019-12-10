# 更新弹性公网IP<a name="ZH-CN_TOPIC_0201534286"></a>

## 功能介绍<a name="section43589445"></a>

更新弹性公网IP，将弹性公网IP跟一个网卡绑定或者解绑定，转换IP地址版本类型。

## URI<a name="section56760689"></a>

PUT /v1/\{project\_id\}/publicips/\{publicip\_id\}

参数说明请参见[表1](#table25231885)。

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
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
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
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p3878783152226"><a name="p3878783152226"></a><a name="p3878783152226"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p9060565152226"><a name="p9060565152226"></a><a name="p9060565152226"></a>弹性公网IP对象，请参见<a href="#table23403840">表3</a>。</p>
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
    <td class="cellrowborder" valign="top" width="17.29%" headers="mcps1.2.5.1.3 "><p id="p13391130151713"><a name="p13391130151713"></a><a name="p13391130151713"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.830000000000002%" headers="mcps1.2.5.1.4 "><a name="ul181841019112919"></a><a name="ul181841019112919"></a><ul id="ul181841019112919"><li>功能说明：IP版本信息。</li><li>取值范围：4和6<a name="ul9525142083711"></a><a name="ul9525142083711"></a><ul id="ul9525142083711"><li>4：IPv4</li><li>6：IPv6</li></ul>
    </li><li>约束：<a name="ul11875851417"></a><a name="ul11875851417"></a><ul id="ul11875851417"><li>必须是系统支持的IP版本类型</li><li>和port_id互斥：不能同时设置port_id和ip_version字段。</li></ul>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例1（EIP绑定一张网卡）

    ```
    PUT https://{Endpoint}/v1/{project_id}/publicips/{publicip_id}
    
    {
        "publicip": {
            "port_id": "f588ccfa-8750-4d7c-bf5d-2ede24414706"
        }
    }
    ```


-   请求样例2（转换为IPv6 EIP）

    ```
    PUT https://{Endpoint}/v1/{project_id}/publicips/{publicip_id}
    
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
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p50907501152250"><a name="p50907501152250"></a><a name="p50907501152250"></a><em id="i1810218131512"><a name="i1810218131512"></a><a name="i1810218131512"></a>Object</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p366643152250"><a name="p366643152250"></a><a name="p366643152250"></a>弹性公网IP对象，请参见<a href="#table83964341880">表5</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  publicips字段说明

    <a name="table83964341880"></a>
    <table><thead align="left"><tr id="row608739661880"><th class="cellrowborder" valign="top" width="36.046395360463954%" id="mcps1.2.4.1.1"><p id="p318442431880"><a name="p318442431880"></a><a name="p318442431880"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.90720927907209%" id="mcps1.2.4.1.2"><p id="p201897271880"><a name="p201897271880"></a><a name="p201897271880"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="36.046395360463954%" id="mcps1.2.4.1.3"><p id="p247551571880"><a name="p247551571880"></a><a name="p247551571880"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row590107001880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p151373871880"><a name="p151373871880"></a><a name="p151373871880"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p623914921880"><a name="p623914921880"></a><a name="p623914921880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p205460611880"><a name="p205460611880"></a><a name="p205460611880"></a>弹性公网IP唯一标识</p>
    </td>
    </tr>
    <tr id="row506968211880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p128018091880"><a name="p128018091880"></a><a name="p128018091880"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p394853281880"><a name="p394853281880"></a><a name="p394853281880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul263945115243"></a><a name="ul263945115243"></a><ul id="ul263945115243"><li>功能说明：弹性公网IP的状态</li><li>取值范围：<a name="ul7905205815810"></a><a name="ul7905205815810"></a><ul id="ul7905205815810"><li>FREEZED：冻结</li><li>BIND_ERROR：绑定失败</li><li>BINDING：绑定中</li><li>PENDING_DELETE：释放中</li><li>PENDING_CREATE：创建中</li><li>PENDING_UPDATE：更新中</li><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ELB：绑定ELB</li><li>ERROR：异常失败</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row16130133562319"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p09743162419"><a name="p09743162419"></a><a name="p09743162419"></a>profile</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p12971231132410"><a name="p12971231132410"></a><a name="p12971231132410"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p5644118182514"><a name="p5644118182514"></a><a name="p5644118182514"></a>功能说明：额外参数，包括订单id、产品id等信息，详情请参见<a href="#table66651219193417">表6</a>。</p>
    <p id="p16644118152519"><a name="p16644118152519"></a><a name="p16644118152519"></a>约束：如果profile不为空，说明是包周期的弹性公网IP</p>
    </td>
    </tr>
    <tr id="row230260811880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p30749271"><a name="p30749271"></a><a name="p30749271"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p379401841880"><a name="p379401841880"></a><a name="p379401841880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul7176216121014"></a><a name="ul7176216121014"></a><ul id="ul7176216121014"><li>功能说明：弹性公网IP的类型</li><li>取值范围：<em id="i16850184017499"><a name="i16850184017499"></a><a name="i16850184017499"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="ul585004064911"></a><a name="ul585004064911"></a><ul id="ul585004064911"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li></ul>
    </li><li>约束：<a name="ul9738153015499"></a><a name="ul9738153015499"></a><ul id="ul9738153015499"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"publicip_type"字段未给定时，默认为5_bgp。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row389218135338"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p3576115214619"><a name="p3576115214619"></a><a name="p3576115214619"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p35761552124618"><a name="p35761552124618"></a><a name="p35761552124618"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p19576252174619"><a name="p19576252174619"></a><a name="p19576252174619"></a>IPv4时是申请到的弹性公网IP地址，IPv6时是IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="row6663943910"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p117521510894"><a name="p117521510894"></a><a name="p117521510894"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p97524108911"><a name="p97524108911"></a><a name="p97524108911"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p167581149102812"><a name="p167581149102812"></a><a name="p167581149102812"></a>IPv4时无此字段，IPv6时为申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="row2030210714336"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p5577105234617"><a name="p5577105234617"></a><a name="p5577105234617"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p2577165217467"><a name="p2577165217467"></a><a name="p2577165217467"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p10645141832513"><a name="p10645141832513"></a><a name="p10645141832513"></a>IP版本信息，取值范围是4和6</p>
    <a name="ul13987110227"></a><a name="ul13987110227"></a><ul id="ul13987110227"><li>4：表示IPv4</li><li>6：表示IPv6</li></ul>
    </td>
    </tr>
    <tr id="row283940631880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p182177951880"><a name="p182177951880"></a><a name="p182177951880"></a>private_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p60695041880"><a name="p60695041880"></a><a name="p60695041880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul1693412582014"></a><a name="ul1693412582014"></a><ul id="ul1693412582014"><li>功能说明：绑定弹性公网IP的私有IP地址</li><li>约束：只有绑定了的弹性公网IP查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="row264614551880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p630030811880"><a name="p630030811880"></a><a name="p630030811880"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p397229231880"><a name="p397229231880"></a><a name="p397229231880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul420471472010"></a><a name="ul420471472010"></a><ul id="ul420471472010"><li>功能说明：端口id。</li><li>约束：只有绑定了的弹性公网IP查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="row340905521880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p98713501880"><a name="p98713501880"></a><a name="p98713501880"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p58747301880"><a name="p58747301880"></a><a name="p58747301880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p269114516312"><a name="p269114516312"></a><a name="p269114516312"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row548200921880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p112424711880"><a name="p112424711880"></a><a name="p112424711880"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p92119381880"><a name="p92119381880"></a><a name="p92119381880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p36292894"><a name="p36292894"></a><a name="p36292894"></a>弹性公网IP申请时间（UTC）</p>
    </td>
    </tr>
    <tr id="row46164031880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p383843571880"><a name="p383843571880"></a><a name="p383843571880"></a>bandwidth_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p473107141880"><a name="p473107141880"></a><a name="p473107141880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p3934181618641"><a name="p3934181618641"></a><a name="p3934181618641"></a>弹性公网IP对应带宽ID</p>
    </td>
    </tr>
    <tr id="row626637421880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p425983371880"><a name="p425983371880"></a><a name="p425983371880"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p463832691880"><a name="p463832691880"></a><a name="p463832691880"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p2365466"><a name="p2365466"></a><a name="p2365466"></a>带宽大小，单位为Mbit/s。</p>
    </td>
    </tr>
    <tr id="row576448061880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p387177161880"><a name="p387177161880"></a><a name="p387177161880"></a>bandwidth_share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p21369006155933"><a name="p21369006155933"></a><a name="p21369006155933"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul2255712095"></a><a name="ul2255712095"></a><ul id="ul2255712095"><li>功能说明：弹性公网IP的带宽类型</li><li>取值范围：PER，WHOLE。<a name="ul729412507220"></a><a name="ul729412507220"></a><ul id="ul729412507220"><li>PER：独享带宽</li><li>WHOLE：共享带宽</li></ul>
    </li></ul>
    <a name="ul1369035014203"></a><a name="ul1369035014203"></a><ul id="ul1369035014203"><li>约束：其中IPv6暂不支持WHOLE类型带宽。</li></ul>
    </td>
    </tr>
    <tr id="row1444049321927"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p605297721941"><a name="p605297721941"></a><a name="p605297721941"></a>bandwidth_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p5224891921941"><a name="p5224891921941"></a><a name="p5224891921941"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p374970718414"><a name="p374970718414"></a><a name="p374970718414"></a>带宽名称。</p>
    </td>
    </tr>
    <tr id="row1353343333617"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p19564181313543"><a name="p19564181313543"></a><a name="p19564181313543"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p13564413185412"><a name="p13564413185412"></a><a name="p13564413185412"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul184004104214"></a><a name="ul184004104214"></a><ul id="ul184004104214"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。</li><li>创建弹性公网IP时，给弹性公网IP绑定企业项目ID。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  profile字段说明

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
    <td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.3 "><p id="p27381919173415"><a name="p27381919173415"></a><a name="p27381919173415"></a>用户的id</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例1（EIP绑定一张网卡）

    ```
    {
      "publicip": {
        "id": "f6318bef-6508-4ea5-a48f-6152b6b1a8fb",
        "status": "ACTIVE",
        "type": "5_bgp",
        "port_id": "a135e9b8-1630-40d2-a6c5-eb534a61efbe",
        "public_ip_address": "10.xx.xx.162",
        "private_ip_address": "192.168.1.131",
        "tenant_id": "26ae5181a416420998eb2093aaed84d9",
        "create_time": "2019-03-27 01:33:18",
        "bandwidth_size": 7,
        "ip_version": 4
      }
    }
    ```


-   响应样例2（转换为IPv6 EIP）

    ```
    {
      "publicip": {
        "id": "f6318bef-6508-4ea5-a48f-6152b6b1a8fb",
        "status": "DOWN",
        "type": "5_bgp",
        "public_ip_address": "10.xx.xx.162",
        "public_ipv6_address": "cdcd:xx:xx:xx::a9a:4aa2",
        "tenant_id": "26ae5181a416420998eb2093aaed84d9",
        "create_time": "2019-03-27 01:33:18",
        "bandwidth_size": 7,
        "ip_version": 6
      }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

