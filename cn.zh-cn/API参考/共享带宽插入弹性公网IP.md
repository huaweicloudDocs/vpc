# 共享带宽插入弹性公网IP<a name="ZH-CN_TOPIC_0201534131"></a>

## 功能介绍<a name="section16581154"></a>

共享带宽插入弹性公网IP。

## URI<a name="section15012662"></a>

POST /v2.0/\{project\_id\}/bandwidths/\{bandwidth\_id\}/insert

参数说明请参见[表1](#table25281875)。

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
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
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

    **表 2**  请求参数

    <a name="table3057854815556"></a>
    <table><thead align="left"><tr id="row6286666315556"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="p5903494715556"><a name="p5903494715556"></a><a name="p5903494715556"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="p1710139915556"><a name="p1710139915556"></a><a name="p1710139915556"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="p4303610815556"><a name="p4303610815556"></a><a name="p4303610815556"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.18%" id="mcps1.2.5.1.4"><p id="p6337274615556"><a name="p6337274615556"></a><a name="p6337274615556"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3291877615556"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p4917516615556"><a name="p4917516615556"></a><a name="p4917516615556"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p2376550915556"><a name="p2376550915556"></a><a name="p2376550915556"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p4595806815556"><a name="p4595806815556"></a><a name="p4595806815556"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p1610901815556"><a name="p1610901815556"></a><a name="p1610901815556"></a>带宽对象，请参见<a href="#table31854691">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  bandwidth字段说明

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
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.3 "><p id="p18599757172316"><a name="p18599757172316"></a><a name="p18599757172316"></a>Array of <a href="#table30936422">publicip_info</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.830000000000005%" headers="mcps1.2.5.1.4 "><a name="ul1057071610312"></a><a name="ul1057071610312"></a><ul id="ul1057071610312"><li>功能说明：要插入共享带宽的弹性公网IP信息，请参见<a href="#table30936422">表4</a>。</li><li>约束：WHOLE类型的带宽支持多个弹性公网IP，跟租户的配额相关，默认一个共享带宽的配额为20。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  publicip\_info对象

    <a name="table30936422"></a>
    <table><thead align="left"><tr id="row17161430"><th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1"><p id="p47898561"><a name="p47898561"></a><a name="p47898561"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.03%" id="mcps1.2.5.1.2"><p id="p169718416504"><a name="p169718416504"></a><a name="p169718416504"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.96%" id="mcps1.2.5.1.3"><p id="p2828296517154"><a name="p2828296517154"></a><a name="p2828296517154"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.72%" id="mcps1.2.5.1.4"><p id="p58761073"><a name="p58761073"></a><a name="p58761073"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row62026502"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="p58090788"><a name="p58090788"></a><a name="p58090788"></a>publicip_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.03%" headers="mcps1.2.5.1.2 "><p id="p79716416504"><a name="p79716416504"></a><a name="p79716416504"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.2.5.1.3 "><p id="p921881117154"><a name="p921881117154"></a><a name="p921881117154"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.72%" headers="mcps1.2.5.1.4 "><p id="p476380"><a name="p476380"></a><a name="p476380"></a>带宽对应的弹性公网IP的唯一标识</p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    POST https://{Endpoint}/v2.0/{project_id}/bandwidths/{bandwidth_id}/insert
    
    {
      "bandwidth": {
        "publicip_info": [
          {
            "publicip_id": "29b114d1-2d41-4741-a1f0-b6f80aabceff",
            "publici_type": "5_bgp"
          }
        ]
      }
    }
    ```


## 响应消息<a name="section8066134"></a>

-   响应参数

    **表 5**  响应参数

    <a name="table58151089155516"></a>
    <table><thead align="left"><tr id="row25417629155516"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p45562050155516"><a name="p45562050155516"></a><a name="p45562050155516"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="p29734214155516"><a name="p29734214155516"></a><a name="p29734214155516"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="p59661173155516"><a name="p59661173155516"></a><a name="p59661173155516"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row716877155516"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p58067061155516"><a name="p58067061155516"></a><a name="p58067061155516"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p967638155516"><a name="p967638155516"></a><a name="p967638155516"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p34319839155516"><a name="p34319839155516"></a><a name="p34319839155516"></a>带宽对象，请参见<a href="#table138718569112">表6</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  bandwidth字段说明

    <a name="table138718569112"></a>
    <table><thead align="left"><tr id="row128705614111"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="p787856121118"><a name="p787856121118"></a><a name="p787856121118"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24%" id="mcps1.2.4.1.2"><p id="p2088556181119"><a name="p2088556181119"></a><a name="p2088556181119"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51%" id="mcps1.2.4.1.3"><p id="p1888115661112"><a name="p1888115661112"></a><a name="p1888115661112"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1688115611112"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p78865651114"><a name="p78865651114"></a><a name="p78865651114"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1588256131115"><a name="p1588256131115"></a><a name="p1588256131115"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul181211824134816"></a><a name="ul181211824134816"></a><ul id="ul181211824134816"><li>功能说明：带宽名称</li><li>取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li></ul>
    </td>
    </tr>
    <tr id="row17881356171113"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p20882056151111"><a name="p20882056151111"></a><a name="p20882056151111"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p208855641111"><a name="p208855641111"></a><a name="p208855641111"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul19451840174816"></a><a name="ul19451840174816"></a><ul id="ul19451840174816"><li>功能说明：带宽大小。</li><li>取值范围：默认5Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。</li></ul>
    </td>
    </tr>
    <tr id="row488105641111"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p10881056191119"><a name="p10881056191119"></a><a name="p10881056191119"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p88816566118"><a name="p88816566118"></a><a name="p88816566118"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><p id="p48813561118"><a name="p48813561118"></a><a name="p48813561118"></a>带宽唯一标识</p>
    </td>
    </tr>
    <tr id="row158855661120"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p17881856151120"><a name="p17881856151120"></a><a name="p17881856151120"></a>share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p18887564112"><a name="p18887564112"></a><a name="p18887564112"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul4262181884915"></a><a name="ul4262181884915"></a><ul id="ul4262181884915"><li>功能说明：带宽类型，标识是否是共享带宽</li><li>取值范围：WHOLE，PER<a name="ul313253512484"></a><a name="ul313253512484"></a><ul id="ul313253512484"><li>WHOLE表示共享带宽</li><li>PER表示独享带宽</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row1089195616112"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p88910565118"><a name="p88910565118"></a><a name="p88910565118"></a>publicip_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p289456141114"><a name="p289456141114"></a><a name="p289456141114"></a>Array of <a href="#table51281965">publicip_info</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul14114132894913"></a><a name="ul14114132894913"></a><ul id="ul14114132894913"><li>功能说明：带宽对应的弹性公网IP信息，请参见<a href="#table51281965">表7</a>。</li><li>约束：WHOLE类型的带宽支持多个弹性公网IP，PER类型的带宽只能对应一个弹性公网IP</li></ul>
    </td>
    </tr>
    <tr id="row1489156171117"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p489456141120"><a name="p489456141120"></a><a name="p489456141120"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p19891756141115"><a name="p19891756141115"></a><a name="p19891756141115"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><p id="p19517617121017"><a name="p19517617121017"></a><a name="p19517617121017"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row1089056121112"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p1989105620112"><a name="p1989105620112"></a><a name="p1989105620112"></a>bandwidth_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p158995611110"><a name="p158995611110"></a><a name="p158995611110"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul5731955125012"></a><a name="ul5731955125012"></a><ul id="ul5731955125012"><li>功能说明：带宽类型，共享带宽默认为share。</li><li>取值范围：share，bgp，telcom，sbgp等<a name="ul1933102125013"></a><a name="ul1933102125013"></a><ul id="ul1933102125013"><li>share：共享带宽</li><li>bgp：动态bgp</li><li>telcom ：联通</li><li>sbgp：静态bgp</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row1590155616116"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p1090356181119"><a name="p1090356181119"></a><a name="p1090356181119"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p69010561114"><a name="p69010561114"></a><a name="p69010561114"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul690195631110"></a><a name="ul690195631110"></a><ul id="ul690195631110"><li>功能说明：按流量计费还是按带宽计费。</li><li>取值范围：bandwidth（按带宽计费），traffic（按流量计费），不返回或者为空时表示是bandwidth。</li><li>约束：共享带宽仅支持按带宽计费。</li></ul>
    </td>
    </tr>
    <tr id="row590556151112"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p99015567111"><a name="p99015567111"></a><a name="p99015567111"></a>billing_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1890115614111"><a name="p1890115614111"></a><a name="p1890115614111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><p id="p1190145612112"><a name="p1190145612112"></a><a name="p1190145612112"></a>账单信息。</p>
    <p id="p414131417317"><a name="p414131417317"></a><a name="p414131417317"></a>如果billing_info不为空，说明是包周期的带宽。</p>
    </td>
    </tr>
    <tr id="row457893134810"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p36136296490"><a name="p36136296490"></a><a name="p36136296490"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p561632984912"><a name="p561632984912"></a><a name="p561632984912"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul137091434125111"></a><a name="ul137091434125111"></a><ul id="ul137091434125111"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。创建共享带宽时，给共享带宽绑定企业项目ID。</li></ul>
    <div class="note" id="note13203107131712"><a name="note13203107131712"></a><a name="note13203107131712"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1915862704914"><a name="p1915862704914"></a><a name="p1915862704914"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0126101490.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row9477203041814"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p16479330181816"><a name="p16479330181816"></a><a name="p16479330181816"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p5479163011185"><a name="p5479163011185"></a><a name="p5479163011185"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="ul114381249113115"></a><a name="ul114381249113115"></a><ul id="ul114381249113115"><li>功能说明：带宽的状态</li><li>取值范围：<a name="ul1943874963116"></a><a name="ul1943874963116"></a><ul id="ul1943874963116"><li>FREEZED：冻结</li><li>NORMAL：正常</li></ul>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 7**  publicip\_info对象

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
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="p3792141220526"><a name="p3792141220526"></a><a name="p3792141220526"></a>功能说明：带宽对应的弹性公网IP的唯一标识或IPv6端口的唯一标识</p>
    </td>
    </tr>
    <tr id="row963478"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="p621304517467"><a name="p621304517467"></a><a name="p621304517467"></a>publicip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="p1021574544615"><a name="p1021574544615"></a><a name="p1021574544615"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="p198309316175"><a name="p198309316175"></a><a name="p198309316175"></a>功能说明：IPv4时是申请到的弹性公网IP地址，IPv6时为IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="row049765515547"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="p1270211337315"><a name="p1270211337315"></a><a name="p1270211337315"></a>publicipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="p570212339313"><a name="p570212339313"></a><a name="p570212339313"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="p383015318171"><a name="p383015318171"></a><a name="p383015318171"></a>功能说明：IPv4时无此字段，IPv6时为申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="row11195191125518"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="p197308575327"><a name="p197308575327"></a><a name="p197308575327"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="p11730115718326"><a name="p11730115718326"></a><a name="p11730115718326"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><a name="ul4257145935817"></a><a name="ul4257145935817"></a><ul id="ul4257145935817"><li>功能说明：IP版本信息</li><li>取值范围：<a name="ul208241936115914"></a><a name="ul208241936115914"></a><ul id="ul208241936115914"><li>4：IPv4</li><li>6：IPv6</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row32534423"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="p18042568"><a name="p18042568"></a><a name="p18042568"></a>publicip_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="p42115453172552"><a name="p42115453172552"></a><a name="p42115453172552"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><a name="ul13831731151713"></a><a name="ul13831731151713"></a><ul id="ul13831731151713"><li>功能说明：弹性公网IP的类型</li><li>取值范围：5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）<a name="ul161028178419"></a><a name="ul161028178419"></a><ul id="ul161028178419"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li></ul>
    </li><li>约束：必须是系统具体支持的类型</li></ul>
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
                     "publicip_address": "::ffff:192.168.89.9", 
                     "publicip_type": "5_dualStack",
                     "ip_version": 6
                },
                {
                    "publicip_id": "1d184b2c-4ec9-49b5-a3f9-27600a76ba3f",
                    "publicip_address": "99.xx.xx.82",
                    "publicip_type": "5_bgp",
                    "ip_version": 4
                }
            ],
            "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
            "charge_mode": "traffic",
            "bandwidth_type": "share",
            "billing_info": "CS1712121146TSQOJ:0616e2a5dc9f4985ba52ea8c0c7e273c:southchina:35f2b308f5d64441a6fa7999fbcd4321"
        }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

