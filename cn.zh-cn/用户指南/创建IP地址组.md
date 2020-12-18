# 创建IP地址组<a name="vpc_IPAddressGroup_0003"></a>

## 操作场景<a name="section66699152161428"></a>

创建IP地址组，添加需要统一管理的IP地址。

>![](public_sys-resources/icon-note.gif) **说明：** 
>IP地址组功能目前仅在“华北-北京四”、“华南-广州”、“西南-贵阳一”开放。

## 操作步骤<a name="section16419124611591"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，选择“网络 \> 虚拟私有云”。
4.  在左侧导航栏选择“访问控制 \> IP地址组”。
5.  单击“创建IP地址组”。
6.  配置IP地址组参数，如[表1](#table145313414319)所示。

    **表 1**  参数说明

    <a name="table145313414319"></a>
    <table><thead align="left"><tr id="row05304110314"><th class="cellrowborder" valign="top" width="14.85%" id="mcps1.2.4.1.1"><p id="p5530411336"><a name="p5530411336"></a><a name="p5530411336"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.32%" id="mcps1.2.4.1.2"><p id="p35314117314"><a name="p35314117314"></a><a name="p35314117314"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.83%" id="mcps1.2.4.1.3"><p id="p75313411731"><a name="p75313411731"></a><a name="p75313411731"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2053541033"><td class="cellrowborder" valign="top" width="14.85%" headers="mcps1.2.4.1.1 "><p id="p155314118320"><a name="p155314118320"></a><a name="p155314118320"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.32%" headers="mcps1.2.4.1.2 "><p id="p105334113312"><a name="p105334113312"></a><a name="p105334113312"></a>IP地址组的名称，必填项。</p>
    <p id="p453441837"><a name="p453441837"></a><a name="p453441837"></a>IP地址组的名称只能由中文、英文字母、数字、下划线、中划线、点组成，且不能有空格，长度不能大于64个字符。</p>
    <p id="p115913531031"><a name="p115913531031"></a><a name="p115913531031"></a>您可以自定义IP地址组名称，IP地址组的唯一性由系统分配的ID号保证。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p15319411234"><a name="p15319411234"></a><a name="p15319411234"></a>ipGroup-f7de</p>
    </td>
    </tr>
    <tr id="row189916579720"><td class="cellrowborder" valign="top" width="14.85%" headers="mcps1.2.4.1.1 "><p id="p1010018579710"><a name="p1010018579710"></a><a name="p1010018579710"></a>IP地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.32%" headers="mcps1.2.4.1.2 "><p id="p1510085719718"><a name="p1510085719718"></a><a name="p1510085719718"></a>包含的IP地址，多个IP地址使用换行隔开，最多可添加20个。</p>
    <p id="p17377408915"><a name="p17377408915"></a><a name="p17377408915"></a>例如：</p>
    <p id="p19323831495"><a name="p19323831495"></a><a name="p19323831495"></a>192.168.10.10（IP地址）</p>
    <p id="p1265484619913"><a name="p1265484619913"></a><a name="p1265484619913"></a>192.168.52.0/24（IP地址网段）</p>
    <p id="p9114646191014"><a name="p9114646191014"></a><a name="p9114646191014"></a>192.168.1.1-192.168.1.50（IP地址网段）</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p141005572715"><a name="p141005572715"></a><a name="p141005572715"></a>192.168.10.10</p>
    <p id="p3880135123816"><a name="p3880135123816"></a><a name="p3880135123816"></a>192.168.52.0/24</p>
    <p id="p8605131593810"><a name="p8605131593810"></a><a name="p8605131593810"></a>192.168.1.1</p>
    <p id="p263543211383"><a name="p263543211383"></a><a name="p263543211383"></a></p>
    </td>
    </tr>
    <tr id="row1753541637"><td class="cellrowborder" valign="top" width="14.85%" headers="mcps1.2.4.1.1 "><p id="p16535411332"><a name="p16535411332"></a><a name="p16535411332"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.32%" headers="mcps1.2.4.1.2 "><p id="p55384117316"><a name="p55384117316"></a><a name="p55384117316"></a>IP地址组的描述信息，非必填项。</p>
    <p id="p185324110315"><a name="p185324110315"></a><a name="p185324110315"></a>描述信息内容不能超过255个字符，且不能包含“&lt;”、“&gt;”符号。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p95315415313"><a name="p95315415313"></a><a name="p95315415313"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“确定”，完成创建。

