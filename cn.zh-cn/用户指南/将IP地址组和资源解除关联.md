# 将IP地址组和资源解除关联<a name="vpc_IPAddressGroup_0006"></a>

## 操作场景<a name="section66699152161428"></a>

如果您的IP地址已经不需要使用，本章节指导用户解除IP地址组和资源的关联关系。

IP地址组可关联至安全组，网络ACL中。

## 约束与限制<a name="section71241632161817"></a>

解除关联IP地址组后，资源相关的网络规则将会失效，并且无法恢复，请您谨慎操作。

## 操作步骤<a name="section16419124611591"></a>

1.  登录管理控制台。


1.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
2.  在系统首页，选择“网络\>虚拟私有云”。

    进入虚拟私有云列表页面。

3.  在左侧导航栏，选择“IP地址组”。

    进入IP地址组列表页面。

4.  在IP地址组列表中，在目标IP地址组所在行的“关联资源”列下，单击资源超链接。

    进入“关联资源”详情页。

5.  在关联资源列表中，单击对应的资源名称超链接。

    进入资源的详情页，解除IP地址组和资源的关联关系操作指导如[表1](#table106971359413)所示。

    **表 1**  IP地址组解除关联资源指导

    <a name="table106971359413"></a>
    <table><thead align="left"><tr id="row12697951849"><th class="cellrowborder" valign="top" width="18.581858185818582%" id="mcps1.2.4.1.1"><p id="p16697175140"><a name="p16697175140"></a><a name="p16697175140"></a>资源</p>
    </th>
    <th class="cellrowborder" valign="top" width="37.603760376037606%" id="mcps1.2.4.1.2"><p id="p8697251842"><a name="p8697251842"></a><a name="p8697251842"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="43.81438143814381%" id="mcps1.2.4.1.3"><p id="p11697135847"><a name="p11697135847"></a><a name="p11697135847"></a>操作指导</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row36971959414"><td class="cellrowborder" valign="top" width="18.581858185818582%" headers="mcps1.2.4.1.1 "><p id="p114331040541"><a name="p114331040541"></a><a name="p114331040541"></a>安全组</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.603760376037606%" headers="mcps1.2.4.1.2 "><p id="p16971551447"><a name="p16971551447"></a><a name="p16971551447"></a>在安全组入方向或者出方向规则中，修改或者删除IP地址组对应的规则。</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.81438143814381%" headers="mcps1.2.4.1.3 "><a name="ul13731443111418"></a><a name="ul13731443111418"></a><ul id="ul13731443111418"><li><a href="修改安全组规则.md">修改安全组规则</a>：<a name="ul1778144914236"></a><a name="ul1778144914236"></a><ul id="ul1778144914236"><li>入方向规则：修改“源地址”。</li><li>出方向规则：修改“目的地址”。</li></ul>
    </li><li><a href="删除安全组规则.md">删除安全组规则</a></li></ul>
    </td>
    </tr>
    <tr id="row66973512419"><td class="cellrowborder" valign="top" width="18.581858185818582%" headers="mcps1.2.4.1.1 "><p id="p18697958416"><a name="p18697958416"></a><a name="p18697958416"></a><span id="text1514165819811"><a name="text1514165819811"></a><a name="text1514165819811"></a></span><span id="text51413581184"><a name="text51413581184"></a><a name="text51413581184"></a>网络ACL</span></p>
    </td>
    <td class="cellrowborder" valign="top" width="37.603760376037606%" headers="mcps1.2.4.1.2 "><p id="p1769715545"><a name="p1769715545"></a><a name="p1769715545"></a>在<span id="text11116011091"><a name="text11116011091"></a><a name="text11116011091"></a></span><span id="text11164115913"><a name="text11164115913"></a><a name="text11164115913"></a>网络ACL</span>入方向或者出方向规则中，修改或者删除IP地址组对应的规则。</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.81438143814381%" headers="mcps1.2.4.1.3 "><a name="ul194756361256"></a><a name="ul194756361256"></a><ul id="ul194756361256"><li><a href="修改网络ACL规则.md">修改网络ACL规则</a>：<a name="ul1322055661616"></a><a name="ul1322055661616"></a><ul id="ul1322055661616"><li>入方向规则：修改“源地址”或者“目的地址”。</li><li>出方向规则：修改“源地址”或者“目的地址”。</li></ul>
    </li><li><a href="删除网络ACL规则.md">删除网络ACL规则</a></li></ul>
    </td>
    </tr>
    </tbody>
    </table>


