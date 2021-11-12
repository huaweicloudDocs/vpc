# IPv4/IPv6双栈网络<a name="vpc_0002"></a>

## 简介<a name="section31519520369"></a>

IPv4/IPv6双栈可为您的实例（例如：ECS）提供两个不同版本的IP地址：IPv4地址和IPv6地址，这两个IP地址都可以进行内网/公网访问。

-   通过IPv4私网地址在ECS之间进行内网访问。
-   通过IPv4私网地址绑定弹性公网IP的方式访问互联网。
-   通过IPv6地址在双栈ECS之间进行内网访问（同VPC）。
-   通过IPv6地址与互联网上的IPv6网络进行访问。

## 应用场景<a name="section182413208373"></a>

如果您的应用需要为使用IPv6终端的用户提供访问服务，则您可使用：IPv6弹性公网IP或IPv6双栈。

如果您的应用既需要为使用IPv6终端的用户提供访问服务，又需要对这些访问来源进行数据分析处理，则您必须使用IPv6双栈。

如果您的应用系统与其他系统（例如：数据库系统）、应用系统之间需要使用IPv6进行内网访问，则您必须使用IPv6双栈。

IPv4/IPv6双栈网络的基本操作与之前的IPv4网络相同。只有部分页面的配置参数会略有差异，具体请以管理控制台显示为准。

## 约束与限制<a name="section20733103220"></a>

