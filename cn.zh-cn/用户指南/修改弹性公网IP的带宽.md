# 修改弹性公网IP的带宽<a name="zh-cn_topic_0013748743"></a>

## 操作场景<a name="section10773344113312"></a>

当您购买弹性公网IP时，无论是哪种计费模式，只要没有加入共享带宽，那么您的弹性公网IP使用的是独享带宽。

本章节指导用户修改独享带宽大小，你可以增加或者降低带宽大小。

当您修改带宽大小时，不同计费方式的带宽收费和生效时间不同，请您参考[表1](#zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0013748743_table117061129519)了解详情，适用于独享带宽和共享带宽两种情况。

**表 1**  修改带宽大小的费用情况

<a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0013748743_table117061129519"></a>
<table><thead align="left"><tr id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_row2070710212517"><th class="cellrowborder" valign="top" width="14.12141214121412%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p192751613174111"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p192751613174111"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p192751613174111"></a>计费模式</p>
</th>
<th class="cellrowborder" valign="top" width="12.461246124612462%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p72751213104111"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p72751213104111"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p72751213104111"></a>计费方式</p>
</th>
<th class="cellrowborder" valign="top" width="18.771877187718772%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p13707142550"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p13707142550"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p13707142550"></a>变更操作</p>
</th>
<th class="cellrowborder" valign="top" width="54.64546454645465%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p1170715212514"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p1170715212514"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p1170715212514"></a>对费用的影响</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_row599095714407"><td class="cellrowborder" rowspan="3" valign="top" width="14.12141214121412%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p42751813174114"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p42751813174114"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p42751813174114"></a>包年/包月</p>
</td>
<td class="cellrowborder" valign="top" width="12.461246124612462%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1227591314412"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1227591314412"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1227591314412"></a>按带宽计费</p>
</td>
<td class="cellrowborder" valign="top" width="18.771877187718772%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p37072027518"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p37072027518"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p37072027518"></a>增加带宽大小（补差价升配）</p>
</td>
<td class="cellrowborder" valign="top" width="54.64546454645465%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p137921136204510"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p137921136204510"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p137921136204510"></a>升配后，新带宽大小将在原来已有的时间周期内立即生效。</p>
<p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p767918917713"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p767918917713"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p767918917713"></a>您需要按照与原带宽的价格差，结合使用周期内的剩余时间，补齐差价。</p>
<p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p86671154121414"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p86671154121414"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p86671154121414"></a>例如：（以下价格仅作示例，实际价格以控制台显示为准）</p>
<p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p12682927111510"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p12682927111510"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p12682927111510"></a>客户于2018/11/1 购买了1Mbit/s的带宽，购买时长为1个月，此时价格为18.4元/月，客户使用余额支付18.4元，实付金额为18.4元。</p>
<p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p4682827141512"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p4682827141512"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p4682827141512"></a>客户在2018/11/24 将带宽升级为5Mbit/s，价格为92元/月。</p>
<p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p2682327141516"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p2682327141516"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p2682327141516"></a>这时，剩余天数为 30 - 24 = 6天，升配费用=92 / 30 * 6 - 18.4 / 30 * 6 = 14.72元。</p>
<p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p9529133320254"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p9529133320254"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p9529133320254"></a>了解更多变更资源计费信息，请参见<a href="https://support.huaweicloud.com/usermanual-billing/renewals_topic_60000001.html" target="_blank" rel="noopener noreferrer">变更资源费用说明</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_row1797215914408"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1782175895717"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1782175895717"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1782175895717"></a>按带宽计费</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p661712881111"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p661712881111"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p661712881111"></a>降低带宽大小（续费降配）</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p3299102165312"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p3299102165312"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p3299102165312"></a>降配后，新带宽大小不会立即生效。</p>
<div class="p" id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p186171228151117"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p186171228151117"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_p186171228151117"></a>你需要选择续费时长并根据新的带宽大小进行续费，续费成功后，新带宽大小在新的计费周期内生效。<a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_ul178551434171416"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_ul178551434171416"></a><ul id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_ul178551434171416"><li>续费降配订单在资源未生效前支持退订。</li><li>续费降配后，当前计费周期的剩余时间内不能再对带宽进行任何修改，请谨慎操作。</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_row173115585423"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p4831958195714"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p4831958195714"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p4831958195714"></a>按带宽计费</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p2311145811424"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p2311145811424"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p2311145811424"></a>临时增加带宽大小（使用带宽加油包临时升配）</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p47671371431"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p47671371431"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p47671371431"></a>带宽加油包单独计费，您可以在带宽的使用周期内选择任意时间段使用带宽加油包临时增加带宽，带宽加油包到期后带宽自动回落。</p>
</td>
</tr>
<tr id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_row129737166211"><td class="cellrowborder" rowspan="2" valign="top" width="14.12141214121412%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p29731716727"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p29731716727"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p29731716727"></a>按需计费</p>
</td>
<td class="cellrowborder" valign="top" width="12.461246124612462%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p155655310417"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p155655310417"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p155655310417"></a>按带宽计费</p>
</td>
<td class="cellrowborder" valign="top" width="18.771877187718772%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p103945561024"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p103945561024"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p103945561024"></a>增加/降低带宽大小</p>
</td>
<td class="cellrowborder" valign="top" width="54.64546454645465%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p99732163210"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p99732163210"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_p99732163210"></a>增加/降低带宽大小后，新的带宽大小和计费方式将立即生效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_zh-cn_topic_0213996262_zh-cn_topic_0013748743_row6707727518"><td class="cellrowborder" valign="top" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1956503134119"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1956503134119"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1956503134119"></a>按流量计费</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p58721747174214"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p58721747174214"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p58721747174214"></a>增加/降低带宽大小</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1965713187107"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1965713187107"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p1965713187107"></a>增加/降低带宽大小后，新的带宽大小将立即生效。</p>
<p id="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p82981749691"><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p82981749691"></a><a name="zh-cn_topic_0213996262_zh-cn_topic_0000001240837046_p82981749691"></a>按流量计费的EIP，带宽仅做限速使用，带宽大小不影响实际费用。</p>
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

    **图 1**  修改按需带宽<a name="fig10519348133519"></a>  
    ![](figures/修改按需带宽.png "修改按需带宽")

    **图 2**  修改包年包月带宽<a name="fig18374419368"></a>  
    ![](figures/修改包年包月带宽.png "修改包年包月带宽")

6.  单击“下一步”。
7.  单击“提交”，完成修改。

## 相关操作<a name="section11286143172713"></a>

-   [如何切换计费方式中的“按带宽计费”和“按流量计费”？](https://support.huaweicloud.com/vpc_faq/vpc_common_0001.html)
-   [什么是入云带宽和出云带宽？](https://support.huaweicloud.com/vpc_faq/faq_bandwidth_0004.html)
-   [包年包月模式的带宽支持升配后再降配吗？](https://support.huaweicloud.com/vpc_faq/faq_bandwidth_0005.html)
-   [带宽如何扩大至300Mbit/s以上？](https://support.huaweicloud.com/eip_faq/faq_bandwidth_0015.html)

