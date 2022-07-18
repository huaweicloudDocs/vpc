# 创建VPC流日志<a name="FlowLog_0003"></a>

## 操作场景<a name="section15598193716333"></a>

创建VPC流日志，记录虚拟私有云中的流量信息。

## 前提条件<a name="section48811154114711"></a>

在创建VPC流日志前，请确保您在云日志服务完成了如下配置：

-   创建日志组。
-   创建日志流。

云日志服务更多内容请参见[《云日志服务用户指南》](https://support.huaweicloud.com/lts/index.html)。

## 操作步骤<a name="section7359352124511"></a>

1.  登录管理控制台。


1.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。

1.  在系统首页，选择“网络 \> 虚拟私有云”。
2.  在左侧导航栏，选择“VPC流日志”。
3.  在页面右上角，单击“创建VPC流日志”，按照提示配置参数。

    **表 1**  参数说明

    <a name="table134731712211"></a>
    <table><thead align="left"><tr id="row1434717171627"><th class="cellrowborder" valign="top" width="19.24%" id="mcps1.2.4.1.1"><p id="p234731711214"><a name="p234731711214"></a><a name="p234731711214"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.7%" id="mcps1.2.4.1.2"><p id="p934711715210"><a name="p934711715210"></a><a name="p934711715210"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.06%" id="mcps1.2.4.1.3"><p id="p23473171214"><a name="p23473171214"></a><a name="p23473171214"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2034718171526"><td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.4.1.1 "><p id="p63477171520"><a name="p63477171520"></a><a name="p63477171520"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.7%" headers="mcps1.2.4.1.2 "><p id="p0347817222"><a name="p0347817222"></a><a name="p0347817222"></a>VPC流日志的名称。</p>
    <p id="p3691035194820"><a name="p3691035194820"></a><a name="p3691035194820"></a>名称只能由中文、英文字母、数字、“_”、“-”和“.”组成，且不能有空格，长度不能大于64个字符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p14347191710216"><a name="p14347191710216"></a><a name="p14347191710216"></a>flowlog-495d</p>
    </td>
    </tr>
    <tr id="row183478171729"><td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.4.1.1 "><p id="p11347141710216"><a name="p11347141710216"></a><a name="p11347141710216"></a>资源类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.7%" headers="mcps1.2.4.1.2 "><p id="p834721711219"><a name="p834721711219"></a><a name="p834721711219"></a>选择要采集流量的资源类型，目前支持网卡、子网、虚拟私有云类型。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p6347317525"><a name="p6347317525"></a><a name="p6347317525"></a>网卡</p>
    </td>
    </tr>
    <tr id="row83477171628"><td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.4.1.1 "><p id="p1081611984120"><a name="p1081611984120"></a><a name="p1081611984120"></a>选择资源</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.7%" headers="mcps1.2.4.1.2 "><p id="p143471917921"><a name="p143471917921"></a><a name="p143471917921"></a>选择需要采集流量信息的具体资源。</p>
    <div class="note" id="note81381412191719"><a name="note81381412191719"></a><a name="note81381412191719"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p111391812141715"><a name="p111391812141715"></a><a name="p111391812141715"></a>建议您选择处于开机状态的弹性云服务器。如果选择了关机状态的弹性云服务器，请在VPC流日志创建完成后，重启弹性云服务器，以便准确的记录网卡流量。</p>
    </div></div>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p4347517128"><a name="p4347517128"></a><a name="p4347517128"></a>-</p>
    </td>
    </tr>
    <tr id="row734713175216"><td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.4.1.1 "><p id="p934719178215"><a name="p934719178215"></a><a name="p934719178215"></a>采集类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.7%" headers="mcps1.2.4.1.2 "><a name="ul1934716177219"></a><a name="ul1934716177219"></a><ul id="ul1934716177219"><li>全部：采集指定资源的全部流量。</li><li>接受：采集指定资源被安全组或<span id="text11248715171311"><a name="text11248715171311"></a><a name="text11248715171311"></a></span><span id="text45551720134"><a name="text45551720134"></a><a name="text45551720134"></a>网络ACL</span>允许的流量。</li><li>拒绝：采集指定资源被<span id="text770047201316"><a name="text770047201316"></a><a name="text770047201316"></a></span><span id="text167001772131"><a name="text167001772131"></a><a name="text167001772131"></a>网络ACL</span>拒绝的流量。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p93471617626"><a name="p93471617626"></a><a name="p93471617626"></a>全部</p>
    </td>
    </tr>
    <tr id="row143475171327"><td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.4.1.1 "><p id="p734771710219"><a name="p734771710219"></a><a name="p734771710219"></a>日志组</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.7%" headers="mcps1.2.4.1.2 "><p id="p16347111715218"><a name="p16347111715218"></a><a name="p16347111715218"></a>选择在云日志服务中创建的日志组。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="FlowLog_0003_p634714176216"><a name="FlowLog_0003_p634714176216"></a><a name="FlowLog_0003_p634714176216"></a>lts-group-wule</p>
    </td>
    </tr>
    <tr id="row1435820326356"><td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.4.1.1 "><p id="p1336093217351"><a name="p1336093217351"></a><a name="p1336093217351"></a>日志流</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.7%" headers="mcps1.2.4.1.2 "><p id="p73611832173519"><a name="p73611832173519"></a><a name="p73611832173519"></a>选择在云日志服务中创建的日志流。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p8918114703619"><a name="p8918114703619"></a><a name="p8918114703619"></a>lts-topic-wule</p>
    </td>
    </tr>
    <tr id="row1834761720219"><td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.4.1.1 "><p id="p113471171229"><a name="p113471171229"></a><a name="p113471171229"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.7%" headers="mcps1.2.4.1.2 "><p id="p43473171124"><a name="p43473171124"></a><a name="p43473171124"></a>VPC流日志的描述信息，非必填项。</p>
    <p id="p17347181718216"><a name="p17347181718216"></a><a name="p17347181718216"></a>描述信息内容不能超过255个字符，且不能包含“&lt;”和“&gt;”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p3347141715212"><a name="p3347141715212"></a><a name="p3347141715212"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >同一个资源在同一个日志组的同一个日志流下，只能有两个不同采集类型的VPC流日志。不能重复创建相同的VPC流日志。

4.  单击“确定”。

