# 申请包周期弹性公网IP<a name="ZH-CN_TOPIC_0097550708"></a>

## 功能介绍<a name="section95417125714"></a>

申请弹性公网IP。

## URI<a name="section135831105716"></a>

POST /v2.0/\{project\_id\}/publicips

**表 1**  参数说明

<a name="table56312185710"></a>
<table><thead align="left"><tr id="row1965641135717"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p665618113574"><a name="p665618113574"></a><a name="p665618113574"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p166564116579"><a name="p166564116579"></a><a name="p166564116579"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p3657101185710"><a name="p3657101185710"></a><a name="p3657101185710"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row166578119574"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1865719114578"><a name="p1865719114578"></a><a name="p1865719114578"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p18657181175718"><a name="p18657181175718"></a><a name="p18657181175718"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p136571019574"><a name="p136571019574"></a><a name="p136571019574"></a>项目ID</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section14762185713"></a>

-   请求参数

    **表 2**  请求参数

    <a name="table15872015575"></a>
    <table><thead align="left"><tr id="row126571614572"><th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.1"><p id="p1465751175719"><a name="p1465751175719"></a><a name="p1465751175719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p56571318579"><a name="p56571318579"></a><a name="p56571318579"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.3"><p id="p1657161135717"><a name="p1657161135717"></a><a name="p1657161135717"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.95520447955205%" id="mcps1.2.5.1.4"><p id="p965717135716"><a name="p965717135716"></a><a name="p965717135716"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row166579118574"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.1 "><p id="p565741155713"><a name="p565741155713"></a><a name="p565741155713"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p5657161175715"><a name="p5657161175715"></a><a name="p5657161175715"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.3 "><p id="p865721165716"><a name="p865721165716"></a><a name="p865721165716"></a><em id="i9657116576"><a name="i9657116576"></a><a name="i9657116576"></a>字典数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="47.95520447955205%" headers="mcps1.2.5.1.4 "><p id="p465781125718"><a name="p465781125718"></a><a name="p465781125718"></a>弹性公网IP对象</p>
    </td>
    </tr>
    <tr id="row1465781175717"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.1 "><p id="p15657131175716"><a name="p15657131175716"></a><a name="p15657131175716"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p765771205716"><a name="p765771205716"></a><a name="p765771205716"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.3 "><p id="p16657181155715"><a name="p16657181155715"></a><a name="p16657181155715"></a><em id="i116579117574"><a name="i116579117574"></a><a name="i116579117574"></a>字典数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="47.95520447955205%" headers="mcps1.2.5.1.4 "><p id="p965771145711"><a name="p965771145711"></a><a name="p965771145711"></a>带宽对象</p>
    </td>
    </tr>
    <tr id="row36589119571"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.1 "><p id="p1265815112573"><a name="p1265815112573"></a><a name="p1265815112573"></a>extendParam</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p186581217571"><a name="p186581217571"></a><a name="p186581217571"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.3 "><p id="p965861175711"><a name="p965861175711"></a><a name="p965861175711"></a><em id="i146588165713"><a name="i146588165713"></a><a name="i146588165713"></a>字典数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="47.95520447955205%" headers="mcps1.2.5.1.4 "><p id="p14658615577"><a name="p14658615577"></a><a name="p14658615577"></a>扩展参数，用于包周期资源申请。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicip字段说明

    <a name="table91041517574"></a>
    <table><thead align="left"><tr id="row2065811135712"><th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.5.1.1"><p id="p12658181125714"><a name="p12658181125714"></a><a name="p12658181125714"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.2"><p id="p166581415574"><a name="p166581415574"></a><a name="p166581415574"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="p1965801105715"><a name="p1965801105715"></a><a name="p1965801105715"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.5.1.4"><p id="p56582105713"><a name="p56582105713"></a><a name="p56582105713"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1065821115717"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="p106581111575"><a name="p106581111575"></a><a name="p106581111575"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="p8658916571"><a name="p8658916571"></a><a name="p8658916571"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p18658513579"><a name="p18658513579"></a><a name="p18658513579"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="ul9658911575"></a><a name="ul9658911575"></a><ul id="ul9658911575"><li>功能说明：弹性公网IP的类型</li><li>取值范围：<em id="i1356114110344"><a name="i1356114110344"></a><a name="i1356114110344"></a>5_telcom</em><em id="i1656174163415"><a name="i1656174163415"></a><a name="i1656174163415"></a>，5_union</em><em id="i0564419348"><a name="i0564419348"></a><a name="i0564419348"></a>，5_bgp</em><em id="i856194123415"><a name="i856194123415"></a><a name="i856194123415"></a>，5_sbgp</em><a name="ul517646113412"></a><a name="ul517646113412"></a><ul id="ul517646113412"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_sbgp</li><li>华东-上海二：5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li></ul>
    </li><li>约束：必须是系统具体支持的类型</li></ul>
    </td>
    </tr>
    <tr id="row2935112184111"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="p1661484872917"><a name="p1661484872917"></a><a name="p1661484872917"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="p1861404882912"><a name="p1861404882912"></a><a name="p1861404882912"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p1661413481295"><a name="p1661413481295"></a><a name="p1661413481295"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="ul1116316117358"></a><a name="ul1116316117358"></a><ul id="ul1116316117358"><li>取值范围：4、6，分别表示创建ipv4和ipv6，没有时默认创建ipv4</li><li>约束：必须是系统具体支持的类型</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  bandwidth字段说明

    <a name="table15129191175710"></a>
    <table><thead align="left"><tr id="row1665918116579"><th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.5.1.1"><p id="p765971205718"><a name="p765971205718"></a><a name="p765971205718"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.2"><p id="p18659111125710"><a name="p18659111125710"></a><a name="p18659111125710"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="p965901145714"><a name="p965901145714"></a><a name="p965901145714"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.5.1.4"><p id="p26593115712"><a name="p26593115712"></a><a name="p26593115712"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row96591313578"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="p86597165720"><a name="p86597165720"></a><a name="p86597165720"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="p1165971175715"><a name="p1165971175715"></a><a name="p1165971175715"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p165918117578"><a name="p165918117578"></a><a name="p165918117578"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="ul4651549103511"></a><a name="ul4651549103511"></a><ul id="ul4651549103511"><li>功能说明：带宽名称</li><li>取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li><li>约束：<a name="ul56861953103518"></a><a name="ul56861953103518"></a><ul id="ul56861953103518"><li>如果share_type是PER，该字段是必选。</li><li>如果bandwidth对象的id有值，该字段被忽略。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row56591115718"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="p8659101115716"><a name="p8659101115716"></a><a name="p8659101115716"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="p26591318572"><a name="p26591318572"></a><a name="p26591318572"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p4659181175718"><a name="p4659181175718"></a><a name="p4659181175718"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="ul9790510185"></a><a name="ul9790510185"></a><ul id="ul9790510185"><li>功能说明：带宽大小</li><li>取值范围：默认1Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。</li><li>约束：share_type取值PER时，该字段必选。如果bandwidth对象的id有值，该字段被忽略。</li><li>注意：调整带宽时的最小单位会根据带宽范围不同存在差异。<a name="ul4773151615366"></a><a name="ul4773151615366"></a><ul id="ul4773151615366"><li>小于等于300Mbit/s：默认最小单位为1Mbit/s。</li><li>300Mbit/s~1000Mbit/s：默认最小单位为50Mbit/s。</li><li>大于1000Mbit/s：默认最小单位为500Mbit/s。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row565991115718"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="p196595175716"><a name="p196595175716"></a><a name="p196595175716"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="p126597105713"><a name="p126597105713"></a><a name="p126597105713"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p196606165717"><a name="p196606165717"></a><a name="p196606165717"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="ul940614814366"></a><a name="ul940614814366"></a><ul id="ul940614814366"><li>功能说明：使用已有的共享带宽创建IP</li><li>取值范围：共享带宽ID</li><li>约束：<a name="ul3277456133617"></a><a name="ul3277456133617"></a><ul id="ul3277456133617"><li>WHOLE类型的带宽ID；</li><li>在预付费的情况下，不填该值。该字段取空字符串时，会被忽略。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row196601419579"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="p1166021105718"><a name="p1166021105718"></a><a name="p1166021105718"></a>share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="p19660316577"><a name="p19660316577"></a><a name="p19660316577"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p5660919572"><a name="p5660919572"></a><a name="p5660919572"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="ul850110171372"></a><a name="ul850110171372"></a><ul id="ul850110171372"><li>功能说明：带宽类型</li><li>取值范围：PER，WHOLE。取值为PER，表示独享带宽。</li><li>使用已有带宽创建IP时，该字段的值，以带宽的共享类型为准。</li><li>约束：在预付费的情况下，只能使用PER类型</li></ul>
    </td>
    </tr>
    <tr id="row1660131135719"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="p96604119574"><a name="p96604119574"></a><a name="p96604119574"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="p066010175715"><a name="p066010175715"></a><a name="p066010175715"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p1166021195720"><a name="p1166021195720"></a><a name="p1166021195720"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="ul48781258153710"></a><a name="ul48781258153710"></a><ul id="ul48781258153710"><li>功能说明：计费模式，按流量计费或者按带宽计费。</li><li>取值范围：bandwidth，traffic，默认是bandwidth。取值为traffic，表示流量计费。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  extendParam字段说明：

    <a name="table1616617135712"></a>
    <table><thead align="left"><tr id="row1666011115575"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.2.5.1.1"><p id="p19660131125711"><a name="p19660131125711"></a><a name="p19660131125711"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.131313131313133%" id="mcps1.2.5.1.2"><p id="p866014175712"><a name="p866014175712"></a><a name="p866014175712"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.21212121212121%" id="mcps1.2.5.1.3"><p id="p12660111125715"><a name="p12660111125715"></a><a name="p12660111125715"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.5.1.4"><p id="p1866091105712"><a name="p1866091105712"></a><a name="p1866091105712"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1066011118573"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p66604118574"><a name="p66604118574"></a><a name="p66604118574"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="p2660111135718"><a name="p2660111135718"></a><a name="p2660111135718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.5.1.3 "><p id="p8660111115715"><a name="p8660111115715"></a><a name="p8660111115715"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="ul4848115153813"></a><a name="ul4848115153813"></a><ul id="ul4848115153813"><li>功能说明：付费方式（预付费、按需付费；预付费，即包周期付费）</li><li>取值范围：<a name="ul169751157183817"></a><a name="ul169751157183817"></a><ul id="ul169751157183817"><li>prePaid -预付费，即包年包月；</li><li>postPaid -后付费，即按需付费；</li><li>默认值是postPaid。</li></ul>
    </li><li>后付费的场景下，extendParam的其他字段都会被忽略。</li></ul>
    </td>
    </tr>
    <tr id="row66611219574"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p1666120145712"><a name="p1666120145712"></a><a name="p1666120145712"></a>period_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="p1666131105719"><a name="p1666131105719"></a><a name="p1666131105719"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.5.1.3 "><p id="p76616185712"><a name="p76616185712"></a><a name="p76616185712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="ul182664270396"></a><a name="ul182664270396"></a><ul id="ul182664270396"><li>功能说明：订购资源的周期类型（包年、包月等）。</li><li>取值范围：<a name="ul1188493318393"></a><a name="ul1188493318393"></a><ul id="ul1188493318393"><li>month-月</li><li>year-年</li></ul>
    </li><li>约束：<p id="p1027114324528"><a name="p1027114324528"></a><a name="p1027114324528"></a>如果用包周期共享带宽创建时（即携带共享带宽id创建弹性公网IP）此字段可不填。付费方式是预付费且不是使用共享带宽创建IP时，该字段必选；</p>
    </li></ul>
    <p id="p1979334215564"><a name="p1979334215564"></a><a name="p1979334215564"></a>使用共享带宽创建IP时，带宽资源到期时间与IP的到期时间相同。</p>
    </td>
    </tr>
    <tr id="row166111135717"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p12661318573"><a name="p12661318573"></a><a name="p12661318573"></a>period_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="p36616113576"><a name="p36616113576"></a><a name="p36616113576"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.5.1.3 "><p id="p166611514573"><a name="p166611514573"></a><a name="p166611514573"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="ul4447175653915"></a><a name="ul4447175653915"></a><ul id="ul4447175653915"><li>功能说明：订购周期数</li><li>取值范围：(后续会随运营策略变化)<a name="ul52991518407"></a><a name="ul52991518407"></a><ul id="ul52991518407"><li>period_type为month时，为[1,9]，</li><li>period_type为year时，为[1,1]</li></ul>
    </li><li>约束：同period_type约束。</li></ul>
    </td>
    </tr>
    <tr id="row1666191155718"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p176615185712"><a name="p176615185712"></a><a name="p176615185712"></a>is_auto_renew</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="p1166112125711"><a name="p1166112125711"></a><a name="p1166112125711"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.5.1.3 "><p id="p966110165717"><a name="p966110165717"></a><a name="p966110165717"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="ul1059612233404"></a><a name="ul1059612233404"></a><ul id="ul1059612233404"><li>功能说明：是否自动续订</li><li>取值范围：<p id="p437113598116"><a name="p437113598116"></a><a name="p437113598116"></a>false：不自动续订；true：自动续订；默认值：false</p>
    </li><li>约束：<p id="p797817497111"><a name="p797817497111"></a><a name="p797817497111"></a>到期后，默认自动续订1个月（自动续订时间后续可能会变化），详情可联系客服咨询。</p>
    </li></ul>
    </td>
    </tr>
    <tr id="row566112118576"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p166111105711"><a name="p166111105711"></a><a name="p166111105711"></a>is_auto_pay</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="p7661215578"><a name="p7661215578"></a><a name="p7661215578"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.2.5.1.3 "><p id="p266218155720"><a name="p266218155720"></a><a name="p266218155720"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="ul781495117401"></a><a name="ul781495117401"></a><ul id="ul781495117401"><li>功能说明：下单订购后，是否自动从客户的账户中支付；默认是“不自动支付”</li><li>取值范围：<a name="ul1754865674019"></a><a name="ul1754865674019"></a><ul id="ul1754865674019"><li>true：是（自动支付，从账户余额自动扣费）</li><li>false：否（默认值，只提交订单不支付，需要客户手动去支付）</li></ul>
    </li><li>约束：<p id="p483505155946"><a name="p483505155946"></a><a name="p483505155946"></a>自动支付时，只能使用账户的现金支付；如果要使用代金券，请选择不自动支付，然后在用户费用中心，选择代金券支付。</p>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例1

    创建包周期独占带宽和弹性公网IP，大小1Mb，周期1个月。不自动续费，不自动扣费。

    ```
    {
        "publicip": {
            "type": "5_bgp"
        },
        "bandwidth": {
            "name": "bw_666",
            "size": 1,
            "share_type": "PER",
            "charge_mode": "bandwidth"
        },
        "extendParam": {
            "charge_mode": "prePaid",
            "period_type": "month",
            "period_num": 1,
            "is_auto_renew": "false",
            "is_auto_pay": "true"
        }
    }
    ```

