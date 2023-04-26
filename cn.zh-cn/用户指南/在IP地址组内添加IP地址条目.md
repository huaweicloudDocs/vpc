# 在IP地址组内添加IP地址条目<a name="vpc_IPAddressGroup_0007"></a>

## 操作场景<a name="section13287171811418"></a>

本章节指导用户在IP地址组内添加IP地址条目。

IP地址组中已有的IP地址不支持修改，您可以参考本章节添加新的IP地址，然后[删除不需要的IP地址](删除IP地址组内的IP地址条目.md)即可。

## 约束与限制<a name="section11584101142314"></a>

如果IP地址组已关联至资源，添加IP地址条目后，会对已关联资源的网络产生影响，并且无法恢复，请您谨慎操作。

对安全组和网络ACL来说，IP地址组相关的规则将会发生改变。


## 操作步骤<a name="section29798319613"></a>

1.  登录管理控制台。


1.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
2.  在系统首页，选择“网络\>虚拟私有云”。

    进入虚拟私有云列表页面。

3.  在左侧导航栏，选择“IP地址组”。

    进入IP地址组列表页面。

4.  在IP地址组列表中，单击目标IP地址组名称超链接。

    进入IP地址组的基本信息页面。

5.  在IP地址条目列表左上方，单击“添加”。

    弹出“添加IP地址条目”对话框。

