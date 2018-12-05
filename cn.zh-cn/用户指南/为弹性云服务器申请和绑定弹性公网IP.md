# 为弹性云服务器申请和绑定弹性公网IP<a name="zh-cn_topic_0013748738"></a>

## 操作场景<a name="s974a02c09b8e44f59dcc9335de2d030a"></a>

可以通过申请弹性公网IP并将弹性公网IP绑定到弹性云服务器上，实现弹性云服务器访公网的目的。

## 操作步骤<a name="section2598706202629"></a>

**申请弹性公网IP**

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)图标，选择区域和项目。
3.  在系统首页，单击“网络 \> 虚拟私有云”。
4.  在左侧导航树，单击“弹性公网IP”。
5.  在“弹性公网IP”界面，单击“购买弹性公网IP”。
6.  根据界面提示配置参数。

    **表 1**  参数说明

    <a name="table44837990111658"></a>
    <table><thead align="left"><tr id="row63207427111658"><th class="cellrowborder" valign="top" width="31%" id="mcps1.2.4.1.1"><p id="p19527969111658"><a name="p19527969111658"></a><a name="p19527969111658"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="44%" id="mcps1.2.4.1.2"><p id="p38261696111658"><a name="p38261696111658"></a><a name="p38261696111658"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.3"><p id="p12189704111658"><a name="p12189704111658"></a><a name="p12189704111658"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row24586407211236"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p19951072211236"><a name="p19951072211236"></a><a name="p19951072211236"></a>当前区域</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p42342941211344"><a name="p42342941211344"></a><a name="p42342941211344"></a>不同区域的资源之间内网不互通。请选择靠近您客户的区域，可以降低网络时延、提高访问速度。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p7226197211344"><a name="p7226197211344"></a><a name="p7226197211344"></a>华北-北京一</p>
    </td>
    </tr>
    <tr id="row65243563111847"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p50321163111847"><a name="p50321163111847"></a><a name="p50321163111847"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><a name="ul1206270693355"></a><a name="ul1206270693355"></a><ul id="ul1206270693355"><li>全动态BGP：可以根据设定的寻路协议实时自动优化网络结构，以保持客户使用的网络持续稳定、高效。</li><li>静态BGP：网络结构发生变化时，无法实时自动调整网络设置以保障用户体验。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p48649567111847"><a name="p48649567111847"></a><a name="p48649567111847"></a>全动态BGP</p>
    </td>
    </tr>
    <tr id="row30983912111847"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p10419756111847"><a name="p10419756111847"></a><a name="p10419756111847"></a>计费模式</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p29164913112213"><a name="p29164913112213"></a><a name="p29164913112213"></a>计费模式分为以下两种：</p>
    <a name="ul40900084113350"></a><a name="ul40900084113350"></a><ul id="ul40900084113350"><li>包年包月</li><li>按需计费</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p47201727111847"><a name="p47201727111847"></a><a name="p47201727111847"></a>按需计费</p>
    </td>
    </tr>
    <tr id="row6661229195610"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p48192945195617"><a name="p48192945195617"></a><a name="p48192945195617"></a>标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p11314500195617"><a name="p11314500195617"></a><a name="p11314500195617"></a>用于标示弹性公网IP地址。包括键和值。</p>
    <p id="p60989264195617"><a name="p60989264195617"></a><a name="p60989264195617"></a>标签的命名规则请参考<a href="#zh-cn_topic_0013748738__table36606052153313">表2</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><a name="ul35105694195617"></a><a name="ul35105694195617"></a><ul id="ul35105694195617"><li>键：Ipv4_key1</li><li>值：192.168.12.10</li></ul>
    </td>
    </tr>
    <tr id="row2221351111842"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p19992167111842"><a name="p19992167111842"></a><a name="p19992167111842"></a>带宽选择</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p8752793111842"><a name="p8752793111842"></a><a name="p8752793111842"></a>选择新建带宽或者使用已有带宽。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p37887648111842"><a name="p37887648111842"></a><a name="p37887648111842"></a>新建带宽</p>
    </td>
    </tr>
    <tr id="row47841952111658"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p49992880111658"><a name="p49992880111658"></a><a name="p49992880111658"></a>带宽名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p44897586111658"><a name="p44897586111658"></a><a name="p44897586111658"></a>带宽的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p12825835111658"><a name="p12825835111658"></a><a name="p12825835111658"></a>bandwidth</p>
    </td>
    </tr>
    <tr id="row48460918114647"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p33495085114647"><a name="p33495085114647"></a><a name="p33495085114647"></a>带宽类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p6450524511474"><a name="p6450524511474"></a><a name="p6450524511474"></a>带宽类型分为以下两种：</p>
    <a name="ul2039802123533"></a><a name="ul2039802123533"></a><ul id="ul2039802123533"><li>独享：带宽只能被一个弹性公网IP地址使用。</li><li>共享：带宽可以加入多个弹性公网IP，带宽被多个弹性公网IP地址共用。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p46834114114647"><a name="p46834114114647"></a><a name="p46834114114647"></a>独享。</p>
    </td>
    </tr>
    <tr id="row34748231124245"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p44298631124245"><a name="p44298631124245"></a><a name="p44298631124245"></a>计费方式</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p2244102212432"><a name="p2244102212432"></a><a name="p2244102212432"></a>按带宽计费或按流量计费</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p61941702124245"><a name="p61941702124245"></a><a name="p61941702124245"></a>按带宽计费</p>
    </td>
    </tr>
    <tr id="row48323655111658"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p60664281114521"><a name="p60664281114521"></a><a name="p60664281114521"></a>带宽大小</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p6134036111658"><a name="p6134036111658"></a><a name="p6134036111658"></a>带宽大小，单位Mbit/s。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p27094928111658"><a name="p27094928111658"></a><a name="p27094928111658"></a>100</p>
    </td>
    </tr>
    <tr id="row51190584211858"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p1546328421192"><a name="p1546328421192"></a><a name="p1546328421192"></a>购买时长</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p4456648021192"><a name="p4456648021192"></a><a name="p4456648021192"></a>选择包年包月计费模式时，需要选择购买时长。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p5311508821192"><a name="p5311508821192"></a><a name="p5311508821192"></a>1个月</p>
    </td>
    </tr>
    <tr id="row12901616175414"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p16911162545"><a name="p16911162545"></a><a name="p16911162545"></a>购买量</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p10238183312133"><a name="p10238183312133"></a><a name="p10238183312133"></a>弹性公网IP数量。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p891516155410"><a name="p891516155410"></a><a name="p891516155410"></a>1</p>
    </td>
    </tr>
    <tr id="row17886175710398"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.4.1.1 "><p id="p128872057193916"><a name="p128872057193916"></a><a name="p128872057193916"></a>企业项目</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.2.4.1.2 "><p id="p19686163713818"><a name="p19686163713818"></a><a name="p19686163713818"></a>弹性公网IP归属的企业项目，默认归属于Default项目。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.3 "><p id="p688765711391"><a name="p688765711391"></a><a name="p688765711391"></a>Default</p>
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
    <td class="cellrowborder" valign="top" width="53.39%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0068145818_uac40e19ce4ac49d0913d48b334564c45"></a><a name="zh-cn_topic_0068145818_uac40e19ce4ac49d0913d48b334564c45"></a><ul id="zh-cn_topic_0068145818_uac40e19ce4ac49d0913d48b334564c45"><li>不能为空。</li><li>对于同一弹性公网IP地址键值唯一。</li><li>长度不超过36个字符。</li><li>不能包含“=”、“*”、“&lt;”、“&gt;”、“\\”、“,”、“|”和“/”，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0068145818_a1a10de6d67c04555a3508a8cdc3500e7"><a name="zh-cn_topic_0068145818_a1a10de6d67c04555a3508a8cdc3500e7"></a><a name="zh-cn_topic_0068145818_a1a10de6d67c04555a3508a8cdc3500e7"></a>Ipv4_key1</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0068145818_r32a79d8bde844fda8a6254383317e58f"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0068145818_a1ebd1dda592448d49631c7f099519113"><a name="zh-cn_topic_0068145818_a1ebd1dda592448d49631c7f099519113"></a><a name="zh-cn_topic_0068145818_a1ebd1dda592448d49631c7f099519113"></a>值</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.39%" headers="mcps1.2.4.1.2 "><a name="zh-cn_topic_0068145818_uaf17b1ea9b9a4e58b95cafefa2898283"></a><a name="zh-cn_topic_0068145818_uaf17b1ea9b9a4e58b95cafefa2898283"></a><ul id="zh-cn_topic_0068145818_uaf17b1ea9b9a4e58b95cafefa2898283"><li>长度不超过43个字符。</li><li>不能包含“=”、“*”、“&lt;”、“&gt;”、“\\”、“,”、“|”和“/”，且首尾字符不能为空格。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0068145818_a21a035aeb72143f5ab0fd45a08248d08"><a name="zh-cn_topic_0068145818_a21a035aeb72143f5ab0fd45a08248d08"></a><a name="zh-cn_topic_0068145818_a21a035aeb72143f5ab0fd45a08248d08"></a>192.168.12.10</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >带宽只限制出方向的大小，入方向带宽当前不做限制。  
    >对于按需计费的弹性公网IP，当带宽类型选择“共享带宽”时，只能在“带宽名称”的下拉选项中选择已有的共享带宽加入。如果带宽名称不可选，说明您没有可用共享带宽，请先创建。  

7.  单击“立即购买”。
8.  单击“提交”。

    当申请选择新建带宽时，需要同时购买带宽。


**绑定**

1.  在“弹性公网IP”界面待绑定弹性公网IP地址所在行，单击“绑定”。
2.  选择实例。
3.  单击“确定”。

