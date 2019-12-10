# 修改网络ACL规则<a name="zh-cn_topic_0051746703"></a>

## 操作场景<a name="section66699152161428"></a>

您可根据自身网络需求，修改出方向和入方向的规则。

## 操作步骤<a name="section25103352161542"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，选择“网络 \> 虚拟私有云”。
4.  在左侧导航栏选择“访问控制 \> 网络ACL”。
5.  在“网络ACL”列表区域，选择网络ACL的名称列，单击您需要修改的“网络ACL名称”进入网络ACL详情页面。
6.  在入方向规则或出方向规则页签，单击“操作”列的“修改”，根据界面提示修改相关参数。参数说明参见[表1](#table59686157164549)。

    **表 1**  参数说明

    <a name="table59686157164549"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051746702_row245764813417"><th class="cellrowborder" valign="top" width="19.89%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0051746702_p14456948183410"><a name="zh-cn_topic_0051746702_p14456948183410"></a><a name="zh-cn_topic_0051746702_p14456948183410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.769999999999996%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0051746702_p2456154812347"><a name="zh-cn_topic_0051746702_p2456154812347"></a><a name="zh-cn_topic_0051746702_p2456154812347"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.34%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0051746702_p1645724863410"><a name="zh-cn_topic_0051746702_p1645724863410"></a><a name="zh-cn_topic_0051746702_p1645724863410"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051746702_row184641148133419"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0051746702_p6457134819341"><a name="zh-cn_topic_0051746702_p6457134819341"></a><a name="zh-cn_topic_0051746702_p6457134819341"></a>策略</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.769999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0051746702_p20487105491017"><a name="zh-cn_topic_0051746702_p20487105491017"></a><a name="zh-cn_topic_0051746702_p20487105491017"></a>网络ACL策略。必选项，单击下拉按钮可选择。目前支持“允许”和“拒绝”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0051746702_p1446404843410"><a name="zh-cn_topic_0051746702_p1446404843410"></a><a name="zh-cn_topic_0051746702_p1446404843410"></a>允许</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051746702_row0466148153411"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0051746702_p246464863416"><a name="zh-cn_topic_0051746702_p246464863416"></a><a name="zh-cn_topic_0051746702_p246464863416"></a>协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.769999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0051746702_p124661748163411"><a name="zh-cn_topic_0051746702_p124661748163411"></a><a name="zh-cn_topic_0051746702_p124661748163411"></a>网络ACL支持的协议。必选项，单击下拉按钮可选择。目前只支持选择TCP、UDP、全部、ICMP协议，当选择全部或者ICMP时，端口信息不可填写。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0051746702_p114661548163415"><a name="zh-cn_topic_0051746702_p114661548163415"></a><a name="zh-cn_topic_0051746702_p114661548163415"></a>TCP</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051746702_row7466248203412"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0051746702_p1546611481340"><a name="zh-cn_topic_0051746702_p1546611481340"></a><a name="zh-cn_topic_0051746702_p1546611481340"></a>源地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.769999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0051746702_p1446616487341"><a name="zh-cn_topic_0051746702_p1446616487341"></a><a name="zh-cn_topic_0051746702_p1446616487341"></a>此方向允许的源地址。</p>
    <p id="zh-cn_topic_0051746702_p144661848153418"><a name="zh-cn_topic_0051746702_p144661848153418"></a><a name="zh-cn_topic_0051746702_p144661848153418"></a>默认值为0.0.0.0/0，代表支持所有的IP地址。</p>
    <p id="zh-cn_topic_0051746702_p64667482345"><a name="zh-cn_topic_0051746702_p64667482345"></a><a name="zh-cn_topic_0051746702_p64667482345"></a>例如：</p>
    <p id="zh-cn_topic_0051746702_p1646613483344"><a name="zh-cn_topic_0051746702_p1646613483344"></a><a name="zh-cn_topic_0051746702_p1646613483344"></a>xxx.xxx.xxx.xxx/32（IP地址）</p>
    <p id="zh-cn_topic_0051746702_p2466154823416"><a name="zh-cn_topic_0051746702_p2466154823416"></a><a name="zh-cn_topic_0051746702_p2466154823416"></a>xxx.xxx.xxx.0/24（子网）</p>
    <p id="zh-cn_topic_0051746702_p4466194820347"><a name="zh-cn_topic_0051746702_p4466194820347"></a><a name="zh-cn_topic_0051746702_p4466194820347"></a>0.0.0.0/0（任意地址）</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0051746702_p12466164823419"><a name="zh-cn_topic_0051746702_p12466164823419"></a><a name="zh-cn_topic_0051746702_p12466164823419"></a>0.0.0.0/0</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051746702_row446624812347"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0051746702_p846664863418"><a name="zh-cn_topic_0051746702_p846664863418"></a><a name="zh-cn_topic_0051746702_p846664863418"></a>源端口范围</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.769999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0051746702_p6466104812345"><a name="zh-cn_topic_0051746702_p6466104812345"></a><a name="zh-cn_topic_0051746702_p6466104812345"></a>源端口范围，取值范围是1～65535的数字。表示某一范围时，两个数字必须以短划线分隔。例如，1-100。</p>
    <p id="zh-cn_topic_0051746702_p124661448153411"><a name="zh-cn_topic_0051746702_p124661448153411"></a><a name="zh-cn_topic_0051746702_p124661448153411"></a>选择TCP或UDP协议时必须填写。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0051746702_p6466104818341"><a name="zh-cn_topic_0051746702_p6466104818341"></a><a name="zh-cn_topic_0051746702_p6466104818341"></a>22或22-30</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051746702_row346764883414"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0051746702_p046719484349"><a name="zh-cn_topic_0051746702_p046719484349"></a><a name="zh-cn_topic_0051746702_p046719484349"></a>目的地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.769999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0051746702_p046712485344"><a name="zh-cn_topic_0051746702_p046712485344"></a><a name="zh-cn_topic_0051746702_p046712485344"></a>此方向允许的目的地址。</p>
    <p id="zh-cn_topic_0051746702_p10467174817345"><a name="zh-cn_topic_0051746702_p10467174817345"></a><a name="zh-cn_topic_0051746702_p10467174817345"></a>默认值为0.0.0.0/0，代表支持所有的IP地址。</p>
    <p id="zh-cn_topic_0051746702_p3467104893419"><a name="zh-cn_topic_0051746702_p3467104893419"></a><a name="zh-cn_topic_0051746702_p3467104893419"></a>例如：</p>
    <p id="zh-cn_topic_0051746702_p64671748143413"><a name="zh-cn_topic_0051746702_p64671748143413"></a><a name="zh-cn_topic_0051746702_p64671748143413"></a>xxx.xxx.xxx.xxx/32（IP地址）</p>
    <p id="zh-cn_topic_0051746702_p124671648113415"><a name="zh-cn_topic_0051746702_p124671648113415"></a><a name="zh-cn_topic_0051746702_p124671648113415"></a>xxx.xxx.xxx.0/24（子网）</p>
    <p id="zh-cn_topic_0051746702_p94671448203411"><a name="zh-cn_topic_0051746702_p94671448203411"></a><a name="zh-cn_topic_0051746702_p94671448203411"></a>0.0.0.0/0（任意地址）</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0051746702_p104679481342"><a name="zh-cn_topic_0051746702_p104679481342"></a><a name="zh-cn_topic_0051746702_p104679481342"></a>0.0.0.0/0</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051746702_row646834823419"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0051746702_p1946720489346"><a name="zh-cn_topic_0051746702_p1946720489346"></a><a name="zh-cn_topic_0051746702_p1946720489346"></a>目的端口范围</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.769999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0051746702_p646734819340"><a name="zh-cn_topic_0051746702_p646734819340"></a><a name="zh-cn_topic_0051746702_p646734819340"></a>目的端口范围，取值范围是介于1～65535的数字。表示某一范围时，两个数字必须以短划线分隔。例如，1-100。</p>
    <p id="zh-cn_topic_0051746702_p124671748153410"><a name="zh-cn_topic_0051746702_p124671748153410"></a><a name="zh-cn_topic_0051746702_p124671748153410"></a>选择TCP或UDP协议时必须填写。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0051746702_p346854811345"><a name="zh-cn_topic_0051746702_p346854811345"></a><a name="zh-cn_topic_0051746702_p346854811345"></a>22或22-30</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051746702_row2641164215415"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0051746702_p2641134254111"><a name="zh-cn_topic_0051746702_p2641134254111"></a><a name="zh-cn_topic_0051746702_p2641134254111"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.769999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0051746702_p55384117316"><a name="zh-cn_topic_0051746702_p55384117316"></a><a name="zh-cn_topic_0051746702_p55384117316"></a>网络ACL规则的描述信息，非必填项。</p>
    <p id="zh-cn_topic_0051746702_p185324110315"><a name="zh-cn_topic_0051746702_p185324110315"></a><a name="zh-cn_topic_0051746702_p185324110315"></a>描述信息内容不能超过255个字符，且不能包含&lt;、&gt;符号。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0051746702_p1364284284110"><a name="zh-cn_topic_0051746702_p1364284284110"></a><a name="zh-cn_topic_0051746702_p1364284284110"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  单击“确定”，修改网络ACL规则。

