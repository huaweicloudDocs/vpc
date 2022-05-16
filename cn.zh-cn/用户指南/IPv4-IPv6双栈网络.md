# IPv4/IPv6双栈网络<a name="vpc_0002"></a>

## 什么是IPv4/IPv6双栈网络<a name="section31519520369"></a>

IPv4/IPv6双栈网络，表示为您的实例（例如ECS）提供两个版本的的IP地址：IPv4 IP地址和IPv6 IP地址，这两个IP地址都可以进行内网或者公网访问。以ECS为例，使用IPv4/IPv6双栈网络可实现以下功能：

-   使用IPv4私有IP地址，实现ECS在内网之间互访。
-   使用IPv4私有IP地址，通过绑定弹性公网IP的方式，实现ECS和公网之间互访。
-   使用IPv6 IP地址，实现双栈ECS在内网之间互访。
-   使用IPv6 IP地址，通过绑定带宽的方式，实现ECS和公网之间互访。

>![](public_sys-resources/icon-note.gif) **说明：** 
>创建子网时，勾选“开启IPv6”，将自动为当前子网分配IPv6网段。
>IPv4/IPv6双栈网络的基本操作与之前的IPv4网络相同。只有部分页面的配置参数会略有差异，具体请以管理控制台显示为准。

## 约束与限制<a name="section20733103220"></a>

