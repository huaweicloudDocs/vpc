# 共享VPC使用示例<a name="vpc_share_0005"></a>

某企业的云上业务主要分为两类，一类业务需要连接公网，一类业务不需要连接公网。为了规范管理各类资源，该企业使用账号A作为IT管理账号，用来管理基础公共资源，主要包括VPC、子网、路由表等。同时，账号A需要将子网共享给其他账号共同使用（账号B，账号C以及账号D），其他账号可以在子网内创建各自的资源，例如ECS、RDS以及ELB等。企业的账号和资源规划详情如[表1](#table534341514119)所示。

**图 1**  共享VPC业务规划示例<a name="fig121911186551"></a>  
![](figures/共享VPC业务规划示例.png "共享VPC业务规划示例")

**表 1**  账号及资源规划说明

<a name="table534341514119"></a>
<table><thead align="left"><tr id="row1334311513119"><th class="cellrowborder" valign="top" width="12.541254125412543%" id="mcps1.2.4.1.1"><p id="p123433158116"><a name="p123433158116"></a><a name="p123433158116"></a>账号</p>
</th>
<th class="cellrowborder" valign="top" width="24.512451245124513%" id="mcps1.2.4.1.2"><p id="p10343515213"><a name="p10343515213"></a><a name="p10343515213"></a>账号角色</p>
</th>
<th class="cellrowborder" valign="top" width="62.94629462946294%" id="mcps1.2.4.1.3"><p id="p1534313153115"><a name="p1534313153115"></a><a name="p1534313153115"></a>资源说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row173435151718"><td class="cellrowborder" valign="top" width="12.541254125412543%" headers="mcps1.2.4.1.1 "><p id="p734316153110"><a name="p734316153110"></a><a name="p734316153110"></a>账号A</p>
</td>
<td class="cellrowborder" valign="top" width="24.512451245124513%" headers="mcps1.2.4.1.2 "><p id="p1734315156110"><a name="p1734315156110"></a><a name="p1734315156110"></a>共享VPC和子网的所有者</p>
</td>
<td class="cellrowborder" valign="top" width="62.94629462946294%" headers="mcps1.2.4.1.3 "><a name="ul12568316835"></a><a name="ul12568316835"></a><ul id="ul12568316835"><li>账号A创建VPC和子网，并将子网共享给其他账号。</li><li>账号A创建NAT网关以及EIP资源，通过配置SNAT使子网Subnet-01连通公网。</li></ul>
</td>
</tr>
<tr id="row18344415815"><td class="cellrowborder" valign="top" width="12.541254125412543%" headers="mcps1.2.4.1.1 "><p id="p53441515216"><a name="p53441515216"></a><a name="p53441515216"></a>账号B</p>
</td>
<td class="cellrowborder" valign="top" width="24.512451245124513%" headers="mcps1.2.4.1.2 "><p id="p934414151711"><a name="p934414151711"></a><a name="p934414151711"></a>共享子网的使用者</p>
</td>
<td class="cellrowborder" valign="top" width="62.94629462946294%" headers="mcps1.2.4.1.3 "><p id="p934451510110"><a name="p934451510110"></a><a name="p934451510110"></a>账号B在子网Subnet-01创建ECS和RDS资源，用来部署面向公网的应用程序。</p>
</td>
</tr>
<tr id="row1845116400317"><td class="cellrowborder" valign="top" width="12.541254125412543%" headers="mcps1.2.4.1.1 "><p id="p645216402315"><a name="p645216402315"></a><a name="p645216402315"></a>账号C和账号D</p>
</td>
<td class="cellrowborder" valign="top" width="24.512451245124513%" headers="mcps1.2.4.1.2 "><p id="p154522401310"><a name="p154522401310"></a><a name="p154522401310"></a>共享子网的使用者</p>
</td>
<td class="cellrowborder" valign="top" width="62.94629462946294%" headers="mcps1.2.4.1.3 "><p id="p1545284017313"><a name="p1545284017313"></a><a name="p1545284017313"></a>账号C和账号D共同使用子网Subnet-02，在子网内创建各自业务所需的ECS、RDS以及ELB等资源，不需要连通公网。</p>
</td>
</tr>
</tbody>
</table>

同一个VPC内的不同子网网络默认互通，但是由于不同账号下的资源需要关联各自的安全组，不同安全组之间网络隔离，因此如果有网络互通需求，需要放通资源对应安全组之间的网络。

-   账号A内的资源属于安全组Sg-A。
-   账号B内的资源属于安全组Sg-B。
-   账号C内的资源属于安全组Sg-C。
-   账号D内的资源属于安全组Sg-D。

如果需要账号C和账号D内的资源网络互通，则需要在Sg-C和Sg-D的入方向分别添加以下规则：

**表 2**  放通Sg-C和Sg-D的网络

<a name="table274125420311"></a>
<table><thead align="left"><tr id="row13741154103116"><th class="cellrowborder" valign="top" width="8.73912608739126%" id="mcps1.2.8.1.1"><p id="p0251161411563"><a name="p0251161411563"></a><a name="p0251161411563"></a>安全组</p>
</th>
<th class="cellrowborder" valign="top" width="12.668733126687329%" id="mcps1.2.8.1.2"><p id="p07517548312"><a name="p07517548312"></a><a name="p07517548312"></a>方向</p>
</th>
<th class="cellrowborder" valign="top" width="13.148685131486848%" id="mcps1.2.8.1.3"><p id="p9750543315"><a name="p9750543315"></a><a name="p9750543315"></a>优先级</p>
</th>
<th class="cellrowborder" valign="top" width="13.148685131486848%" id="mcps1.2.8.1.4"><p id="p1275155418316"><a name="p1275155418316"></a><a name="p1275155418316"></a>策略</p>
</th>
<th class="cellrowborder" valign="top" width="11.62883711628837%" id="mcps1.2.8.1.5"><p id="p17545419312"><a name="p17545419312"></a><a name="p17545419312"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.788321167883208%" id="mcps1.2.8.1.6"><p id="p1775125453119"><a name="p1775125453119"></a><a name="p1775125453119"></a>协议端口</p>
</th>
<th class="cellrowborder" valign="top" width="23.87761223877612%" id="mcps1.2.8.1.7"><p id="p1975145416311"><a name="p1975145416311"></a><a name="p1975145416311"></a>源地址</p>
</th>
</tr>
</thead>
<tbody><tr id="row15751154173117"><td class="cellrowborder" valign="top" width="8.73912608739126%" headers="mcps1.2.8.1.1 "><p id="p3189122225619"><a name="p3189122225619"></a><a name="p3189122225619"></a>Sg-C</p>
</td>
<td class="cellrowborder" valign="top" width="12.668733126687329%" headers="mcps1.2.8.1.2 "><p id="p07535443115"><a name="p07535443115"></a><a name="p07535443115"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="13.148685131486848%" headers="mcps1.2.8.1.3 "><p id="p177545418314"><a name="p177545418314"></a><a name="p177545418314"></a>1</p>
</td>
<td class="cellrowborder" valign="top" width="13.148685131486848%" headers="mcps1.2.8.1.4 "><p id="p67565413115"><a name="p67565413115"></a><a name="p67565413115"></a>允许</p>
</td>
<td class="cellrowborder" valign="top" width="11.62883711628837%" headers="mcps1.2.8.1.5 "><p id="p17751454203117"><a name="p17751454203117"></a><a name="p17751454203117"></a>IPv4</p>
</td>
<td class="cellrowborder" valign="top" width="16.788321167883208%" headers="mcps1.2.8.1.6 "><p id="p275654173111"><a name="p275654173111"></a><a name="p275654173111"></a>根据业务需求选择该项。</p>
<p id="p1438842119599"><a name="p1438842119599"></a><a name="p1438842119599"></a>示例：全部协议</p>
</td>
<td class="cellrowborder" valign="top" width="23.87761223877612%" headers="mcps1.2.8.1.7 "><p id="p1675354183118"><a name="p1675354183118"></a><a name="p1675354183118"></a>安全组：Sg-D</p>
</td>
</tr>
<tr id="row667242155711"><td class="cellrowborder" valign="top" width="8.73912608739126%" headers="mcps1.2.8.1.1 "><p id="p14971715713"><a name="p14971715713"></a><a name="p14971715713"></a>Sg-D</p>
</td>
<td class="cellrowborder" valign="top" width="12.668733126687329%" headers="mcps1.2.8.1.2 "><p id="p129717705710"><a name="p129717705710"></a><a name="p129717705710"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="13.148685131486848%" headers="mcps1.2.8.1.3 "><p id="p197187105711"><a name="p197187105711"></a><a name="p197187105711"></a>1</p>
</td>
<td class="cellrowborder" valign="top" width="13.148685131486848%" headers="mcps1.2.8.1.4 "><p id="p189719711576"><a name="p189719711576"></a><a name="p189719711576"></a>允许</p>
</td>
<td class="cellrowborder" valign="top" width="11.62883711628837%" headers="mcps1.2.8.1.5 "><p id="p159713717575"><a name="p159713717575"></a><a name="p159713717575"></a>IPv4</p>
</td>
<td class="cellrowborder" valign="top" width="16.788321167883208%" headers="mcps1.2.8.1.6 "><p id="p96861547175915"><a name="p96861547175915"></a><a name="p96861547175915"></a>根据业务需求选择该项。</p>
<p id="p7686947185910"><a name="p7686947185910"></a><a name="p7686947185910"></a>示例：全部协议</p>
</td>
<td class="cellrowborder" valign="top" width="23.87761223877612%" headers="mcps1.2.8.1.7 "><p id="p18971745714"><a name="p18971745714"></a><a name="p18971745714"></a>安全组：Sg-C</p>
</td>
</tr>
</tbody>
</table>