-   请求样例2

    创建按需的IP、带宽；extendParam扩展字段，不填即可。

    ```
    {
        "publicip": {
            "type": "5_bgp"
        },
        "bandwidth": {
            "name": "bw_666",
            "size": 1,
            "share_type": "PER",
            "charge_mode": "bandwidth"
        }
    }
    ```


## 响应消息<a name="section4196111195719"></a>

-   响应参数

    <a name="table719831105710"></a>
    <table><thead align="left"><tr id="row206633110574"><th class="cellrowborder" valign="top" width="18.08%" id="mcps1.1.4.1.1"><p id="p116636185715"><a name="p116636185715"></a><a name="p116636185715"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.3%" id="mcps1.1.4.1.2"><p id="p1766313112570"><a name="p1766313112570"></a><a name="p1766313112570"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.620000000000005%" id="mcps1.1.4.1.3"><p id="p066391195720"><a name="p066391195720"></a><a name="p066391195720"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row7663161195710"><td class="cellrowborder" valign="top" width="18.08%" headers="mcps1.1.4.1.1 "><p id="p4663112575"><a name="p4663112575"></a><a name="p4663112575"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.1.4.1.2 "><p id="p176632120574"><a name="p176632120574"></a><a name="p176632120574"></a>字典数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.620000000000005%" headers="mcps1.1.4.1.3 "><p id="p1266319110571"><a name="p1266319110571"></a><a name="p1266319110571"></a>弹性公网IP对象（后付费场景返回对象）</p>
    </td>
    </tr>
    <tr id="row196635135712"><td class="cellrowborder" valign="top" width="18.08%" headers="mcps1.1.4.1.1 "><p id="p1366441185715"><a name="p1366441185715"></a><a name="p1366441185715"></a>order_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.1.4.1.2 "><p id="p1966419105711"><a name="p1966419105711"></a><a name="p1966419105711"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.620000000000005%" headers="mcps1.1.4.1.3 "><p id="p566413115570"><a name="p566413115570"></a><a name="p566413115570"></a>订单号（预付费场景返回该字段）</p>
    </td>
    </tr>
    <tr id="row341910754414"><td class="cellrowborder" valign="top" width="18.08%" headers="mcps1.1.4.1.1 "><p id="p05181714414"><a name="p05181714414"></a><a name="p05181714414"></a>publicip_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.1.4.1.2 "><p id="p175181794417"><a name="p175181794417"></a><a name="p175181794417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.620000000000005%" headers="mcps1.1.4.1.3 "><p id="p25191774418"><a name="p25191774418"></a><a name="p25191774418"></a>弹性公网IP的ID</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  publicip字段说明

    <a name="table12207101195717"></a>
    <table><thead align="left"><tr id="row86647165710"><th class="cellrowborder" valign="top" width="18.781878187818783%" id="mcps1.2.4.1.1"><p id="p146642116578"><a name="p146642116578"></a><a name="p146642116578"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.802480248024803%" id="mcps1.2.4.1.2"><p id="p966461125710"><a name="p966461125710"></a><a name="p966461125710"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.41564156415642%" id="mcps1.2.4.1.3"><p id="p86642018575"><a name="p86642018575"></a><a name="p86642018575"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row19664316570"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="p166419135719"><a name="p166419135719"></a><a name="p166419135719"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="p766410195716"><a name="p766410195716"></a><a name="p766410195716"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="p36641516576"><a name="p36641516576"></a><a name="p36641516576"></a>弹性公网IP唯一标识</p>
    </td>
    </tr>
    <tr id="row1266412113577"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="p196641195712"><a name="p196641195712"></a><a name="p196641195712"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="p466416125717"><a name="p466416125717"></a><a name="p466416125717"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><a name="ul19116513422"></a><a name="ul19116513422"></a><ul id="ul19116513422"><li>功能说明：弹性公网IP的状态</li><li>取值范围：<a name="ul15948194512578"></a><a name="ul15948194512578"></a><ul id="ul15948194512578"><li>冻结FREEZED</li><li>绑定失败BIND_ERROR</li><li>绑定中BINDING</li><li>释放中PENDING_DELETE</li><li>创建中PENDING_CREATE</li><li>创建中NOTIFYING</li><li>释放中NOTIFY_DELETE</li><li>更新中PENDING_UPDATE</li><li>未绑定DOWN</li><li>绑定ACTIVE</li><li>绑定ELB</li><li>失败ERROR</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row146646155711"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="p46645118579"><a name="p46645118579"></a><a name="p46645118579"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="p66644114572"><a name="p66644114572"></a><a name="p66644114572"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="p166641110572"><a name="p166641110572"></a><a name="p166641110572"></a>弹性公网IP的类型</p>
    </td>
    </tr>
    <tr id="row666491145710"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="p36645114579"><a name="p36645114579"></a><a name="p36645114579"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="p196641014573"><a name="p196641014573"></a><a name="p196641014573"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="p5664181115719"><a name="p5664181115719"></a><a name="p5664181115719"></a>申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="row88911219154214"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="p174765913710"><a name="p174765913710"></a><a name="p174765913710"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="p18476149163714"><a name="p18476149163714"></a><a name="p18476149163714"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="p1447614916377"><a name="p1447614916377"></a><a name="p1447614916377"></a>IPv4时无此字段，IPv6时为申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="row933062812445"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="p171101456172118"><a name="p171101456172118"></a><a name="p171101456172118"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="p1811012569218"><a name="p1811012569218"></a><a name="p1811012569218"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="p1211011564217"><a name="p1211011564217"></a><a name="p1211011564217"></a>IP版本信息，取值范围是4和6</p>
    </td>
    </tr>
    <tr id="row366410119579"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="p46646115713"><a name="p46646115713"></a><a name="p46646115713"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="p66640115716"><a name="p66640115716"></a><a name="p66640115716"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="p66641017571"><a name="p66641017571"></a><a name="p66641017571"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row1966411195714"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="p126656118578"><a name="p126656118578"></a><a name="p126656118578"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="p666517111573"><a name="p666517111573"></a><a name="p666517111573"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="p166519135713"><a name="p166519135713"></a><a name="p166519135713"></a>弹性公网IP申请时间</p>
    </td>
    </tr>
    <tr id="row56651165710"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="p46651711577"><a name="p46651711577"></a><a name="p46651711577"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="p16665714575"><a name="p16665714575"></a><a name="p16665714575"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="p36659155710"><a name="p36659155710"></a><a name="p36659155710"></a>带宽大小</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例1

    按需场景

    ```
    {
        "publicip": {
            "id": "f588ccfa-8750-4d7c-bf5d-2ede24414706",
            "status": "PENDING_CREATE",
            "type": "5_bgp",
            "public_ip_address": "161.17.101.7",
            "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
            "create_time": "2015-07-16 04:10:52",
            "bandwidth_size": 0,
            "ip_version": 4
        }
    }
    ```


