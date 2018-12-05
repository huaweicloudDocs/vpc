# 查询弹性公网IP列表<a name="ZH-CN_TOPIC_0020090598"></a>

## 功能介绍<a name="section52618256"></a>

查询弹性公网IP列表。

## URI<a name="section3802258"></a>

GET /v1/\{project\_id\}/publicips

样例：

```
/v1/{project_id}/publicips?limit=10&marker=4779ab1c-7c1a-44b1-a02e-93dfc361b32d
```

**表 1**  参数说明

<a name="table51200735"></a>
<table><thead align="left"><tr id="row8909633"><th class="cellrowborder" valign="top" width="30.826917308269174%" id="mcps1.2.5.1.1"><p id="p50591634"><a name="p50591634"></a><a name="p50591634"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.7981201879812%" id="mcps1.2.5.1.2"><p id="p4281684"><a name="p4281684"></a><a name="p4281684"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.548045195480455%" id="mcps1.2.5.1.3"><p id="p2939873918724"><a name="p2939873918724"></a><a name="p2939873918724"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="30.826917308269174%" id="mcps1.2.5.1.4"><p id="p11272110"><a name="p11272110"></a><a name="p11272110"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row40625737"><td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.1 "><p id="p2350413"><a name="p2350413"></a><a name="p2350413"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.7981201879812%" headers="mcps1.2.5.1.2 "><p id="p56165728"><a name="p56165728"></a><a name="p56165728"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.548045195480455%" headers="mcps1.2.5.1.3 "><p id="p3248766718724"><a name="p3248766718724"></a><a name="p3248766718724"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.4 "><p id="p53130157"><a name="p53130157"></a><a name="p53130157"></a>项目ID</p>
</td>
</tr>
<tr id="row8409368"><td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.1 "><p id="p10070188"><a name="p10070188"></a><a name="p10070188"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="18.7981201879812%" headers="mcps1.2.5.1.2 "><p id="p10378893"><a name="p10378893"></a><a name="p10378893"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.548045195480455%" headers="mcps1.2.5.1.3 "><p id="p1425535118724"><a name="p1425535118724"></a><a name="p1425535118724"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.4 "><p id="p47529299"><a name="p47529299"></a><a name="p47529299"></a>分页查询起始的资源id，为空时为查询第一页</p>
</td>
</tr>
<tr id="row25110514"><td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.1 "><p id="p20685786"><a name="p20685786"></a><a name="p20685786"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="18.7981201879812%" headers="mcps1.2.5.1.2 "><p id="p64935954"><a name="p64935954"></a><a name="p64935954"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.548045195480455%" headers="mcps1.2.5.1.3 "><p id="p1383277618724"><a name="p1383277618724"></a><a name="p1383277618724"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.4 "><a name="ul58841132132312"></a><a name="ul58841132132312"></a><ul id="ul58841132132312"><li>功能说明：每页返回的个数</li><li>取值范围：0~intmax</li></ul>
</td>
</tr>
<tr id="row1508191624314"><td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.1 "><p id="p388332415436"><a name="p388332415436"></a><a name="p388332415436"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="18.7981201879812%" headers="mcps1.2.5.1.2 "><p id="p4883162416438"><a name="p4883162416438"></a><a name="p4883162416438"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.548045195480455%" headers="mcps1.2.5.1.3 "><p id="p208831024134318"><a name="p208831024134318"></a><a name="p208831024134318"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.4 "><p id="p1388342494310"><a name="p1388342494310"></a><a name="p1388342494310"></a>IP地址版本信息，IPv4或IPv6</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section34220326"></a>

-   请求参数

    无

-   请求样例

    无


