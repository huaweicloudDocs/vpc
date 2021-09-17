# 添加网络ACL规则<a name="zh-cn_topic_0051746702"></a>

## 操作场景<a name="section66699152161428"></a>

您可根据自身网络需求，在出方向和入方向添加相应规则。

一个网络ACL单方向拥有的规则数量最好不超过20条，否则可能引起网络ACL性能下降

## 操作步骤<a name="section25103352161542"></a>

1.  登录管理控制台。

1.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
2.  在系统首页，选择“网络 \> 虚拟私有云”。
3.  在左侧导航栏选择“访问控制 \> 网络ACL”。
4.  在“网络ACL”列表区域，选择网络ACL的名称列，单击目标“网络ACL名称”进入网络ACL详情页面。
5.  在入方向规则或出方向规则页签，单击“添加规则”，添加入方向或出方向规则。

    单击“+”可以依次增加多条规则。

    **表 1**  参数说明

    <a name="table746894814342"></a>
    <table><thead align="left"><tr id="row245764813417"><th class="cellrowborder" valign="top" width="19.89%" id="mcps1.2.4.1.1"><p id="p14456948183410"><a name="p14456948183410"></a><a name="p14456948183410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.730000000000004%" id="mcps1.2.4.1.2"><p id="p2456154812347"><a name="p2456154812347"></a><a name="p2456154812347"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.38%" id="mcps1.2.4.1.3"><p id="p1645724863410"><a name="p1645724863410"></a><a name="p1645724863410"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row19441848446"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="p144213414415"><a name="p144213414415"></a><a name="p144213414415"></a>类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.730000000000004%" headers="mcps1.2.4.1.2 "><p id="p13864733105816"><a name="p13864733105816"></a><a name="p13864733105816"></a>开通IPv6功能后可见。</p>
    <p id="p535711174917"><a name="p535711174917"></a><a name="p535711174917"></a><span id="text8363112322016"><a name="text8363112322016"></a><a name="text8363112322016"></a></span><span id="text1436342302019"><a name="text1436342302019"></a><a name="text1436342302019"></a>网络ACL</span>类型。必选项，单击下拉按钮可选择。目前支持“IPv4”和“IPv6”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.3 "><p id="p1844284194413"><a name="p1844284194413"></a><a name="p1844284194413"></a>IPv4</p>
    </td>
    </tr>
    <tr id="row184641148133419"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="p6457134819341"><a name="p6457134819341"></a><a name="p6457134819341"></a>策略</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.730000000000004%" headers="mcps1.2.4.1.2 "><p id="p20487105491017"><a name="p20487105491017"></a><a name="p20487105491017"></a><span id="text139841625122019"><a name="text139841625122019"></a><a name="text139841625122019"></a></span><span id="text998452592018"><a name="text998452592018"></a><a name="text998452592018"></a>网络ACL</span>策略。必选项，单击下拉按钮可选择。目前支持“允许”和“拒绝”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.3 "><p id="p1446404843410"><a name="p1446404843410"></a><a name="p1446404843410"></a>允许</p>
    </td>
    </tr>
    <tr id="row0466148153411"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="p246464863416"><a name="p246464863416"></a><a name="p246464863416"></a>协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.730000000000004%" headers="mcps1.2.4.1.2 "><p id="p124661748163411"><a name="p124661748163411"></a><a name="p124661748163411"></a><span id="text7569431172011"><a name="text7569431172011"></a><a name="text7569431172011"></a></span><span id="text125691631132020"><a name="text125691631132020"></a><a name="text125691631132020"></a>网络ACL</span>支持的协议。必选项，单击下拉按钮可选择。目前只支持选择TCP、UDP、全部、ICMP协议，当选择全部或者ICMP时，端口信息不可填写。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.3 "><p id="p114661548163415"><a name="p114661548163415"></a><a name="p114661548163415"></a>TCP</p>
    </td>
    </tr>
    <tr id="row7466248203412"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="p1546611481340"><a name="p1546611481340"></a><a name="p1546611481340"></a>源地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.730000000000004%" headers="mcps1.2.4.1.2 "><p id="p1446616487341"><a name="p1446616487341"></a><a name="p1446616487341"></a>此方向允许的源地址。可以是IP地址、IP地址段。</p>
    <p id="p144661848153418"><a name="p144661848153418"></a><a name="p144661848153418"></a>默认值为0.0.0.0/0，代表支持所有的IP地址。</p>
    <p id="p64667482345"><a name="p64667482345"></a><a name="p64667482345"></a>例如：</p>
    <a name="ul2087319185119"></a><a name="ul2087319185119"></a><ul id="ul2087319185119"><li>单个IP地址：192.168.10.10/32（IPv4地址）；2002:50::44/127（IPv6地址）</li><li>IP地址段：192.168.1.0/24（IPv4地址段）；2407:c080:802:469::/64（IPv6地址段）</li><li>所有IP地址：0.0.0.0/0（IPv4任意地址）；::/0（IPv6任意地址）</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.3 "><p id="p12466164823419"><a name="p12466164823419"></a><a name="p12466164823419"></a>0.0.0.0/0</p>
    </td>
    </tr>
    <tr id="row446624812347"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="p846664863418"><a name="p846664863418"></a><a name="p846664863418"></a>源端口范围</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.730000000000004%" headers="mcps1.2.4.1.2 "><p id="p6466104812345"><a name="p6466104812345"></a><a name="p6466104812345"></a>源端口范围，取值范围是1～65535的数字。表示某一范围时，两个数字必须以短划线分隔。例如，1-100。</p>
    <p id="p124661448153411"><a name="p124661448153411"></a><a name="p124661448153411"></a>选择TCP或UDP协议时必须填写。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.3 "><p id="p6466104818341"><a name="p6466104818341"></a><a name="p6466104818341"></a>22或22-30</p>
    </td>
    </tr>
    <tr id="row346764883414"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="p046719484349"><a name="p046719484349"></a><a name="p046719484349"></a>目的地址</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.730000000000004%" headers="mcps1.2.4.1.2 "><p id="p046712485344"><a name="p046712485344"></a><a name="p046712485344"></a>此方向允许的目的地址。可以是IP地址、IP地址段。</p>
    <p id="p10467174817345"><a name="p10467174817345"></a><a name="p10467174817345"></a>默认值为0.0.0.0/0，代表支持所有的IP地址。</p>
    <p id="p3467104893419"><a name="p3467104893419"></a><a name="p3467104893419"></a>例如：</p>
    <a name="ul184132717549"></a><a name="ul184132717549"></a><ul id="ul184132717549"><li>单个IP地址：192.168.10.10/32（IPv4地址）；2002:50::44/127（IPv6地址）</li><li>IP地址段：192.168.1.0/24（IPv4地址段）；2407:c080:802:469::/64（IPv6地址段）</li><li>所有IP地址：0.0.0.0/0（IPv4任意地址）；::/0（IPv6任意地址）</li></ul>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.3 "><p id="p104679481342"><a name="p104679481342"></a><a name="p104679481342"></a>0.0.0.0/0</p>
    </td>
    </tr>
    <tr id="row646834823419"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="p1946720489346"><a name="p1946720489346"></a><a name="p1946720489346"></a>目的端口范围</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.730000000000004%" headers="mcps1.2.4.1.2 "><p id="p646734819340"><a name="p646734819340"></a><a name="p646734819340"></a>目的端口范围，取值范围是介于1～65535的数字。表示某一范围时，两个数字必须以短划线分隔。例如，1-100。</p>
    <p id="p124671748153410"><a name="p124671748153410"></a><a name="p124671748153410"></a>选择TCP或UDP协议时必须填写。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.3 "><p id="p346854811345"><a name="p346854811345"></a><a name="p346854811345"></a>22或22-30</p>
    </td>
    </tr>
    <tr id="row2641164215415"><td class="cellrowborder" valign="top" width="19.89%" headers="mcps1.2.4.1.1 "><p id="p2641134254111"><a name="p2641134254111"></a><a name="p2641134254111"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.730000000000004%" headers="mcps1.2.4.1.2 "><p id="p55384117316"><a name="p55384117316"></a><a name="p55384117316"></a><span id="text06561944142015"><a name="text06561944142015"></a><a name="text06561944142015"></a></span><span id="text765619447206"><a name="text765619447206"></a><a name="text765619447206"></a>网络ACL</span>规则的描述信息，非必填项。</p>
    <p id="p185324110315"><a name="p185324110315"></a><a name="p185324110315"></a>描述信息内容不能超过255个字符，且不能包含&lt;、&gt;符号。</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.3 "><p id="p1364284284110"><a name="p1364284284110"></a><a name="p1364284284110"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“确定”，添加网络ACL规则。