-   响应样例2

    包周期场景

    ```
    {
        "order_id": "CS1802081410IMDRN",
        "publicip_id": "f588ccfa-8750-4d7c-bf5d-2ede24414706"
    }
    ```


## 状态码<a name="section12294185717"></a>

-   正常

    2xx

-   异常

    **表 7**  异常状态码

    <a name="table465374199568"></a>
    <table><thead align="left"><tr id="row143247899568"><th class="cellrowborder" valign="top" width="43.419999999999995%" id="mcps1.2.3.1.1"><p id="p194572529568"><a name="p194572529568"></a><a name="p194572529568"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.58%" id="mcps1.2.3.1.2"><p id="p325336049568"><a name="p325336049568"></a><a name="p325336049568"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row179762859568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p467929509568"><a name="p467929509568"></a><a name="p467929509568"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p321325679568"><a name="p321325679568"></a><a name="p321325679568"></a>服务器未能处理请求。</p>
    </td>
    </tr>
    <tr id="row207576509568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p36481159568"><a name="p36481159568"></a><a name="p36481159568"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p270619379568"><a name="p270619379568"></a><a name="p270619379568"></a>被请求的页面需要用户名和密码。</p>
    </td>
    </tr>
    <tr id="row422308469568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p652553789568"><a name="p652553789568"></a><a name="p652553789568"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p511942299568"><a name="p511942299568"></a><a name="p511942299568"></a>对被请求页面的访问被禁止。</p>
    </td>
    </tr>
    <tr id="row580948859568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p80652539568"><a name="p80652539568"></a><a name="p80652539568"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p493057379568"><a name="p493057379568"></a><a name="p493057379568"></a>服务器无法找到被请求的页面。</p>
    </td>
    </tr>
    <tr id="row410984529568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p406403309568"><a name="p406403309568"></a><a name="p406403309568"></a>405 Method Not Allowed</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p35324409568"><a name="p35324409568"></a><a name="p35324409568"></a>请求中指定的方法不被允许。</p>
    </td>
    </tr>
    <tr id="row317919689568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p250126479568"><a name="p250126479568"></a><a name="p250126479568"></a>406 Not Acceptable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p127584899568"><a name="p127584899568"></a><a name="p127584899568"></a>服务器生成的响应无法被客户端所接受。</p>
    </td>
    </tr>
    <tr id="row477175439568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p399157519568"><a name="p399157519568"></a><a name="p399157519568"></a>407 Proxy Authentication Required</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p119504089568"><a name="p119504089568"></a><a name="p119504089568"></a>用户必须首先使用代理服务器进行验证，这样请求才会被处理。</p>
    </td>
    </tr>
    <tr id="row404448129568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p548043539568"><a name="p548043539568"></a><a name="p548043539568"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p99675949568"><a name="p99675949568"></a><a name="p99675949568"></a>请求超出了服务器的等待时间。</p>
    </td>
    </tr>
    <tr id="row225994869568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p186190579568"><a name="p186190579568"></a><a name="p186190579568"></a>409 Conflict</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p317486209568"><a name="p317486209568"></a><a name="p317486209568"></a>由于冲突，请求无法被完成。</p>
    </td>
    </tr>
    <tr id="row173021289568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p592951649568"><a name="p592951649568"></a><a name="p592951649568"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p381789479568"><a name="p381789479568"></a><a name="p381789479568"></a>请求未完成。服务异常。</p>
    </td>
    </tr>
    <tr id="row80662099568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p493832159568"><a name="p493832159568"></a><a name="p493832159568"></a>501 Not Implemented</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p406174539568"><a name="p406174539568"></a><a name="p406174539568"></a>请求未完成。服务器不支持所请求的功能。</p>
    </td>
    </tr>
    <tr id="row300127579568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p151142719568"><a name="p151142719568"></a><a name="p151142719568"></a>502 Bad Gateway</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p162964299568"><a name="p162964299568"></a><a name="p162964299568"></a>请求未完成。服务器从上游服务器收到一个无效的响应。</p>
    </td>
    </tr>
    <tr id="row124501379568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p18282019568"><a name="p18282019568"></a><a name="p18282019568"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p138666109568"><a name="p138666109568"></a><a name="p138666109568"></a>请求未完成。系统暂时异常。</p>
    </td>
    </tr>
    <tr id="row576906279568"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.2.3.1.1 "><p id="p424291719568"><a name="p424291719568"></a><a name="p424291719568"></a>504 Gateway Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.2.3.1.2 "><p id="p142107999568"><a name="p142107999568"></a><a name="p142107999568"></a>网关超时。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 错误码<a name="section18721175919471"></a>