6.  根据界面提示设置IP地址组参数。

    参数详细说明请参见[表1](#vpc_IPAddressGroup_0003_table15989174133114)。

    **表 1**  IP地址组参数说明

    <a name="vpc_IPAddressGroup_0003_table15989174133114"></a>
    <table><thead align="left"><tr id="vpc_IPAddressGroup_0003_row99907413319"><th class="cellrowborder" valign="top" width="14.81%" id="mcps1.2.4.1.1"><p id="vpc_IPAddressGroup_0003_p49901541173110"><a name="vpc_IPAddressGroup_0003_p49901541173110"></a><a name="vpc_IPAddressGroup_0003_p49901541173110"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.35999999999999%" id="mcps1.2.4.1.2"><p id="vpc_IPAddressGroup_0003_p14990441173111"><a name="vpc_IPAddressGroup_0003_p14990441173111"></a><a name="vpc_IPAddressGroup_0003_p14990441173111"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.83%" id="mcps1.2.4.1.3"><p id="vpc_IPAddressGroup_0003_p1999094111313"><a name="vpc_IPAddressGroup_0003_p1999094111313"></a><a name="vpc_IPAddressGroup_0003_p1999094111313"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="vpc_IPAddressGroup_0003_row99901241203114"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="vpc_IPAddressGroup_0003_p99909414312"><a name="vpc_IPAddressGroup_0003_p99909414312"></a><a name="vpc_IPAddressGroup_0003_p99909414312"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><p id="vpc_IPAddressGroup_0003_p199024114311"><a name="vpc_IPAddressGroup_0003_p199024114311"></a><a name="vpc_IPAddressGroup_0003_p199024114311"></a>必选参数。</p>
    <p id="vpc_IPAddressGroup_0003_p57241222173317"><a name="vpc_IPAddressGroup_0003_p57241222173317"></a><a name="vpc_IPAddressGroup_0003_p57241222173317"></a>此处填写IP地址组的名称。</p>
    <a name="vpc_IPAddressGroup_0003_ul13354429153415"></a><a name="vpc_IPAddressGroup_0003_ul13354429153415"></a><ul id="vpc_IPAddressGroup_0003_ul13354429153415"><li>长度范围为1~64位。</li><li>名称由中文、英文字母、数字、下划线（_）、中划线（-）、点（.）组成。</li></ul>
    <p id="vpc_IPAddressGroup_0003_p099010413318"><a name="vpc_IPAddressGroup_0003_p099010413318"></a><a name="vpc_IPAddressGroup_0003_p099010413318"></a>您可以自定义IP地址组名称，IP地址组的唯一性由系统分配的ID号保证。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="vpc_IPAddressGroup_0003_p18990194112316"><a name="vpc_IPAddressGroup_0003_p18990194112316"></a><a name="vpc_IPAddressGroup_0003_p18990194112316"></a>ipGroup-A</p>
    </td>
    </tr>
    <tr id="vpc_IPAddressGroup_0003_row79904416315"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="vpc_IPAddressGroup_0003_p199909417319"><a name="vpc_IPAddressGroup_0003_p199909417319"></a><a name="vpc_IPAddressGroup_0003_p199909417319"></a>IP类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><p id="vpc_IPAddressGroup_0003_p6990194173112"><a name="vpc_IPAddressGroup_0003_p6990194173112"></a><a name="vpc_IPAddressGroup_0003_p6990194173112"></a>必选参数。</p>
    <div class="p" id="vpc_IPAddressGroup_0003_p1990541203113"><a name="vpc_IPAddressGroup_0003_p1990541203113"></a><a name="vpc_IPAddressGroup_0003_p1990541203113"></a>此处设置IP地址组内支持的IP类型，具体如下：<a name="vpc_IPAddressGroup_0003_ul139905412312"></a><a name="vpc_IPAddressGroup_0003_ul139905412312"></a><ul id="vpc_IPAddressGroup_0003_ul139905412312"><li>IPv4</li><li>IPv6</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="vpc_IPAddressGroup_0003_p16990104153115"><a name="vpc_IPAddressGroup_0003_p16990104153115"></a><a name="vpc_IPAddressGroup_0003_p16990104153115"></a>IPv4</p>
    </td>
    </tr>
    <tr id="vpc_IPAddressGroup_0003_row299017413314"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="vpc_IPAddressGroup_0003_p129901741193112"><a name="vpc_IPAddressGroup_0003_p129901741193112"></a><a name="vpc_IPAddressGroup_0003_p129901741193112"></a>IP地址条目</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.35999999999999%" headers="mcps1.2.4.1.2 "><p id="vpc_IPAddressGroup_0003_p14393745111819"><a name="vpc_IPAddressGroup_0003_p14393745111819"></a><a name="vpc_IPAddressGroup_0003_p14393745111819"></a>可选参数。</p>
    <p id="vpc_IPAddressGroup_0003_p1625192361815"><a name="vpc_IPAddressGroup_0003_p1625192361815"></a><a name="vpc_IPAddressGroup_0003_p1625192361815"></a>您可以在IP地址组内添加多个不同格式的IP地址，每个IP地址输入完成后，按回车键换行。</p>
    <div class="p" id="vpc_IPAddressGroup_0003_p19990194173120"><a name="vpc_IPAddressGroup_0003_p19990194173120"></a><a name="vpc_IPAddressGroup_0003_p19990194173120"></a>支持的IP格式如下：<a name="vpc_IPAddressGroup_0003_ul7990741163115"></a><a name="vpc_IPAddressGroup_0003_ul7990741163115"></a><ul id="vpc_IPAddressGroup_0003_ul7990741163115"><li>IPv4网段：IP地址/掩码，例如192.168.0.0/16</li><li>单个IPv4地址：IP地址/掩码，例如192.168.10.10/32</li><li>IPv6网段：IP地址/掩码，例如2001:db8:a583:6e::/64</li><li>单个IPv6地址：IP地址/掩码，例如2001:db8:a583:6e::5c/128</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="33.83%" headers="mcps1.2.4.1.3 "><p id="vpc_IPAddressGroup_0003_p124895322015"><a name="vpc_IPAddressGroup_0003_p124895322015"></a><a name="vpc_IPAddressGroup_0003_p124895322015"></a>192.168.0.0/16</p>
    <p id="vpc_IPAddressGroup_0003_p263955012207"><a name="vpc_IPAddressGroup_0003_p263955012207"></a><a name="vpc_IPAddressGroup_0003_p263955012207"></a>192.168.10.10/32</p>
    </td>
    </tr>
    </tbody>
    </table>

7.  基本信息设置完成后，单击“确定”。

    返回IP地址条目列表，可以看到新添加的IP地址。