## 响应消息<a name="section39547486"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table22603002152149"></a>
    <table><thead align="left"><tr id="row30843029152149"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p15257431152149"><a name="p15257431152149"></a><a name="p15257431152149"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="p44693705152149"><a name="p44693705152149"></a><a name="p44693705152149"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="p63420361152149"><a name="p63420361152149"></a><a name="p63420361152149"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row36775597152149"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p26033374152149"><a name="p26033374152149"></a><a name="p26033374152149"></a>publicips</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p12908356152149"><a name="p12908356152149"></a><a name="p12908356152149"></a><em id="i28723475152212"><a name="i28723475152212"></a><a name="i28723475152212"></a>列表数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p14951203152149"><a name="p14951203152149"></a><a name="p14951203152149"></a>弹性公网IP列表对象</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicips字段说明

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
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul263945115243"></a><a name="ul263945115243"></a><ul id="ul263945115243"><li>功能说明：弹性公网IP的状态</li><li>取值范围：<a name="ul7905205815810"></a><a name="ul7905205815810"></a><ul id="ul7905205815810"><li>冻结FREEZED</li><li>绑定失败BIND_ERROR</li><li>绑定中BINDING</li><li>释放中PENDING_DELETE</li><li>创建中PENDING_CREATE</li><li>创建中NOTIFYING</li><li>释放中NOTIFY_DELETE</li><li>更新中PENDING_UPDATE</li><li>未绑定DOWN</li><li>绑定ACTIVE</li><li>绑定ELB</li><li>失败ERROR</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row16130133562319"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p09743162419"><a name="p09743162419"></a><a name="p09743162419"></a>profile</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p12971231132410"><a name="p12971231132410"></a><a name="p12971231132410"></a>Dict</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p169773114242"><a name="p169773114242"></a><a name="p169773114242"></a>额外参数，包括订单id、产品id等信息</p>
    <p id="p156320510335"><a name="p156320510335"></a><a name="p156320510335"></a>如果profile不为空，说明是包周期的弹性公网IP</p>
    </td>
    </tr>
    <tr id="row230260811880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p531732681880"><a name="p531732681880"></a><a name="p531732681880"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p379401841880"><a name="p379401841880"></a><a name="p379401841880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p532560571880"><a name="p532560571880"></a><a name="p532560571880"></a>弹性公网IP的类型</p>
    </td>
    </tr>
    <tr id="row389218135338"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p59108624"><a name="p59108624"></a><a name="p59108624"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p904808818330"><a name="p904808818330"></a><a name="p904808818330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p40237373"><a name="p40237373"></a><a name="p40237373"></a>IPv4时是申请到的弹性公网IP地址，IPv6时是IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="row6663943910"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p117521510894"><a name="p117521510894"></a><a name="p117521510894"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p97524108911"><a name="p97524108911"></a><a name="p97524108911"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p11752410599"><a name="p11752410599"></a><a name="p11752410599"></a>IPv4时无此字段，IPv6时为申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="row2030210714336"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p171101456172118"><a name="p171101456172118"></a><a name="p171101456172118"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p1811012569218"><a name="p1811012569218"></a><a name="p1811012569218"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p1211011564217"><a name="p1211011564217"></a><a name="p1211011564217"></a>IP版本信息，取值范围是4和6</p>
    </td>
    </tr>
    <tr id="row283940631880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p182177951880"><a name="p182177951880"></a><a name="p182177951880"></a>private_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p60695041880"><a name="p60695041880"></a><a name="p60695041880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul631315111255"></a><a name="ul631315111255"></a><ul id="ul631315111255"><li>功能说明：绑定弹性公网IP的私有IP地址</li><li>约束：只有绑定了的弹性公网IP查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="row264614551880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p630030811880"><a name="p630030811880"></a><a name="p630030811880"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p397229231880"><a name="p397229231880"></a><a name="p397229231880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul11879125982520"></a><a name="ul11879125982520"></a><ul id="ul11879125982520"><li>功能说明：端口id。</li><li>约束：只有绑定了的弹性公网IP查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="row340905521880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p98713501880"><a name="p98713501880"></a><a name="p98713501880"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p58747301880"><a name="p58747301880"></a><a name="p58747301880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p60911211880"><a name="p60911211880"></a><a name="p60911211880"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row548200921880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p112424711880"><a name="p112424711880"></a><a name="p112424711880"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p92119381880"><a name="p92119381880"></a><a name="p92119381880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p79694741880"><a name="p79694741880"></a><a name="p79694741880"></a>弹性公网IP申请时间（UTC时间）</p>
    </td>
    </tr>
    <tr id="row46164031880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p383843571880"><a name="p383843571880"></a><a name="p383843571880"></a>bandwidth_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p473107141880"><a name="p473107141880"></a><a name="p473107141880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p69626381880"><a name="p69626381880"></a><a name="p69626381880"></a>弹性公网IP对应带宽ID</p>
    </td>
    </tr>
    <tr id="row626637421880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p425983371880"><a name="p425983371880"></a><a name="p425983371880"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p463832691880"><a name="p463832691880"></a><a name="p463832691880"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p660573021880"><a name="p660573021880"></a><a name="p660573021880"></a>带宽大小</p>
    </td>
    </tr>
    <tr id="row576448061880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p387177161880"><a name="p387177161880"></a><a name="p387177161880"></a>bandwidth_share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p21369006155933"><a name="p21369006155933"></a><a name="p21369006155933"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p1939082916015"><a name="p1939082916015"></a><a name="p1939082916015"></a>表示共享带宽或者独享带宽，WHOLE表示共享带宽，PER表示独享带宽。</p>
    </td>
    </tr>
    <tr id="row1444049321927"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p605297721941"><a name="p605297721941"></a><a name="p605297721941"></a>bandwidth_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p5224891921941"><a name="p5224891921941"></a><a name="p5224891921941"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p430401821941"><a name="p430401821941"></a><a name="p430401821941"></a>带宽名称</p>
    </td>
    </tr>
    <tr id="row1353343333617"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p19564181313543"><a name="p19564181313543"></a><a name="p19564181313543"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p13564413185412"><a name="p13564413185412"></a><a name="p13564413185412"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul12718111415273"></a><a name="ul12718111415273"></a><ul id="ul12718111415273"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。</li><li>创建弹性公网IP时，给弹性公网IP绑定企业项目ID。</li></ul>
    <div class="note" id="note1617278101315"><a name="note1617278101315"></a><a name="note1617278101315"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1817788121313"><a name="p1817788121313"></a><a name="p1817788121313"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见《企业资源服务用户指南》。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  profile字段说明

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
    <td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.3 "><p id="p26235912225"><a name="p26235912225"></a><a name="p26235912225"></a>1、功能说明：订单的id</p>
    </td>
    </tr>
    <tr id="row18686141920341"><td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.1 "><p id="p11688201923418"><a name="p11688201923418"></a><a name="p11688201923418"></a>product_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.2.4.1.2 "><p id="p169318196347"><a name="p169318196347"></a><a name="p169318196347"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.3 "><p id="p149921832153419"><a name="p149921832153419"></a><a name="p149921832153419"></a>1、功能说明：产品的id</p>
    </td>
    </tr>
    <tr id="row167161319173418"><td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.1 "><p id="p5718101903412"><a name="p5718101903412"></a><a name="p5718101903412"></a>region_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.2.4.1.2 "><p id="p47241019143417"><a name="p47241019143417"></a><a name="p47241019143417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.3 "><p id="p09201951174716"><a name="p09201951174716"></a><a name="p09201951174716"></a>1、功能说明：region的id</p>
    </td>
    </tr>
    <tr id="row1472971912347"><td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.1 "><p id="p187311719103415"><a name="p187311719103415"></a><a name="p187311719103415"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.2.4.1.2 "><p id="p9735141923418"><a name="p9735141923418"></a><a name="p9735141923418"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.35%" headers="mcps1.2.4.1.3 "><p id="p27381919173415"><a name="p27381919173415"></a><a name="p27381919173415"></a>1、功能说明：用户的id</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "publicips": [
            {
                "id": "6285e7be-fd9f-497c-bc2d-dd0bdea6efe0",
                "status": "DOWN",
                "profile": {
                  "user_id": "35f2b308f5d64441a6fa7999fbcd4321",
                  "product_id": "00301-48027-0--0",
                  "region_id": "xxx",
                  "order_id": "xxxxxxxxx"
                },
                "type": "5_bgp",
                "public_ip_address": "161.xx.xx.9",
                "private_ip_address": "192.168.10.5",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "create_time": "2015-07-16 04:22:32",
                "bandwidth_id": "3fa5b383-5a73-4dcb-a314-c6128546d855",
                "bandwidth_share_type": "PER",
                "bandwidth_size": 5,
                "bandwidth_name": "bandwidth-test",
                "enterprise_project_id":"b261ac1f-2489-4bc7-b31b-c33c3346a439",
                "ip_version": 4
            },
            {
                "id": "80d5b82e-43b9-4f82-809a-37bec5793bd4",
                "status": "DOWN",
                  "user_id": null,
                "type": "5_bgp",
                "public_ip_address": "161.xx.xx.10",
                "private_ip_address": "192.168.10.6",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "create_time": "2015-07-16 04:23:03",
                "bandwidth_id": "a79fd11a-047b-4f5b-8f12-99c178cc780a",
                "bandwidth_share_type": "PER",
                "bandwidth_size": 5,
                "bandwidth_name": "bandwidth-test1",
                "enterprise_project_id":"0",
                "ip_version": 4
            }
        ]
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