-   IPv6双栈，当前暂不收费，后续定价会根据运营商收费策略的变化进行调整。
-   只有选择支持IPv6的ECS才能体验IPv6双栈功能，请务必选择支持的区域和规格，如[表1](#table1454185617133)所示。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >ECS规格是否支持IPv6，请以管理控制台显示为准。
    >当ECS规格列表中包含“IPv6”参数，且取值为“是”时，表示该ECS规格支持IPv6，如[图1](#fig659015212192)所示。

    **表 1**  支持IPv6的ECS规格

    <a name="table1454185617133"></a>
    <table><thead align="left"><tr id="row653515568130"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p2535756151320"><a name="p2535756151320"></a><a name="p2535756151320"></a>区域</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p19535145610132"><a name="p19535145610132"></a><a name="p19535145610132"></a>可用区</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p85352562131"><a name="p85352562131"></a><a name="p85352562131"></a>规格</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row453615566134"><td class="cellrowborder" rowspan="4" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p9535205620132"><a name="p9535205620132"></a><a name="p9535205620132"></a>华北-北京四</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p653545613133"><a name="p653545613133"></a><a name="p653545613133"></a>可用区1</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p553665601319"><a name="p553665601319"></a><a name="p553665601319"></a>s6、sn3、c6</p>
    </td>
    </tr>
    <tr id="row12536195616132"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1853617568137"><a name="p1853617568137"></a><a name="p1853617568137"></a>可用区2</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p25361564139"><a name="p25361564139"></a><a name="p25361564139"></a>s6、sn3、c6</p>
    </td>
    </tr>
    <tr id="row145361056191316"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p35361956151314"><a name="p35361956151314"></a><a name="p35361956151314"></a>可用区3</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p75361856161315"><a name="p75361856161315"></a><a name="p75361856161315"></a>s6、sn3、c6</p>
    </td>
    </tr>
    <tr id="row653635691320"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p20536205618137"><a name="p20536205618137"></a><a name="p20536205618137"></a>可用区7</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p145369561134"><a name="p145369561134"></a><a name="p145369561134"></a>s6、c6</p>
    </td>
    </tr>
    <tr id="row753610561133"><td class="cellrowborder" rowspan="3" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p9536165612135"><a name="p9536165612135"></a><a name="p9536165612135"></a>华东-上海一</p>
    <p id="p553665615132"><a name="p553665615132"></a><a name="p553665615132"></a></p>
    <p id="p185376566135"><a name="p185376566135"></a><a name="p185376566135"></a></p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p953615618133"><a name="p953615618133"></a><a name="p953615618133"></a>可用区1</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p11536656191311"><a name="p11536656191311"></a><a name="p11536656191311"></a>s6、c6s、c6、c3、m6、m3</p>
    </td>
    </tr>
    <tr id="row18537135631317"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p145361356111314"><a name="p145361356111314"></a><a name="p145361356111314"></a>可用区2</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p14537165631315"><a name="p14537165631315"></a><a name="p14537165631315"></a>s6、c6、c6s、c3、m6</p>
    </td>
    </tr>
    <tr id="row14537125611317"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p853775617138"><a name="p853775617138"></a><a name="p853775617138"></a>可用区3</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p13537165691313"><a name="p13537165691313"></a><a name="p13537165691313"></a>s6、c6s、c6、m6</p>
    </td>
    </tr>
    <tr id="row1453711569138"><td class="cellrowborder" rowspan="4" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p9537115615136"><a name="p9537115615136"></a><a name="p9537115615136"></a>华南-广州</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1753795611135"><a name="p1753795611135"></a><a name="p1753795611135"></a>可用区2</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p11537956181313"><a name="p11537956181313"></a><a name="p11537956181313"></a>s6、c6</p>
    </td>
    </tr>
    <tr id="row45381562138"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p6537115611138"><a name="p6537115611138"></a><a name="p6537115611138"></a>可用区3</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p16537956141310"><a name="p16537956141310"></a><a name="p16537956141310"></a>s6、c6</p>
    </td>
    </tr>
    <tr id="row05391656141314"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p195381756131311"><a name="p195381756131311"></a><a name="p195381756131311"></a>可用区5</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p5539356141314"><a name="p5539356141314"></a><a name="p5539356141314"></a>s6、c6</p>
    </td>
    </tr>
    <tr id="row4539125618132"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p853955618133"><a name="p853955618133"></a><a name="p853955618133"></a>可用区6</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p16539205631314"><a name="p16539205631314"></a><a name="p16539205631314"></a>s6、c6</p>
    </td>
    </tr>
    <tr id="row95395561137"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p185391756181315"><a name="p185391756181315"></a><a name="p185391756181315"></a>西南-贵阳一</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p153965612131"><a name="p153965612131"></a><a name="p153965612131"></a>可用区1</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p153910566136"><a name="p153910566136"></a><a name="p153910566136"></a>s6、c6s、c6、m6</p>
    </td>
    </tr>
    <tr id="row0539256151313"><td class="cellrowborder" rowspan="2" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1953975641317"><a name="p1953975641317"></a><a name="p1953975641317"></a><span id="text453955613132"><a name="text453955613132"></a><a name="text453955613132"></a>中国-香港</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1353917561139"><a name="p1353917561139"></a><a name="p1353917561139"></a>可用区1</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p19539856191318"><a name="p19539856191318"></a><a name="p19539856191318"></a>c6</p>
    </td>
    </tr>
    <tr id="row11540556201312"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1539155610131"><a name="p1539155610131"></a><a name="p1539155610131"></a>可用区2</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p20539135631318"><a name="p20539135631318"></a><a name="p20539135631318"></a>c6</p>
    </td>
    </tr>
    <tr id="row125401556191319"><td class="cellrowborder" rowspan="2" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p12540856141312"><a name="p12540856141312"></a><a name="p12540856141312"></a>亚太-曼谷</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p165405562131"><a name="p165405562131"></a><a name="p165405562131"></a>可用区1</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p17540145620137"><a name="p17540145620137"></a><a name="p17540145620137"></a>c6</p>
    </td>
    </tr>
    <tr id="row125401156161320"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1154018561130"><a name="p1154018561130"></a><a name="p1154018561130"></a>可用区2</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p16540165661316"><a name="p16540165661316"></a><a name="p16540165661316"></a>c6</p>
    </td>
    </tr>
    <tr id="row45405563136"><td class="cellrowborder" rowspan="2" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1054095620134"><a name="p1054095620134"></a><a name="p1054095620134"></a>亚太-新加坡</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p9540205620133"><a name="p9540205620133"></a><a name="p9540205620133"></a>可用区1</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p14540145641318"><a name="p14540145641318"></a><a name="p14540145641318"></a>s6、c6s、c6、m6、i3、t6</p>
    </td>
    </tr>
    <tr id="row05401756161318"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p1554075618139"><a name="p1554075618139"></a><a name="p1554075618139"></a>可用区2</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p10540195614138"><a name="p10540195614138"></a><a name="p10540195614138"></a>s6、c6s、c6、m6、i3</p>
    </td>
    </tr>
    <tr id="row12540175617139"><td class="cellrowborder" rowspan="2" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p6540356141313"><a name="p6540356141313"></a><a name="p6540356141313"></a>拉美-圣保罗一</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p154055619133"><a name="p154055619133"></a><a name="p154055619133"></a>可用区1</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p954045611310"><a name="p954045611310"></a><a name="p954045611310"></a>s6、c6s、c6</p>
    </td>
    </tr>
    <tr id="row10541135651317"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p05411756161320"><a name="p05411756161320"></a><a name="p05411756161320"></a>可用区2</p>
    </td>
    <td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p1254119561137"><a name="p1254119561137"></a><a name="p1254119561137"></a>s6、c6s、c6</p>
    </td>
    </tr>
    </tbody>
    </table>

    **图 1**  选择支持IPv6的ECS规格<a name="fig659015212192"></a>  
    ![](figures/选择支持IPv6的ECS规格.png "选择支持IPv6的ECS规格")

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如[图1](#fig659015212192)所示，当ECS规格列表中包含“IPv6”参数，且取值为“是”时，表示该ECS规格支持IPv6。


## 基本操作<a name="section194330165219"></a>

**创建IPv6子网**

参考[为虚拟私有云创建新的子网](为虚拟私有云创建新的子网.md)创建子网，勾选“开启IPv6”，将自动为子网分配IPv6网段。该功能一旦开启，将不能关闭。暂不支持自定义设置IPv6网段。

**图 2**  创建IPv6子网<a name="fig8113192217189"></a>  
![](figures/创建IPv6子网.png "创建IPv6子网")

**查看已使用IPv6地址**

在子网列表中单击子网名称，在“已用IP地址”页签可以查看已经使用的IPv4地址和IPv6地址。

**添加IPv6安全组规则**

参考[添加安全组规则](添加安全组规则.md)添加安全组规则，类型选择“IPv6”，源地址或目的地址填写IPv6地址。

**图 3**  添加IPv6安全组规则<a name="fig10442193883817"></a>  
![](figures/添加IPv6安全组规则.png "添加IPv6安全组规则")

**添加IPv6网络ACL规则**

参考[添加网络ACL规则](添加网络ACL规则.md)添加网络ACL规则，类型选择“IPv6”，源地址或目的地址填写IPv6地址。

**图 4**  添加IPv6网络ACL规则<a name="fig374494352712"></a>  
![](figures/添加IPv6网络ACL规则.png "添加IPv6网络ACL规则")

**购买IPv6弹性公网IP**

您可以购买IPv6弹性公网IP ，或者将已有IPv4弹性公网IP转换为IPv6弹性公网IP，详情请参见[IPv6弹性公网IP](IPv6弹性公网IP.md)。

**添加IPv6弹性公网IP/IPv6双栈网卡到共享带宽**

参考[添加弹性公网IP到共享带宽](添加弹性公网IP到共享带宽.md)将IPv6弹性公网IP、IPv6双栈网卡添加到共享带宽。

**图 5**  添加IPv6双栈网卡到共享带宽<a name="fig4569191243013"></a>  
![](figures/添加IPv6双栈网卡到共享带宽.png "添加IPv6双栈网卡到共享带宽")

**添加IPv6自定义路由**

参考[添加自定义路由](添加自定义路由-1.md)添加自定义路由，其中目的地址和下一跳地址可以配置IPv4网段或IPv6网段。如果目的地址是IPv6网段，则下一跳地址暂时只能使用同一VPC内的地址。

>![](public_sys-resources/icon-note.gif) **说明：** 
>路由的目的地址为IPv6网段时，对应下一跳类型仅支持ECS实例、扩展网卡、 虚拟IP，同时下一跳资源具备IPv6地址。

**图 6**  添加路由<a name="fig1737433545914"></a>  
![](figures/添加路由.png "添加路由")

**申请IPv6虚拟IP地址**

参考[申请虚拟IP地址](申请虚拟IP地址.md)申请虚拟IP地址，其中IP类型可以选择“IPv4”或“IPv6”。

**图 7**  申请虚拟IP地址<a name="fig4553311304"></a>  
![](figures/申请虚拟IP地址.png "申请虚拟IP地址")

>![](public_sys-resources/icon-note.gif) **说明：** 
>IPv6的虚拟IP仅支持绑定一个网卡（双栈网卡），如需进行服务器的主备切换，请通过调用API方式。具体请参考[配置云服务器高可用的IPv6虚拟IP功能](https://support.huaweicloud.com/api-vpc/vpc_apieg_0006.html)。

**动态获取IPv6地址**

购买的IPv6双栈ECS实例后，您可以在ECS详情页查看自动分配的IPv6地址，也可以登录到ECS，通过**ifconfig**查看分配的IPv6地址。

如果自动分配IPv6地址失败，或者您选的其他镜像不支持自动分配IPv6地址，请参考“[动态获取IPv6地址](https://support.huaweicloud.com/usermanual-ecs/ecs_03_0508.html)”，手动获取IPv6地址。

>![](public_sys-resources/icon-note.gif) **说明：** 
>如果云服务器使用的是公共镜像，则支持情况如下：
>Linux公共镜像开启动态获取IPv6功能时，需要先判断是否支持IPv6协议栈，再判断是否已开启动态获取IPv6。目前，所有Linux公共镜像均已支持IPv6协议栈，并且Ubuntu 16操作系统已默认开启动态获取IPv6。即Ubuntu 16操作系统无需配置，其他Linux公共镜像需要执行开启动态获取IPv6的操作。

