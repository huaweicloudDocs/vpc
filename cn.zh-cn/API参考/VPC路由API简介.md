# VPC路由API简介<a name="ZH-CN_TOPIC_0075677491"></a>

## 对象简介<a name="section14498172511118"></a>

对VPC路由进行管理和操作，包括查询路由列表、创建路由、查询路由、删除路由。

## 对象模型<a name="section1749920252117"></a>

**表 1**  route对象

<a name="table05001250111"></a>
<table><thead align="left"><tr id="row1604152531116"><th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.2.7.1.1"><p id="p19605525151115"><a name="p19605525151115"></a><a name="p19605525151115"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="14.141414141414144%" id="mcps1.2.7.1.2"><p id="p2060572511111"><a name="p2060572511111"></a><a name="p2060572511111"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.101010101010102%" id="mcps1.2.7.1.3"><p id="p76051025151113"><a name="p76051025151113"></a><a name="p76051025151113"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="14.141414141414144%" id="mcps1.2.7.1.4"><p id="p960582511116"><a name="p960582511116"></a><a name="p960582511116"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="14.141414141414144%" id="mcps1.2.7.1.5"><p id="p0605192520110"><a name="p0605192520110"></a><a name="p0605192520110"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="31.313131313131315%" id="mcps1.2.7.1.6"><p id="p11605425111120"><a name="p11605425111120"></a><a name="p11605425111120"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19605172516117"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.7.1.1 "><p id="p4605625141117"><a name="p4605625141117"></a><a name="p4605625141117"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.2 "><p id="p4605425191116"><a name="p4605425191116"></a><a name="p4605425191116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p2060572521118"><a name="p2060572521118"></a><a name="p2060572521118"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.4 "><p id="p126051425111112"><a name="p126051425111112"></a><a name="p126051425111112"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.5 "><p id="p7605192513113"><a name="p7605192513113"></a><a name="p7605192513113"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.7.1.6 "><p id="p136051025171110"><a name="p136051025171110"></a><a name="p136051025171110"></a>路由id</p>
</td>
</tr>
<tr id="row19605192511115"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.7.1.1 "><p id="p1160582510117"><a name="p1160582510117"></a><a name="p1160582510117"></a>destination</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.2 "><p id="p186051725131113"><a name="p186051725131113"></a><a name="p186051725131113"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p186051025141117"><a name="p186051025141117"></a><a name="p186051025141117"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.4 "><p id="p186052025151117"><a name="p186052025151117"></a><a name="p186052025151117"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.5 "><p id="p1160562511112"><a name="p1160562511112"></a><a name="p1160562511112"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.7.1.6 "><p id="p20605425121118"><a name="p20605425121118"></a><a name="p20605425121118"></a>路由目的地址CIDR</p>
</td>
</tr>
<tr id="row160513252111"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.7.1.1 "><p id="p76051225121114"><a name="p76051225121114"></a><a name="p76051225121114"></a>nexthop</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.2 "><p id="p1460592591111"><a name="p1460592591111"></a><a name="p1460592591111"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p26065251115"><a name="p26065251115"></a><a name="p26065251115"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.4 "><p id="p1560672513117"><a name="p1560672513117"></a><a name="p1560672513117"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.5 "><p id="p18606125171118"><a name="p18606125171118"></a><a name="p18606125171118"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.7.1.6 "><p id="p1360692551117"><a name="p1360692551117"></a><a name="p1360692551117"></a>路由下一跳，如果路由是“peering”类型，填写vpc peering id。</p>
</td>
</tr>
<tr id="row26061325191110"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.7.1.1 "><p id="p86067257112"><a name="p86067257112"></a><a name="p86067257112"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.2 "><p id="p260619251118"><a name="p260619251118"></a><a name="p260619251118"></a>String(16)</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p1360618256118"><a name="p1360618256118"></a><a name="p1360618256118"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.4 "><p id="p76061254111"><a name="p76061254111"></a><a name="p76061254111"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.5 "><p id="p1560617254112"><a name="p1560617254112"></a><a name="p1560617254112"></a>目前仅支持“peering”</p>
</td>
<td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.7.1.6 "><p id="p9606112520117"><a name="p9606112520117"></a><a name="p9606112520117"></a>路由类型。</p>
</td>
</tr>
<tr id="row11606125111110"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.7.1.1 "><p id="p12606162501119"><a name="p12606162501119"></a><a name="p12606162501119"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.2 "><p id="p06061925181119"><a name="p06061925181119"></a><a name="p06061925181119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p12606122541120"><a name="p12606122541120"></a><a name="p12606122541120"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.4 "><p id="p16606152521120"><a name="p16606152521120"></a><a name="p16606152521120"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.5 "><p id="p15606102521110"><a name="p15606102521110"></a><a name="p15606102521110"></a>存在的vpc id</p>
</td>
<td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.7.1.6 "><p id="p9606112519111"><a name="p9606112519111"></a><a name="p9606112519111"></a>请求添加路由的vpc</p>
</td>
</tr>
<tr id="row56067256117"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.7.1.1 "><p id="p196065257115"><a name="p196065257115"></a><a name="p196065257115"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.2 "><p id="p10606182591115"><a name="p10606182591115"></a><a name="p10606182591115"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="10.101010101010102%" headers="mcps1.2.7.1.3 "><p id="p9606172511117"><a name="p9606172511117"></a><a name="p9606172511117"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.4 "><p id="p16074259111"><a name="p16074259111"></a><a name="p16074259111"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.141414141414144%" headers="mcps1.2.7.1.5 "><p id="p12607172517116"><a name="p12607172517116"></a><a name="p12607172517116"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="31.313131313131315%" headers="mcps1.2.7.1.6 "><p id="p4607825141118"><a name="p4607825141118"></a><a name="p4607825141118"></a>项目ID。</p>
</td>
</tr>
</tbody>
</table>

