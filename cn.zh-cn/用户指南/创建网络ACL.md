# 创建网络ACL<a name="zh-cn_topic_0051746698"></a>

## 操作场景<a name="section61389724143414"></a>

您可以创建自定义网络ACL。默认情况下，创建的网络ACL没有关联子网和出入规则且处于停用状态。每个用户默认可以创建200个网络ACL。

## 操作步骤<a name="section4636069144430"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，选择“网络 \> 虚拟私有云”。
4.  在左侧导航栏选择“访问控制 \> 网络ACL”。
5.  在页面右侧区域，单击“创建网络ACL”。
6.  在“创建网络ACL”对话框中，根据提示，填写网络ACL参数，如[图1](#fig76501936420)所示，参数参见[表1](#table145313414319)。

    **图 1**  创建网络ACL<a name="fig76501936420"></a>  
    ![](figures/创建网络ACL.png "创建网络ACL")

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
    <td class="cellrowborder" valign="top" width="51.32%" headers="mcps1.2.4.1.2 "><p id="p105334113312"><a name="p105334113312"></a><a name="p105334113312"></a>网络ACL的名称，必填项。</p>
    <p id="p453441837"><a name="p453441837"></a><a name="p453441837"></a>网络ACL的名称只能由中文、英文字母、数字、下划线、中划线组成，且不能有空格，长度不能大于64个字符。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p15319411234"><a name="p15319411234"></a><a name="p15319411234"></a>fw-92d3</p>
    </td>
    </tr>
    <tr id="row1753541637"><td class="cellrowborder" valign="top" width="14.85%" headers="mcps1.2.4.1.1 "><p id="p16535411332"><a name="p16535411332"></a><a name="p16535411332"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.32%" headers="mcps1.2.4.1.2 "><p id="p55384117316"><a name="p55384117316"></a><a name="p55384117316"></a>网络ACL的描述信息，非必填项。</p>
    <p id="p185324110315"><a name="p185324110315"></a><a name="p185324110315"></a>描述信息内容不能超过255个字符，且不能包含&lt;、&gt;符号。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p95315415313"><a name="p95315415313"></a><a name="p95315415313"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“确定”，完成创建。

