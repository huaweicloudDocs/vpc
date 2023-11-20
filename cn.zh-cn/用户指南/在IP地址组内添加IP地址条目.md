# 在IP地址组内添加IP地址条目<a name="vpc_IPAddressGroup_0007"></a>

## 操作场景<a name="section13287171811418"></a>

本章节指导用户在IP地址组内添加IP地址条目。

## 约束与限制<a name="section11584101142314"></a>

如果IP地址组已关联至资源，添加IP地址条目后，会对已关联资源的网络产生影响，并且无法恢复，请您谨慎操作。

对安全组和网络ACL来说，IP地址组相关的规则将会发生改变。

## 操作步骤<a name="section29798319613"></a>

1.  登录管理控制台。

1.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
2.  在页面左上角单击![](figures/zh-cn_image_0000001627054510.png)图标，打开服务列表，选择“网络 \> 虚拟私有云”。

    进入虚拟私有云列表页面。

3.  在左侧导航栏，选择“IP地址组”。

    进入IP地址组列表页面。

4.  在IP地址组列表中，单击目标IP地址组名称超链接。

    进入IP地址组的基本信息页面。

5.  在IP地址条目列表左上方，单击“添加”。

    弹出“添加IP地址条目”对话框。

6.  根据界面提示，在IP地址组内添加IP地址条目。

    **表 1**  IP地址组参数说明

    <a name="table19668122582213"></a>
    <table><thead align="left"><tr id="row6668172518229"><th class="cellrowborder" valign="top" width="14.81%" id="mcps1.2.4.1.1"><p id="p18668625192213"><a name="p18668625192213"></a><a name="p18668625192213"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.35999999999999%" id="mcps1.2.4.1.2"><p id="p4668112515226"><a name="p4668112515226"></a><a name="p4668112515226"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.83%" id="mcps1.2.4.1.3"><p id="p156681125162215"><a name="p156681125162215"></a><a name="p156681125162215"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row9668192522213"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p06683259229"><a name="p06683259229"></a><a name="p06683259229"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><p id="p96684253228"><a name="p96684253228"></a><a name="p96684253228"></a>IP地址组的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p2066812517224"><a name="p2066812517224"></a><a name="p2066812517224"></a>ipGroup-A</p>
    </td>
    </tr>
    <tr id="row18668925142210"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p19668122519222"><a name="p19668122519222"></a><a name="p19668122519222"></a>最大条目数</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><p id="p1966882520222"><a name="p1966882520222"></a><a name="p1966882520222"></a>必选参数。</p>
    <p id="p66684259222"><a name="p66684259222"></a><a name="p66684259222"></a>此处设置IP地址组内支持添加的IP地址条目数量，系统默认显示当前支持的最大条目数，您可以自行减少最大条目数。</p>
    <p id="p1866814255221"><a name="p1866814255221"></a><a name="p1866814255221"></a>如果需要提升IP地址组的最大条目数，您需要<a href="https://console.huaweicloud.com/ticket/#/ticketindex/createIndex" target="_blank" rel="noopener noreferrer">提交工单</a>进行申请。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p26681625172214"><a name="p26681625172214"></a><a name="p26681625172214"></a>20</p>
    </td>
    </tr>
    <tr id="row66681425122218"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p5668325182214"><a name="p5668325182214"></a><a name="p5668325182214"></a>IP类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><div class="p" id="p156687254225"><a name="p156687254225"></a><a name="p156687254225"></a>IP地址组内支持的IP地址类型，创建IP地址组的时候设置该参数，不支持修改。支持的类型具体如下：<a name="ul1766882514224"></a><a name="ul1766882514224"></a><ul id="ul1766882514224"><li>IPv4</li><li>IPv6</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p1866892514225"><a name="p1866892514225"></a><a name="p1866892514225"></a>IPv4</p>
    </td>
    </tr>
    <tr id="row156681525192219"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p1166812519229"><a name="p1166812519229"></a><a name="p1166812519229"></a>IP地址条目</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><p id="p1566810253226"><a name="p1566810253226"></a><a name="p1566810253226"></a>必选参数。</p>
    <p id="p116687259223"><a name="p116687259223"></a><a name="p116687259223"></a>您可以在IP地址组内添加多个不同格式的IP地址，每个IP地址输入完成后，按回车键换行。</p>
    <div class="p" id="p10668162532215"><a name="p10668162532215"></a><a name="p10668162532215"></a>支持的IP格式如下：<a name="ul466819258223"></a><a name="ul466819258223"></a><ul id="ul466819258223"><li>IPv4网段：IP地址/掩码，例如192.168.0.0/16</li><li>单个IPv4地址：IP地址/掩码，例如192.168.10.10/32</li><li>IPv6网段：IP地址/掩码，例如2001:db8:a583:6e::/64</li><li>单个IPv6地址：IP地址/掩码，例如2001:db8:a583:6e::5c/128</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p1866812522217"><a name="p1866812522217"></a><a name="p1866812522217"></a>192.168.0.0/16</p>
    <p id="p66688257220"><a name="p66688257220"></a><a name="p66688257220"></a>192.168.10.10/32</p>
    </td>
    </tr>
    </tbody>
    </table>