-   IPv6双栈，当前暂不收费，后续定价会根据运营商收费策略的变化进行调整。
-   只有选择支持IPv6的ECS，才可以使用IPv4/IPv6双栈网络，请务必选择支持的区域和规格。

    您可以通过以下两种方法查看ECS哪些规格支持IPv6：

    -   通过ECS控制台查看：单击“购买弹性云服务器“，进入购买页面查看ECS规格列表。

        当ECS规格列表中包含“IPv6”参数，且取值为“是”时，表示该规格的ECS支持IPv6。

    -   通过ECS文档查看：打开《ECS产品介绍》中的[ECS规格清单](https://support.huaweicloud.com/productdesc-ecs/zh-cn_topic_0159822360.html)页面，查看ECS规格的详细介绍。


## IPv6网络的应用场景<a name="section182413208373"></a>

如果您的ECS规格支持IPv6，您可以使用IPv4/IPv6双栈网络，场景示例和资源规划如[表1](#table20563744105916)所示。

**表 1**  IPv4/IPv6双栈网络的应用场景及资源规划

<a name="table20563744105916"></a>
<table><thead align="left"><tr id="row10563044205914"><th class="cellrowborder" valign="top" width="12.198780121987799%" id="mcps1.2.5.1.1"><p id="p1756315441597"><a name="p1756315441597"></a><a name="p1756315441597"></a>应用场景</p>
</th>
<th class="cellrowborder" valign="top" width="38.54614538546144%" id="mcps1.2.5.1.2"><p id="p1456364475911"><a name="p1456364475911"></a><a name="p1456364475911"></a>场景示例</p>
</th>
<th class="cellrowborder" valign="top" width="14.47855214478552%" id="mcps1.2.5.1.3"><p id="p856374416599"><a name="p856374416599"></a><a name="p856374416599"></a>子网</p>
</th>
<th class="cellrowborder" valign="top" width="34.776522347765216%" id="mcps1.2.5.1.4"><p id="p71425413219"><a name="p71425413219"></a><a name="p71425413219"></a>ECS</p>
</th>
</tr>
</thead>
<tbody><tr id="row15631044115911"><td class="cellrowborder" valign="top" width="12.198780121987799%" headers="mcps1.2.5.1.1 "><p id="p1756334419595"><a name="p1756334419595"></a><a name="p1756334419595"></a>IPv6内网通信</p>
</td>
<td class="cellrowborder" valign="top" width="38.54614538546144%" headers="mcps1.2.5.1.2 "><p id="p956314455918"><a name="p956314455918"></a><a name="p956314455918"></a>您在ECS上部署应用，需要与其他系统（比如数据库）之间使用IPV6进行内网互访</p>
</td>
<td class="cellrowborder" valign="top" width="14.47855214478552%" headers="mcps1.2.5.1.3 "><a name="ul18873230631"></a><a name="ul18873230631"></a><ul id="ul18873230631"><li>IPv4网段</li><li>IPv6网段</li></ul>
</td>
<td class="cellrowborder" valign="top" width="34.776522347765216%" headers="mcps1.2.5.1.4 "><a name="ul166835410310"></a><a name="ul166835410310"></a><ul id="ul166835410310"><li>IPv4私有地址：用于IPv4内网通信</li><li>IPv6地址：用于IPv6内网通信</li></ul>
</td>
</tr>
<tr id="row1956304410594"><td class="cellrowborder" rowspan="2" valign="top" width="12.198780121987799%" headers="mcps1.2.5.1.1 "><p id="p55632448596"><a name="p55632448596"></a><a name="p55632448596"></a>IPv6公网通信</p>
</td>
<td class="cellrowborder" valign="top" width="38.54614538546144%" headers="mcps1.2.5.1.2 "><p id="p1856324445919"><a name="p1856324445919"></a><a name="p1856324445919"></a>您在ECS上部署应用并面向公网客户端提供服务，支持客户端通过IPv6地址访问</p>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="14.47855214478552%" headers="mcps1.2.5.1.3 "><a name="ul173501936738"></a><a name="ul173501936738"></a><ul id="ul173501936738"><li>IPv4网段</li><li>IPv6网段</li></ul>
</td>
<td class="cellrowborder" rowspan="2" valign="top" width="34.776522347765216%" headers="mcps1.2.5.1.4 "><a name="ul16386838842"></a><a name="ul16386838842"></a><ul id="ul16386838842"><li>IPv4私有地址+IPv4 EIP地址：用于IPv4公网通信</li><li>IPv6地址+共享带宽：用于IPv6公网通信</li></ul>
</td>
</tr>
<tr id="row18563174414591"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="p17563644145912"><a name="p17563644145912"></a><a name="p17563644145912"></a>您在ECS上部署应用并面向公网客户端提供服务，既要支持客户端通过IPv6地址访问，还要对这些访问来源进行数据分析</p>
</td>
</tr>
</tbody>
</table>

如果您的ECS规格不支持IPv6，您可以通过开启EIP的IPv6转换功能，实现IPv6公网通信，具体如[表2](#table105590377292)所示。

**表 2**  IPv6 EIP的应用场景及资源规划

<a name="table105590377292"></a>
<table><thead align="left"><tr id="row1455915377291"><th class="cellrowborder" valign="top" width="12.198780121987799%" id="mcps1.2.5.1.1"><p id="p155591237112916"><a name="p155591237112916"></a><a name="p155591237112916"></a>应用场景</p>
</th>
<th class="cellrowborder" valign="top" width="38.54614538546144%" id="mcps1.2.5.1.2"><p id="p255918376297"><a name="p255918376297"></a><a name="p255918376297"></a>场景示例</p>
</th>
<th class="cellrowborder" valign="top" width="14.47855214478552%" id="mcps1.2.5.1.3"><p id="p14559237132910"><a name="p14559237132910"></a><a name="p14559237132910"></a>子网</p>
</th>
<th class="cellrowborder" valign="top" width="34.776522347765216%" id="mcps1.2.5.1.4"><p id="p105590375296"><a name="p105590375296"></a><a name="p105590375296"></a>ECS</p>
</th>
</tr>
</thead>
<tbody><tr id="row14559183702918"><td class="cellrowborder" valign="top" width="12.198780121987799%" headers="mcps1.2.5.1.1 "><p id="p1559103711297"><a name="p1559103711297"></a><a name="p1559103711297"></a>IPv6公网通信</p>
</td>
<td class="cellrowborder" valign="top" width="38.54614538546144%" headers="mcps1.2.5.1.2 "><p id="p4559123742916"><a name="p4559123742916"></a><a name="p4559123742916"></a>您在ECS上部署应用并面向公网客户端提供服务，支持客户端通过IPv6地址访问</p>
</td>
<td class="cellrowborder" valign="top" width="14.47855214478552%" headers="mcps1.2.5.1.3 "><p id="p199201550113120"><a name="p199201550113120"></a><a name="p199201550113120"></a>IPv4网段</p>
</td>
<td class="cellrowborder" valign="top" width="34.776522347765216%" headers="mcps1.2.5.1.4 "><a name="ul165591737132914"></a><a name="ul165591737132914"></a><ul id="ul165591737132914"><li>IPv4私有地址</li><li>IPv4 EIP地址（开启IPv6转换）：用于IPv4和IPv6公网通信</li></ul>
</td>
</tr>
</tbody>
</table>

**图 1**  IPv6网络应用场景及资源规划<a name="fig3552642124815"></a>  
![](figures/IPv6网络应用场景及资源规划.png "IPv6网络应用场景及资源规划")

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

您可以购买IPv6弹性公网IP ，或者将已有IPv4弹性公网IP转换为IPv6弹性公网IP，详情请参见[管理IPv6弹性公网IP](管理IPv6弹性公网IP.md)。

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

