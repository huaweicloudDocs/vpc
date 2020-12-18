# 为弹性云服务器申请和绑定弹性公网IP<a name="zh-cn_topic_0013748738"></a>

## 操作场景<a name="s974a02c09b8e44f59dcc9335de2d030a"></a>

可以通过申请弹性公网IP并将弹性公网IP绑定到弹性云服务器上，实现弹性云服务器访问公网的目的。

## 申请弹性公网IP<a name="section16739352111811"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，选择“网络 \> 弹性公网IP”。
4.  在“弹性公网IP”界面，单击“购买弹性公网IP”。
5.  根据界面提示配置参数。

    **表 1**  参数说明

    <a name="table44837990111658"></a>
    <table><thead align="left"><tr id="row63207427111658"><th class="cellrowborder" valign="top" width="31%" id="mcps1.2.4.1.1"><p id="p19527969111658"><a name="p19527969111658"></a><a name="p19527969111658"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="43.96%" id="mcps1.2.4.1.2"><p id="p38261696111658"><a name="p38261696111658"></a><a name="p38261696111658"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.040000000000003%" id="mcps1.2.4.1.3"><p id="p12189704111658"><a name="p12189704111658"></a><a name="p12189704111658"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row02151409468"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p10419756111847"><a name="p10419756111847"></a><a name="p10419756111847"></a>计费模式</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p29164913112213"><a name="p29164913112213"></a><a name="p29164913112213"></a>计费模式分为以下两种：</p>
    <a name="ul40900084113350"></a><a name="ul40900084113350"></a><ul id="ul40900084113350"><li>包年/包月</li><li>按需计费</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p47201727111847"><a name="p47201727111847"></a><a name="p47201727111847"></a>按需计费</p>
    </td>
    </tr>
    <tr id="row24586407211236"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p19951072211236"><a name="p19951072211236"></a><a name="p19951072211236"></a>区域</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p42342941211344"><a name="p42342941211344"></a><a name="p42342941211344"></a>不同区域的资源之间内网不互通。请选择靠近您客户的区域，可以降低网络时延、提高访问速度。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p14727534142017"><a name="p14727534142017"></a><a name="p14727534142017"></a>华北-北京一</p>
    </td>
    </tr>
    <tr id="row65243563111847"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p50321163111847"><a name="p50321163111847"></a><a name="p50321163111847"></a>线路</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><a name="ul1206270693355"></a><a name="ul1206270693355"></a><ul id="ul1206270693355"><li>全动态BGP：可以根据设定的寻路协议实时自动优化网络结构，以保持客户使用的网络持续稳定、高效。</li><li>静态BGP：网络结构发生变化时，无法实时自动调整网络设置以保障用户体验。</li></ul>
    <p id="p466726161319"><a name="p466726161319"></a><a name="p466726161319"></a>更多静态BGP与全动态BGP区别信息请参见<a href="https://support.huaweicloud.com/vpc_faq/faq_bandwidth_0008.html" target="_blank" rel="noopener noreferrer">静态BGP与全动态BGP有何区别？</a></p>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p48649567111847"><a name="p48649567111847"></a><a name="p48649567111847"></a>全动态BGP</p>
    </td>
    </tr>
    <tr id="row1919105895410"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p33495085114647"><a name="p33495085114647"></a><a name="p33495085114647"></a>公网带宽</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p3678114619311"><a name="p3678114619311"></a><a name="p3678114619311"></a>选择按需计费时，需要选择公网带宽的计费方式。</p>
    <a name="ul1891882012459"></a><a name="ul1891882012459"></a><ul id="ul1891882012459"><li>按带宽计费：指定带宽上限，按使用时间计费，与使用的流量无关。适用于流量较大或较稳定场景使用。</li><li>按流量计费：指定带宽上限，按实际使用的出公网流量计费，与使用时间无关。适用于流量小或流量波动较大的场景。</li><li>加入共享带宽：带宽可以加入多个<span id="text1191813202458"><a name="text1191813202458"></a><a name="text1191813202458"></a></span><span id="text491852044510"><a name="text491852044510"></a><a name="text491852044510"></a>弹性公网IP</span>，带宽被多个<span id="text391812054515"><a name="text391812054515"></a><a name="text391812054515"></a></span><span id="text129189201455"><a name="text129189201455"></a><a name="text129189201455"></a>弹性公网IP</span>地址共用。适用于多业务流量错峰场景。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p46834114114647"><a name="p46834114114647"></a><a name="p46834114114647"></a>按带宽计费</p>
    </td>
    </tr>
    <tr id="row20646132810552"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p60664281114521"><a name="p60664281114521"></a><a name="p60664281114521"></a>带宽大小</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p6134036111658"><a name="p6134036111658"></a><a name="p6134036111658"></a>带宽大小，单位Mbit/s。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p27094928111658"><a name="p27094928111658"></a><a name="p27094928111658"></a>100</p>
    </td>
    </tr>
    <tr id="row1718915616520"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p1619020564510"><a name="p1619020564510"></a><a name="p1619020564510"></a>IPv6转换</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p9563815144420"><a name="p9563815144420"></a><a name="p9563815144420"></a>开启IPv6转换后，将提供IPv4和IPv6弹性公网IP地址，原有IPv4业务可以快速为IPv6用户提供访问能力。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p21904561056"><a name="p21904561056"></a><a name="p21904561056"></a>开启</p>
    </td>
    </tr>
    <tr id="row47841952111658"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p49992880111658"><a name="p49992880111658"></a><a name="p49992880111658"></a>带宽名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p44897586111658"><a name="p44897586111658"></a><a name="p44897586111658"></a>带宽的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p12825835111658"><a name="p12825835111658"></a><a name="p12825835111658"></a>bandwidth</p>
    </td>
    </tr>
    <tr id="row51190584211858"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p1546328421192"><a name="p1546328421192"></a><a name="p1546328421192"></a>购买时长</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p4456648021192"><a name="p4456648021192"></a><a name="p4456648021192"></a>选择包年包月计费模式时，需要选择购买时长。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p5311508821192"><a name="p5311508821192"></a><a name="p5311508821192"></a>1个月</p>
    </td>
    </tr>
    <tr id="row42527768111658"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p14351203105414"><a name="p14351203105414"></a><a name="p14351203105414"></a>购买量</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p53139340111658"><a name="p53139340111658"></a><a name="p53139340111658"></a><span id="text0559123820468"><a name="text0559123820468"></a><a name="text0559123820468"></a></span><span id="text20559338144612"><a name="text20559338144612"></a><a name="text20559338144612"></a>弹性公网IP</span>数量。</p>
    <p id="p61082105123730"><a name="p61082105123730"></a><a name="p61082105123730"></a>仅在按需计费时可以选择<span id="text0882446104613"><a name="text0882446104613"></a><a name="text0882446104613"></a></span><span id="text1788274610466"><a name="text1788274610466"></a><a name="text1788274610466"></a>弹性公网IP</span>数量。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p9319283111658"><a name="p9319283111658"></a><a name="p9319283111658"></a>1</p>
    </td>
    </tr>
    <tr id="row2882753155310"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p48192945195617"><a name="p48192945195617"></a><a name="p48192945195617"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p11314500195617"><a name="p11314500195617"></a><a name="p11314500195617"></a>用于标识<span id="text18944142610473"><a name="text18944142610473"></a><a name="text18944142610473"></a></span><span id="text119445261476"><a name="text119445261476"></a><a name="text119445261476"></a>弹性公网IP</span>地址。包括键和值。</p>
    <p id="p60989264195617"><a name="p60989264195617"></a><a name="p60989264195617"></a>标签的命名规则请参考<a href="#table36606052153313">表2</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><a name="ul35105694195617"></a><a name="ul35105694195617"></a><ul id="ul35105694195617"><li>键：Ipv4_key1</li><li>值：192.168.12.10</li></ul>
    </td>
    </tr>
    <tr id="row17886175710398"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p128872057193916"><a name="p128872057193916"></a><a name="p128872057193916"></a>企业项目</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.96%" headers="mcps1.2.4.1.2 "><p id="p4358158104112"><a name="p4358158104112"></a><a name="p4358158104112"></a>申请<span id="text197021631104717"><a name="text197021631104717"></a><a name="text197021631104717"></a></span><span id="text27021316479"><a name="text27021316479"></a><a name="text27021316479"></a>弹性公网IP</span>时，可以将<span id="text52965394478"><a name="text52965394478"></a><a name="text52965394478"></a></span><span id="text42965396476"><a name="text42965396476"></a><a name="text42965396476"></a>弹性公网IP</span>加入已启用的企业项目。</p>
    <p id="p335916813413"><a name="p335916813413"></a><a name="p335916813413"></a>企业项目管理提供了一种按企业项目管理云资源的方式，帮助您实现以企业项目为基本单元的资源及人员的统一管理，默认项目为default。</p>
    <p id="p101101523810"><a name="p101101523810"></a><a name="p101101523810"></a>关于创建和管理企业项目的详情，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0131965280.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.040000000000003%" headers="mcps1.2.4.1.3 "><p id="p688765711391"><a name="p688765711391"></a><a name="p688765711391"></a>default</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  弹性公网IP地址标签命名规则

    <a name="table36606052153313"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0068145818_rd57708e01e6443a9805ca72f554fae7f"><th class="cellrowborder" valign="top" width="18.54%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0068145818_abc7708d69440476086850b219c70efa8"><a name="zh-cn_topic_0068145818_abc7708d69440476086850b219c70efa8"></a><a name="zh-cn_topic_0068145818_abc7708d69440476086850b219c70efa8"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.39%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0068145818_a0df2f83c3277432ab05b525e4ffb1c2c"><a name="zh-cn_topic_0068145818_a0df2f83c3277432ab05b525e4ffb1c2c"></a><a name="zh-cn_topic_0068145818_a0df2f83c3277432ab05b525e4ffb1c2c"></a>规则</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0068145818_a902e732241f94e96b0b1b718cf7ed639"><a name="zh-cn_topic_0068145818_a902e732241f94e96b0b1b718cf7ed639"></a><a name="zh-cn_topic_0068145818_a902e732241f94e96b0b1b718cf7ed639"></a>样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0068145818_r95612b479088487b99e620f90b71f798"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0068145818_a7694a48138124d1daf3804556a27bfd6"><a name="zh-cn_topic_0068145818_a7694a48138124d1daf3804556a27bfd6"></a><a name="zh-cn_topic_0068145818_a7694a48138124d1daf3804556a27bfd6"></a>键</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.39%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0068145818_uac40e19ce4ac49d0913d48b334564c45"></a><a name="zh-cn_topic_0068145818_uac40e19ce4ac49d0913d48b334564c45"></a><ul id="zh-cn_topic_0068145818_uac40e19ce4ac49d0913d48b334564c45"><li>不能为空。</li><li>对于同一<span id="zh-cn_topic_0068145818_text1327415505320"><a name="zh-cn_topic_0068145818_text1327415505320"></a><a name="zh-cn_topic_0068145818_text1327415505320"></a></span><span id="zh-cn_topic_0068145818_text72759513533"><a name="zh-cn_topic_0068145818_text72759513533"></a><a name="zh-cn_topic_0068145818_text72759513533"></a>弹性公网IP</span>地址键值唯一。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0068145818_a1a10de6d67c04555a3508a8cdc3500e7"><a name="zh-cn_topic_0068145818_a1a10de6d67c04555a3508a8cdc3500e7"></a><a name="zh-cn_topic_0068145818_a1a10de6d67c04555a3508a8cdc3500e7"></a>Ipv4_key1</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0068145818_r32a79d8bde844fda8a6254383317e58f"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0068145818_a1ebd1dda592448d49631c7f099519113"><a name="zh-cn_topic_0068145818_a1ebd1dda592448d49631c7f099519113"></a><a name="zh-cn_topic_0068145818_a1ebd1dda592448d49631c7f099519113"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.39%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0068145818_uaf17b1ea9b9a4e58b95cafefa2898283"></a><a name="zh-cn_topic_0068145818_uaf17b1ea9b9a4e58b95cafefa2898283"></a><ul id="zh-cn_topic_0068145818_uaf17b1ea9b9a4e58b95cafefa2898283"><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0068145818_a21a035aeb72143f5ab0fd45a08248d08"><a name="zh-cn_topic_0068145818_a21a035aeb72143f5ab0fd45a08248d08"></a><a name="zh-cn_topic_0068145818_a21a035aeb72143f5ab0fd45a08248d08"></a>192.168.12.10</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >-   对于按需计费的弹性公网IP，当带宽类型选择“共享带宽”时，只能在“带宽名称”的下拉选项中选择已有的共享带宽加入。如果带宽名称不可选，说明您没有可用共享带宽，请先创建。
    >-   独享带宽与共享带宽不支持直接互相转换，但针对按需计费的弹性公网IP，您可以购买一个共享带宽，进行如下操作：
    >    -   将弹性公网IP添加到共享带宽，则弹性公网IP使用共享带宽。
    >    -   将弹性公网IP移出共享带宽，则弹性公网IP使用独享带宽。

6.  单击“立即购买”。
7.  单击“提交”。

## 绑定弹性公网IP<a name="section6234163111911"></a>

1.  在“弹性公网IP”界面待绑定弹性公网IP地址所在行，单击“绑定”。
2.  选择实例。
3.  单击“确定”。

## 相关操作<a name="section10852154514166"></a>

-   [如何创建或找回指定的弹性公网IP？](https://support.huaweicloud.com/vpc_faq/faq_eip_0002.html)
-   [弹性公网IP绑定弹性云服务器后如何由外部进行访问？](https://support.huaweicloud.com/vpc_faq/vpc_faq_0020.html)
-   [弹性公网IP是否支持变更绑定的弹性云服务器？](https://support.huaweicloud.com/vpc_faq/faq_eip_0005.html)
-   [弹性云服务器关机再开机后，其绑定的弹性公网IP是否会改变？](https://support.huaweicloud.com/vpc_faq/faq_eip_0006.html)
-   [如何排查带宽超过限制？](https://support.huaweicloud.com/vpc_faq/faq_bandwidth_0002.html)
-   [EIP连接出现问题时，如何排查？](https://support.huaweicloud.com/vpc_faq/vpc_faq_0085.html)

