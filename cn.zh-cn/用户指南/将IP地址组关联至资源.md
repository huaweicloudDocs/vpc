# 将IP地址组关联至资源<a name="vpc_IPAddressGroup_0004"></a>

## 操作场景<a name="section66699152161428"></a>

IP地址创建完成后无法独立使用，本章节指导用户将IP地址组关联至对应的资源投入使用。

IP地址组可关联至安全组，网络ACL中。

## 前提条件<a name="section524672122318"></a>

-   已创建完成IP地址组，具体请参见[创建IP地址组](创建IP地址组.md)。
-   已在IP地址组内添加IP地址条目，具体请参见[在IP地址组内添加IP地址条目](在IP地址组内添加IP地址条目.md)。

## 操作步骤<a name="section16419124611591"></a>

您需要将以创建的IP地址组关联至对应的资源投入使用，操作指导如[表1](#table106971359413)所示。

**表 1**  IP地址组关联资源指导

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
<td class="cellrowborder" valign="top" width="37.603760376037606%" headers="mcps1.2.4.1.2 "><p id="p16971551447"><a name="p16971551447"></a><a name="p16971551447"></a>添加安全组规则的时候，源地址和目的地址可以选择IP地址组。</p>
</td>
<td class="cellrowborder" valign="top" width="43.81438143814381%" headers="mcps1.2.4.1.3 "><p id="p11369105717483"><a name="p11369105717483"></a><a name="p11369105717483"></a><a href="添加安全组规则.md">添加安全组规则</a>：</p>
<a name="ul13731443111418"></a><a name="ul13731443111418"></a><ul id="ul13731443111418"><li>添加入方向规则：“源地址”选择IP地址组。</li><li>添加出方向规则：“目的地址”选择IP地址组。</li></ul>
</td>
</tr>
<tr id="row66973512419"><td class="cellrowborder" valign="top" width="18.581858185818582%" headers="mcps1.2.4.1.1 "><p id="p53281935586"><a name="p53281935586"></a><a name="p53281935586"></a><span id="text959465018482"><a name="text959465018482"></a><a name="text959465018482"></a></span><span id="text1995365711486"><a name="text1995365711486"></a><a name="text1995365711486"></a>网络ACL</span></p>
</td>
<td class="cellrowborder" valign="top" width="37.603760376037606%" headers="mcps1.2.4.1.2 "><p id="p1769715545"><a name="p1769715545"></a><a name="p1769715545"></a>添加<span id="text1643717382088"><a name="text1643717382088"></a><a name="text1643717382088"></a></span><span id="text343714386819"><a name="text343714386819"></a><a name="text343714386819"></a>网络ACL</span>规则的时候，源地址和目的地址可以选择IP地址组。</p>
</td>
<td class="cellrowborder" valign="top" width="43.81438143814381%" headers="mcps1.2.4.1.3 "><div class="p" id="p948410412815"><a name="p948410412815"></a><a name="p948410412815"></a><a href="添加网络ACL规则.md">添加网络ACL规则</a>：<a name="ul1322055661616"></a><a name="ul1322055661616"></a><ul id="ul1322055661616"><li>添加入方向规则：“源地址”或者“目的地址”选择IP地址组，源地址和目的地址只能有一方使用IP地址组。</li><li>添加出方向规则：“源地址”或者“目的地址”选择IP地址组，源地址和目的地址只能有一方使用IP地址组。</li></ul>
</div>
</td>
</tr>
</tbody>
</table>

