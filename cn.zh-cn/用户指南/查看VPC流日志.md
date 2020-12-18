# 查看VPC流日志<a name="FlowLog_0004"></a>

## 操作场景<a name="section15598193716333"></a>

查看流日志记录详情。

捕获窗口大约为10分钟，即每10分钟输出一次流日志记录。所以流日志创建完成后，您需要等待大约10分钟，才能查看流日志记录详情。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   VPC流日志功能目前仅在“亚太-新加坡”、“华南-广州”、“亚太-曼谷”开放，且还在公测期间，请申请公测权限后使用。
>-   弹性云服务器关机状态下，不显示流日志记录。

## 操作步骤<a name="section7359352124511"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，选择“网络 \> 虚拟私有云”。
4.  在左侧导航栏，选择“VPC流日志”。
5.  找到需要查看的流日志，单击操作列的“查看日志”，在云日志服务中查看流日志记录。

    流日志格式：

    ```
    <version> <project-id> <interface-id> <srcaddr> <dstaddr> <srcport> <dstport> <protocol> <packets> <bytes> <start> <end> <action> <log-status>
    ```

    示例1：在捕获窗口中正常记录数据的流日志记录

    ```
    1 5f67944957444bd6bb4fe3b367de8f3d 1d515d18-1b36-47dc-a983-bd6512aed4bd 192.168.0.154 192.168.3.25 38929 53 17 1 96 1548752136 1548752736 ACCEPT OK
    ```

    VPC流日志版本为1，在2019年01月29日16:55:36-17:05:36这10分钟内，网卡（1d515d18-1b36-47dc-a983-bd6512aed4bd）允许流过的流量信息，由源端IP地址和端口（192.168.0.154，38929）通过UDP协议向目的端IP地址和端口（192.168.3.25，53）传输了1个数据包，所有数据包的大小为96 byte。

    示例2：在捕获窗口中未记录数据的流日志记录

    ```
    1 5f67944957444bd6bb4fe3b367de8f3d 1d515d18-1b36-47dc-a983-bd6512aed4bd - - - - - - - 1431280876 1431280934 - NODATA
    ```

    示例3：在捕获窗口中跳过了数据的流日志记录

    ```
    1 5f67944957444bd6bb4fe3b367de8f3d 1d515d18-1b36-47dc-a983-bd6512aed4bd - - - - - - - 1431280876 1431280934 - SKIPDATA
    ```

    字段含义如[表1](#table1313851722313)所示：

    **表 1**  日志字段说明

    <a name="table1313851722313"></a>
    <table><thead align="left"><tr id="row813819178239"><th class="cellrowborder" valign="top" width="21.25%" id="mcps1.2.4.1.1"><p id="p4138151722319"><a name="p4138151722319"></a><a name="p4138151722319"></a>字段</p>
    </th>
    <th class="cellrowborder" valign="top" width="38.29%" id="mcps1.2.4.1.2"><p id="p313821712314"><a name="p313821712314"></a><a name="p313821712314"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.46%" id="mcps1.2.4.1.3"><p id="p181381117112313"><a name="p181381117112313"></a><a name="p181381117112313"></a>示例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row513861742316"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p171381817152313"><a name="p171381817152313"></a><a name="p171381817152313"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p181381017102311"><a name="p181381017102311"></a><a name="p181381017102311"></a>VPC流日志版本。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p181383178234"><a name="p181383178234"></a><a name="p181383178234"></a>1</p>
    </td>
    </tr>
    <tr id="row1013818170231"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p813814175238"><a name="p813814175238"></a><a name="p813814175238"></a>project-id</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p14138171752312"><a name="p14138171752312"></a><a name="p14138171752312"></a>项目ID。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p41383177232"><a name="p41383177232"></a><a name="p41383177232"></a>5f67944957444bd6bb4fe3b367de8f3d</p>
    </td>
    </tr>
    <tr id="row51388179233"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p1138517132311"><a name="p1138517132311"></a><a name="p1138517132311"></a>interface-id</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p10138121792314"><a name="p10138121792314"></a><a name="p10138121792314"></a>为其记录流量的网卡的ID。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p13138131762311"><a name="p13138131762311"></a><a name="p13138131762311"></a>1d515d18-1b36-47dc-a983-bd6512aed4bd</p>
    </td>
    </tr>
    <tr id="row91381417172313"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p313851792312"><a name="p313851792312"></a><a name="p313851792312"></a>srcaddr</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p17138151742312"><a name="p17138151742312"></a><a name="p17138151742312"></a>源地址。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p913821715234"><a name="p913821715234"></a><a name="p913821715234"></a>192.168.0.154</p>
    </td>
    </tr>
    <tr id="row4138817182313"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p15138717162315"><a name="p15138717162315"></a><a name="p15138717162315"></a>dstaddr</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p1313821714235"><a name="p1313821714235"></a><a name="p1313821714235"></a>目的地址。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p181381017162318"><a name="p181381017162318"></a><a name="p181381017162318"></a>192.168.3.25</p>
    </td>
    </tr>
    <tr id="row11381917152316"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p1513815171239"><a name="p1513815171239"></a><a name="p1513815171239"></a>srcport</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p3138101712237"><a name="p3138101712237"></a><a name="p3138101712237"></a>源端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p31381817152318"><a name="p31381817152318"></a><a name="p31381817152318"></a>38929</p>
    </td>
    </tr>
    <tr id="row2013819179235"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p10138217122314"><a name="p10138217122314"></a><a name="p10138217122314"></a>dstport</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p17138131762314"><a name="p17138131762314"></a><a name="p17138131762314"></a>目标端口。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p121381317162319"><a name="p121381317162319"></a><a name="p121381317162319"></a>53</p>
    </td>
    </tr>
    <tr id="row121381117112313"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p1213861710233"><a name="p1213861710233"></a><a name="p1213861710233"></a>protocol</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p1513831742314"><a name="p1513831742314"></a><a name="p1513831742314"></a>IANA协议编号。有关更多信息，请参阅<a href="http://www.iana.org/assignments/protocol-numbers/protocol-numbers.xhtml" target="_blank" rel="noopener noreferrer">Internet 协议编号</a>。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p3138171792310"><a name="p3138171792310"></a><a name="p3138171792310"></a>17</p>
    </td>
    </tr>
    <tr id="row2138171719237"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p113801772317"><a name="p113801772317"></a><a name="p113801772317"></a>packets</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p9138171710235"><a name="p9138171710235"></a><a name="p9138171710235"></a>数据包的数量。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p6138171720239"><a name="p6138171720239"></a><a name="p6138171720239"></a>1</p>
    </td>
    </tr>
    <tr id="row313811178234"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p171381517112312"><a name="p171381517112312"></a><a name="p171381517112312"></a>bytes</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p813861716230"><a name="p813861716230"></a><a name="p813861716230"></a>数据包的大小。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p6138121792314"><a name="p6138121792314"></a><a name="p6138121792314"></a>96</p>
    </td>
    </tr>
    <tr id="row11384176232"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p71380173233"><a name="p71380173233"></a><a name="p71380173233"></a>start</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p513841762316"><a name="p513841762316"></a><a name="p513841762316"></a>捕获窗口启动的时间，采用Unix秒的格式。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p61381178236"><a name="p61381178236"></a><a name="p61381178236"></a>1548752136</p>
    </td>
    </tr>
    <tr id="row17138121720239"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p1313819174239"><a name="p1313819174239"></a><a name="p1313819174239"></a>end</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p11138017112317"><a name="p11138017112317"></a><a name="p11138017112317"></a>捕获窗口结束的时间，采用Unix秒的格式。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p1313821782316"><a name="p1313821782316"></a><a name="p1313821782316"></a>1548752736</p>
    </td>
    </tr>
    <tr id="row11383177238"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p1138517132310"><a name="p1138517132310"></a><a name="p1138517132310"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p19138171732318"><a name="p19138171732318"></a><a name="p19138171732318"></a>与流量关联的操作：</p>
    <a name="ul151381717152318"></a><a name="ul151381717152318"></a><ul id="ul151381717152318"><li>ACCEPT：安全组或网络ACL允许记录的流量。</li><li>REJECT：网络ACL拒绝记录的流量。</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p8138617162312"><a name="p8138617162312"></a><a name="p8138617162312"></a>ACCEPT</p>
    </td>
    </tr>
    <tr id="row1713820178232"><td class="cellrowborder" valign="top" width="21.25%" headers="mcps1.2.4.1.1 "><p id="p91383171236"><a name="p91383171236"></a><a name="p91383171236"></a>log-status</p>
    </td>
    <td class="cellrowborder" valign="top" width="38.29%" headers="mcps1.2.4.1.2 "><p id="p1713861762314"><a name="p1713861762314"></a><a name="p1713861762314"></a>流日志的日志记录状态：</p>
    <a name="ul21381617122319"></a><a name="ul21381617122319"></a><ul id="ul21381617122319"><li>OK：数据正常记录到选定目标。</li><li>NODATA：捕获窗口中没有传入或传出符合“采集类型”的网卡的网络流量。</li><li>SKIPDATA：捕获窗口中跳过了一些流日志记录。这可能是由于内部容量限制或内部错误。</li></ul>
    <p id="p192827623912"><a name="p192827623912"></a><a name="p192827623912"></a>示例：</p>
    <p id="p18825610113911"><a name="p18825610113911"></a><a name="p18825610113911"></a>如果您创建VPC流日志时设置“采集类型”为“接受”，当有接受流量时，“log-status”将显示为“OK”。当没有接受的流量时，不管是否有拒绝的流量，“log-status”都将显示为“NODATA”。当有一些接受流量异常跳过时，“log-status”将显示为“SKIPDATA”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.46%" headers="mcps1.2.4.1.3 "><p id="p161381417142314"><a name="p161381417142314"></a><a name="p161381417142314"></a>OK</p>
    </td>
    </tr>
    </tbody>
    </table>


同时，您也可以在云日志服务的日志主题详情页面，在搜索框中通过关键字搜索日志。

