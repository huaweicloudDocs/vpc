# 创建IP地址组<a name="vpc_IPAddressGroup_0003"></a>

## 操作场景<a name="section11931748102518"></a>

本章节指导用户创建IP地址组，IP地址组是一个或者多个IP地址的集合，可关联至安全组、网络ACL中，用于简化网络架构中IP地址的配置和管理。

## 操作指导<a name="section526211212611"></a>

1.  进入[创建IP地址组页面](https://console.huaweicloud.com/vpc/?locale=zh-cn#/vpc/ipGroups/create)。
2.  根据界面提示设置IP地址组参数。

    参数详细说明请参见[表1](#table15989174133114)。

    **表 1**  IP地址组参数说明

    <a name="table15989174133114"></a>
    <table><thead align="left"><tr id="row99907413319"><th class="cellrowborder" valign="top" width="14.81%" id="mcps1.2.4.1.1"><p id="p49901541173110"><a name="p49901541173110"></a><a name="p49901541173110"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.300000000000004%" id="mcps1.2.4.1.2"><p id="p14990441173111"><a name="p14990441173111"></a><a name="p14990441173111"></a>参数说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.89%" id="mcps1.2.4.1.3"><p id="p1999094111313"><a name="p1999094111313"></a><a name="p1999094111313"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row201694013611"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p19161840564"><a name="p19161840564"></a><a name="p19161840564"></a>区域</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.4.1.2 "><p id="p1512561372720"><a name="p1512561372720"></a><a name="p1512561372720"></a>必选参数。</p>
    <p id="p1420422134014"><a name="p1420422134014"></a><a name="p1420422134014"></a>不同区域的云服务产品之间内网互不相通，请就近选择靠近您业务的区域，可减少网络时延，提高访问速度。</p>
    <p id="p1272912451291"><a name="p1272912451291"></a><a name="p1272912451291"></a>IP地址组只能关联至同区域的资源。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.89%" headers="mcps1.2.4.1.3 "><p id="p3175401360"><a name="p3175401360"></a><a name="p3175401360"></a>区域A</p>
    </td>
    </tr>
    <tr id="row99901241203114"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p99909414312"><a name="p99909414312"></a><a name="p99909414312"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.4.1.2 "><p id="p199024114311"><a name="p199024114311"></a><a name="p199024114311"></a>必选参数。</p>
    <p id="p57241222173317"><a name="p57241222173317"></a><a name="p57241222173317"></a>此处填写IP地址组的名称。</p>
    <a name="ul13354429153415"></a><a name="ul13354429153415"></a><ul id="ul13354429153415"><li>长度范围为1~64位。</li><li>名称由中文、英文字母、数字、下划线（_）、中划线（-）、点（.）组成。</li></ul>
    <p id="p099010413318"><a name="p099010413318"></a><a name="p099010413318"></a>您可以自定义IP地址组名称，IP地址组的唯一性由系统分配的ID号保证。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.89%" headers="mcps1.2.4.1.3 "><p id="p18990194112316"><a name="p18990194112316"></a><a name="p18990194112316"></a>ipGroup-A</p>
    </td>
    </tr>
    <tr id="row1526131061218"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p52718101124"><a name="p52718101124"></a><a name="p52718101124"></a>最大条目数</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.4.1.2 "><p id="p52715103121"><a name="p52715103121"></a><a name="p52715103121"></a>必选参数。</p>
    <p id="p7772834171217"><a name="p7772834171217"></a><a name="p7772834171217"></a>此处设置IP地址组内支持添加的IP地址条目数量，系统默认显示当前支持的最大条目数，您可以自行减少最大条目数。</p>
    <p id="p52902049191416"><a name="p52902049191416"></a><a name="p52902049191416"></a>如果需要提升IP地址组的最大条目数，您需要<a href="https://console.huaweicloud.com/ticket/#/ticketindex/createIndex" target="_blank" rel="noopener noreferrer">提交工单</a>进行申请。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.89%" headers="mcps1.2.4.1.3 "><p id="p172771017125"><a name="p172771017125"></a><a name="p172771017125"></a>20</p>
    </td>
    </tr>
    <tr id="row79904416315"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p199909417319"><a name="p199909417319"></a><a name="p199909417319"></a>IP类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.4.1.2 "><p id="p6990194173112"><a name="p6990194173112"></a><a name="p6990194173112"></a>必选参数。</p>
    <div class="p" id="p1990541203113"><a name="p1990541203113"></a><a name="p1990541203113"></a>此处设置IP地址组内支持的IP类型，具体如下：<a name="ul139905412312"></a><a name="ul139905412312"></a><ul id="ul139905412312"><li>IPv4</li><li>IPv6</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="33.89%" headers="mcps1.2.4.1.3 "><p id="p16990104153115"><a name="p16990104153115"></a><a name="p16990104153115"></a>IPv4</p>
    </td>
    </tr>
    <tr id="row299017413314"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p129901741193112"><a name="p129901741193112"></a><a name="p129901741193112"></a>IP地址条目</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.4.1.2 "><p id="p14393745111819"><a name="p14393745111819"></a><a name="p14393745111819"></a>可选参数。</p>
    <p id="p1625192361815"><a name="p1625192361815"></a><a name="p1625192361815"></a>您可以在IP地址组内添加多个不同格式的IP地址，每个IP地址输入完成后，按回车键换行。</p>
    <div class="p" id="p19990194173120"><a name="p19990194173120"></a><a name="p19990194173120"></a>支持的IP格式如下：<a name="ul7990741163115"></a><a name="ul7990741163115"></a><ul id="ul7990741163115"><li>IPv4网段：IP地址/掩码，例如192.168.0.0/16</li><li>单个IPv4地址：IP地址/掩码，例如192.168.10.10/32</li><li>IPv6网段：IP地址/掩码，例如2001:db8:a583:6e::/64</li><li>单个IPv6地址：IP地址/掩码，例如2001:db8:a583:6e::5c/128</li></ul>
    </div>
    </td>
    <td class="cellrowborder" valign="top" width="33.89%" headers="mcps1.2.4.1.3 "><p id="p124895322015"><a name="p124895322015"></a><a name="p124895322015"></a>192.168.0.0/16</p>
    <p id="p263955012207"><a name="p263955012207"></a><a name="p263955012207"></a>192.168.10.10/32</p>
    </td>
    </tr>
    <tr id="row17472114818610"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p12846948155518"><a name="p12846948155518"></a><a name="p12846948155518"></a>企业项目</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.4.1.2 "><p id="p12659201519713"><a name="p12659201519713"></a><a name="p12659201519713"></a>必选参数。</p>
    <p id="p260812488536"><a name="p260812488536"></a><a name="p260812488536"></a>创建IP地址组时，可以将IP地址组加入已启用的企业项目。</p>
    <p id="p5242161295416"><a name="p5242161295416"></a><a name="p5242161295416"></a>企业项目管理提供了一种按企业项目管理云资源的方式，帮助您实现以企业项目为基本单元的资源及人员的统一管理，默认项目为default。</p>
    <p id="p0846164816550"><a name="p0846164816550"></a><a name="p0846164816550"></a>关于创建和管理企业项目的详情，请参见《企业管理用户指南》。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.89%" headers="mcps1.2.4.1.3 "><p id="p17846194813558"><a name="p17846194813558"></a><a name="p17846194813558"></a>default</p>
    </td>
    </tr>
    <tr id="row20991441183110"><td class="cellrowborder" valign="top" width="14.81%" headers="mcps1.2.4.1.1 "><p id="p109911141133115"><a name="p109911141133115"></a><a name="p109911141133115"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.300000000000004%" headers="mcps1.2.4.1.2 "><p id="p81670915218"><a name="p81670915218"></a><a name="p81670915218"></a>可选参数。</p>
    <p id="p7991241203111"><a name="p7991241203111"></a><a name="p7991241203111"></a>您可以根据需要在文本框中输入IP地址组的描述信息。</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.89%" headers="mcps1.2.4.1.3 "><p id="p13991124143119"><a name="p13991124143119"></a><a name="p13991124143119"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  基本信息设置完成后，单击“立即创建”。

    返回IP地址组列表，创建成功的IP地址组状态为“正常”。

    >![](public_sys-resources/icon-notice.gif) **须知：** 
    >IP地址组无法独立使用，需要将IP地址组关联至对应的资源，具体请参见[将IP地址组关联至资源](将IP地址组关联至资源.md)。

