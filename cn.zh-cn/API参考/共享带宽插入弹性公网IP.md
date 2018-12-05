# 共享带宽插入弹性公网IP<a name="ZH-CN_TOPIC_0106971321"></a>

## 功能介绍<a name="section16581154"></a>

共享带宽插入弹性公网IP。

## URI<a name="section15012662"></a>

POST /v2.0/\{project\_id\}/bandwidths/\{bandwidth\_id\}/insert

**表 1**  参数说明

<a name="table25281875"></a>
<table><thead align="left"><tr id="row26712487"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p16227847"><a name="p16227847"></a><a name="p16227847"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p39387211"><a name="p39387211"></a><a name="p39387211"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p36247516"><a name="p36247516"></a><a name="p36247516"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row50367649"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p53247746"><a name="p53247746"></a><a name="p53247746"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p18100201"><a name="p18100201"></a><a name="p18100201"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p56830139"><a name="p56830139"></a><a name="p56830139"></a>项目ID</p>
</td>
</tr>
<tr id="row41709209"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p23002745"><a name="p23002745"></a><a name="p23002745"></a>bandwidth_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p51283066"><a name="p51283066"></a><a name="p51283066"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p60287683"><a name="p60287683"></a><a name="p60287683"></a>带宽唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section896237"></a>

