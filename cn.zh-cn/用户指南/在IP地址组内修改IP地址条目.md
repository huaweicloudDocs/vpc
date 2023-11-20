# 在IP地址组内修改IP地址条目<a name="vpc_IPAddressGroup_0013"></a>

## 操作场景<a name="section13287171811418"></a>

本章节指导用户在IP地址组内修改IP地址条目，包括IP地址的网段以及描述信息。

## 约束与限制<a name="section11584101142314"></a>

如果IP地址组已关联至资源，修改IP地址条目的网段后，会对已关联资源的网络产生影响，并且无法恢复，请您谨慎操作。

对安全组和网络ACL来说，IP地址组相关的规则将会发生改变。

## 操作步骤<a name="section29798319613"></a>

1.  登录管理控制台。

1.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
2.  在页面左上角单击![](figures/zh-cn_image_0000001748889445.png)图标，打开服务列表，选择“网络 \> 虚拟私有云”。

    进入虚拟私有云列表页面。

3.  在左侧导航栏，选择“IP地址组”。

    进入IP地址组列表页面。

4.  在IP地址组列表中，单击目标IP地址组名称超链接。

    进入IP地址组的基本信息页面。

5.  在IP地址条目列表左上方，单击“修改”。

    弹出“修改IP地址条目”对话框。

6.  根据界面提示，修改IP地址条目信息。

    参数详细说明请参见[表1](#vpc_IPAddressGroup_0003_table15989174133114)。

    **表 1**  修改IP地址条目参数说明

    <a name="vpc_IPAddressGroup_0003_table15989174133114"></a>
    <table><thead align="left"><tr id="vpc_IPAddressGroup_0003_row99907413319"><th class="cellrowborder" valign="top" width="14.81%" id="mcps1.2.4.1.1"><p id="vpc_IPAddressGroup_0003_p49901541173110"><a name="vpc_IPAddressGroup_0003_p49901541173110"></a><a name="vpc_IPAddressGroup_0003_p49901541173110"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.35999999999999%" id="mcps1.2.4.1.2"><p id="vpc_IPAddressGroup_0003_p14990441173111"><a name="vpc_IPAddressGroup_0003_p14990441173111"></a><a name="vpc_IPAddressGroup_0003_p14990441173111"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.83%" id="mcps1.2.4.1.3"><p id="vpc_IPAddressGroup_0003_p1999094111313"><a name="vpc_IPAddressGroup_0003_p1999094111313"></a><a name="vpc_IPAddressGroup_0003_p1999094111313"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5284182342820"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="vpc_IPAddressGroup_0003_p99909414312"><a name="vpc_IPAddressGroup_0003_p99909414312"></a><a name="vpc_IPAddressGroup_0003_p99909414312"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><p id="vpc_IPAddressGroup_0003_p57241222173317"><a name="vpc_IPAddressGroup_0003_p57241222173317"></a><a name="vpc_IPAddressGroup_0003_p57241222173317"></a>IP地址组的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="vpc_IPAddressGroup_0003_p18990194112316"><a name="vpc_IPAddressGroup_0003_p18990194112316"></a><a name="vpc_IPAddressGroup_0003_p18990194112316"></a>ipGroup-A</p>
    </td>
    </tr>
    <tr id="row10740202642817"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="vpc_IPAddressGroup_0003_p199909417319"><a name="vpc_IPAddressGroup_0003_p199909417319"></a><a name="vpc_IPAddressGroup_0003_p199909417319"></a>IP类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><div class="p" id="vpc_IPAddressGroup_0003_p1990541203113"><a name="vpc_IPAddressGroup_0003_p1990541203113"></a><a name="vpc_IPAddressGroup_0003_p1990541203113"></a>IP地址组内支持的IP地址类型，创建IP地址组的时候设置该参数，不支持修改。支持的类型具体如下：<a name="vpc_IPAddressGroup_0003_ul139905412312"></a><a name="vpc_IPAddressGroup_0003_ul139905412312"></a><ul id="vpc_IPAddressGroup_0003_ul139905412312"><li>IPv4</li><li>IPv6</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="vpc_IPAddressGroup_0003_p16990104153115"><a name="vpc_IPAddressGroup_0003_p16990104153115"></a><a name="vpc_IPAddressGroup_0003_p16990104153115"></a>IPv4</p>
    </td>
    </tr>
    <tr id="row20355124819281"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p1166812519229"><a name="p1166812519229"></a><a name="p1166812519229"></a>IP地址条目</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><p id="p1566810253226"><a name="p1566810253226"></a><a name="p1566810253226"></a>必选参数。</p>
    <p id="p116687259223"><a name="p116687259223"></a><a name="p116687259223"></a>您可以在IP地址组内添加多个不同格式的IP地址，每个IP地址输入完成后，按回车键换行。</p>
    <div class="p" id="p10668162532215"><a name="p10668162532215"></a><a name="p10668162532215"></a>支持的IP格式如下：<a name="vpc_ipaddressgroup_0007_ul466819258223"></a><a name="vpc_ipaddressgroup_0007_ul466819258223"></a><ul id="vpc_ipaddressgroup_0007_ul466819258223"><li>IPv4网段：IP地址/掩码，例如192.168.0.0/16</li><li>单个IPv4地址：IP地址/掩码，例如192.168.10.10/32</li><li>IPv6网段：IP地址/掩码，例如2001:db8:a583:6e::/64</li><li>单个IPv6地址：IP地址/掩码，例如2001:db8:a583:6e::5c/128</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="p1866812522217"><a name="p1866812522217"></a><a name="p1866812522217"></a>192.168.0.0/16</p>
    <p id="p66688257220"><a name="p66688257220"></a><a name="p66688257220"></a>192.168.10.10/32</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  IP地址条目信息修改完成后，单击“确定”。

    返回IP地址条目列表，可以看到已修改的IP地址条目。

