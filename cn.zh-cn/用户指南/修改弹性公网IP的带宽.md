# 修改弹性公网IP的带宽<a name="zh-cn_topic_0013748743"></a>

## 操作场景<a name="section10773344113312"></a>

对于按需计费的弹性公网IP，支持修改带宽名称、大小、计费方式（按带宽计费、按流量计费）。

对于包年包月的弹性公网IP，支持修改带宽名称和大小。

## 费用影响<a name="section8326112318419"></a>

**表 1**  费用影响

<a name="table117061129519"></a>
<table><thead align="left"><tr id="row2070710212517"><th class="cellrowborder" valign="top" width="14.04%" id="mcps1.2.4.1.1"><p id="p22514331491"><a name="p22514331491"></a><a name="p22514331491"></a>当前计费模式</p>
</th>
<th class="cellrowborder" valign="top" width="18.91%" id="mcps1.2.4.1.2"><p id="p13707142550"><a name="p13707142550"></a><a name="p13707142550"></a>变更场景</p>
</th>
<th class="cellrowborder" valign="top" width="67.05%" id="mcps1.2.4.1.3"><p id="p1170715212514"><a name="p1170715212514"></a><a name="p1170715212514"></a>对费用的影响</p>
</th>
</tr>
</thead>
<tbody><tr id="row137079211510"><td class="cellrowborder" valign="top" width="14.04%" headers="mcps1.2.4.1.1 "><p id="p3251333391"><a name="p3251333391"></a><a name="p3251333391"></a>按需</p>
</td>
<td class="cellrowborder" valign="top" width="18.91%" headers="mcps1.2.4.1.2 "><p id="p117077212514"><a name="p117077212514"></a><a name="p117077212514"></a>变更计费方式为按带宽计费、按流量计费</p>
</td>
<td class="cellrowborder" valign="top" width="67.05%" headers="mcps1.2.4.1.3 "><p id="p12679391175"><a name="p12679391175"></a><a name="p12679391175"></a>变更成功后，新的计费方式将立即生效。</p>
</td>
</tr>
<tr id="row6707727518"><td class="cellrowborder" rowspan="2" valign="top" width="14.04%" headers="mcps1.2.4.1.1 "><p id="p2251833692"><a name="p2251833692"></a><a name="p2251833692"></a>包年包月</p>
</td>
<td class="cellrowborder" valign="top" width="18.91%" headers="mcps1.2.4.1.2 "><p id="p37072027518"><a name="p37072027518"></a><a name="p37072027518"></a>增加带宽大小（升配）</p>
</td>
<td class="cellrowborder" valign="top" width="67.05%" headers="mcps1.2.4.1.3 "><p id="p767918917713"><a name="p767918917713"></a><a name="p767918917713"></a>升配后新带宽大小将在原来已有的时间周期内立即生效。需按照与原规格的价格差异，结合已使用的时间周期，补上差价。</p>
</td>
</tr>
<tr id="row1616328121117"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p661712881111"><a name="p661712881111"></a><a name="p661712881111"></a>降低带宽大小（续费降配）</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p186171228151117"><a name="p186171228151117"></a><a name="p186171228151117"></a>续费成功后新的带宽大小将在新的计费周期生效。</p>
<a name="ul178551434171416"></a><a name="ul178551434171416"></a><ul id="ul178551434171416"><li>续费降配订单支付成功后不可取消。</li><li>续费降配后，当前计费周期的剩余时间内不能再对带宽进行任何修改，请谨慎操作。</li></ul>
</td>
</tr>
<tr id="row1211891016159"><td class="cellrowborder" valign="top" width="14.04%" headers="mcps1.2.4.1.1 "><p id="p1911811016158"><a name="p1911811016158"></a><a name="p1911811016158"></a>按需</p>
</td>
<td class="cellrowborder" valign="top" width="18.91%" headers="mcps1.2.4.1.2 "><p id="p211817109156"><a name="p211817109156"></a><a name="p211817109156"></a>转包年包月</p>
</td>
<td class="cellrowborder" valign="top" width="67.05%" headers="mcps1.2.4.1.3 "><p id="p6118101031516"><a name="p6118101031516"></a><a name="p6118101031516"></a>您可以在弹性公网IP页面或费用中心转包年包月，变更成功后，新的计费模式将立即生效。具体操作请参见<a href="https://support.huaweicloud.com/vpc_faq/vpc_faq_0078.html" target="_blank" rel="noopener noreferrer">如何切换计费模式中的“按需”和“包年包月”？</a>。</p>
</td>
</tr>
<tr id="row128237518151"><td class="cellrowborder" valign="top" width="14.04%" headers="mcps1.2.4.1.1 "><p id="p682385181517"><a name="p682385181517"></a><a name="p682385181517"></a>包年包月</p>
</td>
<td class="cellrowborder" valign="top" width="18.91%" headers="mcps1.2.4.1.2 "><p id="p28231251191519"><a name="p28231251191519"></a><a name="p28231251191519"></a>转按需</p>
</td>
<td class="cellrowborder" valign="top" width="67.05%" headers="mcps1.2.4.1.3 "><p id="p282325141517"><a name="p282325141517"></a><a name="p282325141517"></a>您可以在费用中心转按需，包年包月资费到期后，新的按需资费才会生效。具体操作请参见<a href="https://support.huaweicloud.com/vpc_faq/vpc_faq_0078.html" target="_blank" rel="noopener noreferrer">如何切换计费模式中的“按需”和“包年包月”？</a>。</p>
</td>
</tr>
</tbody>
</table>

## 操作步骤<a name="section1051492110121"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，选择“网络 \> 弹性公网IP”。
4.  在“操作”列，选择“更多 \> 修改带宽”。
5.  根据界面提示修改带宽参数。

    **图 1**  修改按需带宽<a name="fig153971231554"></a>  
    ![](figures/修改按需带宽.png "修改按需带宽")

    **图 2**  修改包年包月带宽<a name="fig11110715155013"></a>  
    ![](figures/修改包年包月带宽.png "修改包年包月带宽")

6.  单击“下一步”。
7.  单击“提交”，完成修改。

## 相关操作<a name="section11286143172713"></a>

-   [如何切换计费方式中的“按带宽计费”和“按流量计费”？](https://support.huaweicloud.com/vpc_faq/vpc_common_0001.html)
-   [什么是入云带宽和出云带宽？](https://support.huaweicloud.com/vpc_faq/faq_bandwidth_0004.html)
-   [包年包月模式的带宽支持升配后再降配吗？](https://support.huaweicloud.com/vpc_faq/faq_bandwidth_0005.html)