-   请求参数

    <a name="table3057854815556"></a>
    <table><thead align="left"><tr id="row6286666315556"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.1.5.1.1"><p id="p5903494715556"><a name="p5903494715556"></a><a name="p5903494715556"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.1.5.1.2"><p id="p1710139915556"><a name="p1710139915556"></a><a name="p1710139915556"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.5.1.3"><p id="p4303610815556"><a name="p4303610815556"></a><a name="p4303610815556"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.18%" id="mcps1.1.5.1.4"><p id="p6337274615556"><a name="p6337274615556"></a><a name="p6337274615556"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3291877615556"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.1.5.1.1 "><p id="p4917516615556"><a name="p4917516615556"></a><a name="p4917516615556"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.1.5.1.2 "><p id="p2376550915556"><a name="p2376550915556"></a><a name="p2376550915556"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.5.1.3 "><p id="p4595806815556"><a name="p4595806815556"></a><a name="p4595806815556"></a><em id="i1096943515556"><a name="i1096943515556"></a><a name="i1096943515556"></a>字典数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.1.5.1.4 "><p id="p1610901815556"><a name="p1610901815556"></a><a name="p1610901815556"></a>带宽对象</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  bandwidth字段说明

    <a name="table31854691"></a>
    <table><thead align="left"><tr id="row6882862"><th class="cellrowborder" valign="top" width="13.350000000000001%" id="mcps1.2.5.1.1"><p id="p20640979"><a name="p20640979"></a><a name="p20640979"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.91%" id="mcps1.2.5.1.2"><p id="p61306625"><a name="p61306625"></a><a name="p61306625"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.91%" id="mcps1.2.5.1.3"><p id="p5200653172316"><a name="p5200653172316"></a><a name="p5200653172316"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.830000000000005%" id="mcps1.2.5.1.4"><p id="p66889567"><a name="p66889567"></a><a name="p66889567"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row49345813"><td class="cellrowborder" valign="top" width="13.350000000000001%" headers="mcps1.2.5.1.1 "><p id="p37587916"><a name="p37587916"></a><a name="p37587916"></a>publicip_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.2 "><p id="p24722347"><a name="p24722347"></a><a name="p24722347"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.3 "><p id="p18599757172316"><a name="p18599757172316"></a><a name="p18599757172316"></a><em id="i1187916316158"><a name="i1187916316158"></a><a name="i1187916316158"></a>字典数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="58.830000000000005%" headers="mcps1.2.5.1.4 "><a name="ul1057071610312"></a><a name="ul1057071610312"></a><ul id="ul1057071610312"><li>功能说明：要插入共享带宽的弹性公网IP信息</li><li>约束：WHOLE类型的带宽支持多个弹性公网IP，跟租户的配额相关，默认一个共享带宽可以放置20个弹性公网IP</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicip\_info对象

    <a name="table30936422"></a>
    <table><thead align="left"><tr id="row17161430"><th class="cellrowborder" valign="top" width="25.740000000000002%" id="mcps1.2.4.1.1"><p id="p47898561"><a name="p47898561"></a><a name="p47898561"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.5%" id="mcps1.2.4.1.2"><p id="p2828296517154"><a name="p2828296517154"></a><a name="p2828296517154"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.76%" id="mcps1.2.4.1.3"><p id="p58761073"><a name="p58761073"></a><a name="p58761073"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row62026502"><td class="cellrowborder" valign="top" width="25.740000000000002%" headers="mcps1.2.4.1.1 "><p id="p58090788"><a name="p58090788"></a><a name="p58090788"></a>publicip_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.5%" headers="mcps1.2.4.1.2 "><p id="p921881117154"><a name="p921881117154"></a><a name="p921881117154"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.76%" headers="mcps1.2.4.1.3 "><p id="p476380"><a name="p476380"></a><a name="p476380"></a>带宽对应的弹性公网IP的唯一标识</p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    {
        "bandwidth": {
            "publicip_info": [
                {
                    "publicip_id": "d91b0028-6f6b-4478-808a-297b75b6812a"
                },
                {
                    "publicip_id": "1d184b2c-4ec9-49b5-a3f9-27600a76ba3f"
                }
            ]
        }
    }
    ```


## 响应消息<a name="section8066134"></a>

-   响应参数

    <a name="table58151089155516"></a>
    <table><thead align="left"><tr id="row25417629155516"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.1.4.1.1"><p id="p45562050155516"><a name="p45562050155516"></a><a name="p45562050155516"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.1.4.1.2"><p id="p29734214155516"><a name="p29734214155516"></a><a name="p29734214155516"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.1.4.1.3"><p id="p59661173155516"><a name="p59661173155516"></a><a name="p59661173155516"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row716877155516"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.1.4.1.1 "><p id="p58067061155516"><a name="p58067061155516"></a><a name="p58067061155516"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.1.4.1.2 "><p id="p967638155516"><a name="p967638155516"></a><a name="p967638155516"></a><em id="i8708746155516"><a name="i8708746155516"></a><a name="i8708746155516"></a>字典数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.1.4.1.3 "><p id="p34319839155516"><a name="p34319839155516"></a><a name="p34319839155516"></a>带宽对象</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  bandwidth字段说明

    <a name="table60972066"></a>
    <table><thead align="left"><tr id="row10740297"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="p64657722"><a name="p64657722"></a><a name="p64657722"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24%" id="mcps1.2.4.1.2"><p id="p48285594171334"><a name="p48285594171334"></a><a name="p48285594171334"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51%" id="mcps1.2.4.1.3"><p id="p24185120"><a name="p24185120"></a><a name="p24185120"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12837735"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p33223577"><a name="p33223577"></a><a name="p33223577"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p18819060171334"><a name="p18819060171334"></a><a name="p18819060171334"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul109251630343"></a><a name="ul109251630343"></a><ul id="ul109251630343"><li>功能说明：带宽名称</li><li>取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li></ul>
    </td>
    </tr>
    <tr id="row61765553"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p36953931"><a name="p36953931"></a><a name="p36953931"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p47948882171334"><a name="p47948882171334"></a><a name="p47948882171334"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul24323535419"></a><a name="ul24323535419"></a><ul id="ul24323535419"><li>功能说明：带宽大小。</li><li>取值范围：默认5Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。</li></ul>
    </td>
    </tr>
    <tr id="row63416368"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p36452220"><a name="p36452220"></a><a name="p36452220"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p58654237171334"><a name="p58654237171334"></a><a name="p58654237171334"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><p id="p17440495"><a name="p17440495"></a><a name="p17440495"></a>带宽唯一标识</p>
    </td>
    </tr>
    <tr id="row22746728"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p30545685"><a name="p30545685"></a><a name="p30545685"></a>share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p53372732171334"><a name="p53372732171334"></a><a name="p53372732171334"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul175704211750"></a><a name="ul175704211750"></a><ul id="ul175704211750"><li>功能说明：带宽类型，标识是否是共享带宽</li><li>取值范围：WHOLE，PER</li><li>WHOLE表示共享带宽；PER，表示独享带宽</li></ul>
    </td>
    </tr>
    <tr id="row51058985"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p42137138"><a name="p42137138"></a><a name="p42137138"></a>publicip_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p28224024171334"><a name="p28224024171334"></a><a name="p28224024171334"></a>字典数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul2114338754"></a><a name="ul2114338754"></a><ul id="ul2114338754"><li>功能说明：带宽对应的弹性公网IP信息</li><li>约束：WHOLE类型的带宽支持多个弹性公网IP，PER类型的带宽只能对应一个弹性公网IP</li></ul>
    </td>
    </tr>
    <tr id="row36079911"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p36791668"><a name="p36791668"></a><a name="p36791668"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p4444568171334"><a name="p4444568171334"></a><a name="p4444568171334"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><p id="p7337776171431"><a name="p7337776171431"></a><a name="p7337776171431"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row8730397"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p36073588"><a name="p36073588"></a><a name="p36073588"></a>bandwidth_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p24465700171334"><a name="p24465700171334"></a><a name="p24465700171334"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul138981856955"></a><a name="ul138981856955"></a><ul id="ul138981856955"><li>功能说明：带宽类型，共享带宽默认为share。</li><li>取值范围：share，bgp，telcom，sbgp等。</li></ul>
    </td>
    </tr>
    <tr id="row2300081817338"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p3464166173311"><a name="p3464166173311"></a><a name="p3464166173311"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p45598234173311"><a name="p45598234173311"></a><a name="p45598234173311"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul1081883716614"></a><a name="ul1081883716614"></a><ul id="ul1081883716614"><li>功能说明：按流量计费还是按带宽计费。</li><li>取值范围：bandwidth，traffic，不返回或者为空时表示是bandwidth。</li><li>共享带宽仅支持按带宽计费。</li></ul>
    </td>
    </tr>
    <tr id="row186022695519"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p1886113265557"><a name="p1886113265557"></a><a name="p1886113265557"></a>billing_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p886152614551"><a name="p886152614551"></a><a name="p886152614551"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><p id="p9861112645515"><a name="p9861112645515"></a><a name="p9861112645515"></a>功能说明：账单信息</p>
    <p id="p1158114251321"><a name="p1158114251321"></a><a name="p1158114251321"></a>如果billing_info不为空，说明是包周期的带宽</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  publicip\_info对象

    <a name="table51281965"></a>
    <table><thead align="left"><tr id="row26928941"><th class="cellrowborder" valign="top" width="26.71%" id="mcps1.2.4.1.1"><p id="p33760584"><a name="p33760584"></a><a name="p33760584"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.6%" id="mcps1.2.4.1.2"><p id="p37114580172552"><a name="p37114580172552"></a><a name="p37114580172552"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.69%" id="mcps1.2.4.1.3"><p id="p43944024"><a name="p43944024"></a><a name="p43944024"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2696221"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="p17067371"><a name="p17067371"></a><a name="p17067371"></a>publicip_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="p53490986172552"><a name="p53490986172552"></a><a name="p53490986172552"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="p37389755"><a name="p37389755"></a><a name="p37389755"></a>带宽对应的弹性公网IP的唯一标识</p>
    </td>
    </tr>
    <tr id="row963478"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="p621304517467"><a name="p621304517467"></a><a name="p621304517467"></a>publicip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="p1021574544615"><a name="p1021574544615"></a><a name="p1021574544615"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="p102181445114616"><a name="p102181445114616"></a><a name="p102181445114616"></a>IPv4时是申请到的弹性公网IP地址，IPv6时为IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="row049765515547"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="p1270211337315"><a name="p1270211337315"></a><a name="p1270211337315"></a>publicipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="p570212339313"><a name="p570212339313"></a><a name="p570212339313"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="p20702103373114"><a name="p20702103373114"></a><a name="p20702103373114"></a>IPv4时无此字段，IPv6时为申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="row11195191125518"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="p197308575327"><a name="p197308575327"></a><a name="p197308575327"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="p11730115718326"><a name="p11730115718326"></a><a name="p11730115718326"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="p673155783216"><a name="p673155783216"></a><a name="p673155783216"></a>IP版本信息，取值范围是4和6</p>
    </td>
    </tr>
    <tr id="row32534423"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="p18042568"><a name="p18042568"></a><a name="p18042568"></a>publicip_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="p42115453172552"><a name="p42115453172552"></a><a name="p42115453172552"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><a name="ul11964539104914"></a><a name="ul11964539104914"></a><ul id="ul11964539104914"><li>功能说明：弹性公网IP的类型</li><li>取值范围：5_telcom，5_union，5_bgp</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "bandwidth": {
            "id": "3fa5b383-5a73-4dcb-a314-c6128546d855",
            "name": "bandwidth123",
            "size": 10,
            "share_type": "WHOLE",
            "publicip_info": [
                {
                    "publicip_id": "d91b0028-6f6b-4478-808a-297b75b6812a",
                    "publicip_address": "99.xx.xx.140",
                    "publicip_type": "5_bgp",
                    "ip_version": 4
                },
                {
                    "publicip_id": "1d184b2c-4ec9-49b5-a3f9-27600a76ba3f",
                    "publicip_address": "99.xx.xx.82",
                    "publicip_type": "5_bgp",
                    "ip_version": 4
                }
            ],
            "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
            "charge_mode": "bandwidth",
            "bandwidth_type": "share",
            "billing_info": "CS1712121146TSQOJ:0616e2a5dc9f4985ba52ea8c0c7e273c:southchina:35f2b308f5d64441a6fa7999fbcd4321"
        }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