异常情况，响应body体会返回如下格式:

```
{
    "code": "VPC.0301",
    "message": " invalid input param: bandwidth id."
}
```

**表 8**  错误码

<a name="table12351210174712"></a>
<table><thead align="left"><tr id="row18233121014715"><th class="cellrowborder" valign="top" width="43.43%" id="mcps1.2.3.1.1"><p id="p9233131015477"><a name="p9233131015477"></a><a name="p9233131015477"></a>错误码</p>
</th>
<th class="cellrowborder" valign="top" width="56.57%" id="mcps1.2.3.1.2"><p id="p5233101011473"><a name="p5233101011473"></a><a name="p5233101011473"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18233610114714"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.2.3.1.1 "><p id="p1723361019474"><a name="p1723361019474"></a><a name="p1723361019474"></a>VPC.0501</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.3.1.2 "><p id="p162339102475"><a name="p162339102475"></a><a name="p162339102475"></a>publicip参数非法。</p>
</td>
</tr>
<tr id="row1223371054714"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.2.3.1.1 "><p id="p1323331074716"><a name="p1323331074716"></a><a name="p1323331074716"></a>VPC.0301</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.3.1.2 "><p id="p11233161084712"><a name="p11233161084712"></a><a name="p11233161084712"></a>带宽参数非法。</p>
</td>
</tr>
<tr id="row2235141013479"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.2.3.1.1 "><p id="p123318106479"><a name="p123318106479"></a><a name="p123318106479"></a>VPC.0531</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.3.1.2 "><p id="p1123321012471"><a name="p1123321012471"></a><a name="p1123321012471"></a>publicip扩展参数错误。</p>
</td>
</tr>
<tr id="row2023551074712"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.2.3.1.1 "><p id="p723551011475"><a name="p723551011475"></a><a name="p723551011475"></a>0000000001</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.3.1.2 "><p id="p223511109477"><a name="p223511109477"></a><a name="p223511109477"></a>系统内部错误，根据返回message分析原因。</p>
</td>
</tr>
</tbody>
</table>

