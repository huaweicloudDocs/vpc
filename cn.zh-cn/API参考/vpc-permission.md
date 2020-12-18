# VPC<a name="vpc_permission_0022"></a>

<a name="table1351682493510"></a>
<table><thead align="left"><tr id="row1759512463518"><th class="cellrowborder" valign="top" width="12.5%" id="mcps1.1.6.1.1"><p id="p19512155317473"><a name="p19512155317473"></a><a name="p19512155317473"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="30.159999999999997%" id="mcps1.1.6.1.2"><p id="p3595424163511"><a name="p3595424163511"></a><a name="p3595424163511"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="18.22%" id="mcps1.1.6.1.3"><p id="p19595172413511"><a name="p19595172413511"></a><a name="p19595172413511"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="14.530000000000001%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="24.59%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.1.6.1.1 "><p id="p8512185310471"><a name="p8512185310471"></a><a name="p8512185310471"></a>创建VPC</p>
</td>
<td class="cellrowborder" valign="top" width="30.159999999999997%" headers="mcps1.1.6.1.2 "><p id="p1597124133519"><a name="p1597124133519"></a><a name="p1597124133519"></a>POST /v1/{project_id}/vpcs</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.6.1.3 "><p id="p12647123593510"><a name="p12647123593510"></a><a name="p12647123593510"></a>vpc:vpcs:create</p>
</td>
<td class="cellrowborder" valign="top" width="14.530000000000001%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="24.59%" headers="mcps1.1.6.1.5 "><p id="p193691154133112"><a name="p193691154133112"></a><a name="p193691154133112"></a>√</p>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.1.6.1.1 "><p id="p6512145316476"><a name="p6512145316476"></a><a name="p6512145316476"></a>查询VPC</p>
</td>
<td class="cellrowborder" valign="top" width="30.159999999999997%" headers="mcps1.1.6.1.2 "><p id="p1859752463519"><a name="p1859752463519"></a><a name="p1859752463519"></a>GET /v1/{project_id}/vpcs/{vpc_id}</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.6.1.3 "><p id="p01753719354"><a name="p01753719354"></a><a name="p01753719354"></a>vpc:vpcs:get</p>
</td>
<td class="cellrowborder" valign="top" width="14.530000000000001%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="24.59%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>√</p>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.1.6.1.1 "><p id="p0512125314718"><a name="p0512125314718"></a><a name="p0512125314718"></a>查询VPC列表</p>
</td>
<td class="cellrowborder" valign="top" width="30.159999999999997%" headers="mcps1.1.6.1.2 "><p id="p145971624193510"><a name="p145971624193510"></a><a name="p145971624193510"></a>GET /v1/{project_id}/vpcs</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.6.1.3 "><p id="p6748143803513"><a name="p6748143803513"></a><a name="p6748143803513"></a>vpc:vpcs:list</p>
</td>
<td class="cellrowborder" valign="top" width="14.530000000000001%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="24.59%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>√</p>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.1.6.1.1 "><p id="p19513175384711"><a name="p19513175384711"></a><a name="p19513175384711"></a>更新VPC</p>
</td>
<td class="cellrowborder" valign="top" width="30.159999999999997%" headers="mcps1.1.6.1.2 "><p id="p1559702415358"><a name="p1559702415358"></a><a name="p1559702415358"></a>PUT /v1/{project_id}/vpcs/{vpc_id}</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.6.1.3 "><p id="p1523118428359"><a name="p1523118428359"></a><a name="p1523118428359"></a>vpc:vpcs:update</p>
</td>
<td class="cellrowborder" valign="top" width="14.530000000000001%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="24.59%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>√</p>
</td>
</tr>
<tr id="row85979249353"><td class="cellrowborder" valign="top" width="12.5%" headers="mcps1.1.6.1.1 "><p id="p16513135334712"><a name="p16513135334712"></a><a name="p16513135334712"></a>删除VPC</p>
</td>
<td class="cellrowborder" valign="top" width="30.159999999999997%" headers="mcps1.1.6.1.2 "><p id="p115973243353"><a name="p115973243353"></a><a name="p115973243353"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}</p>
</td>
<td class="cellrowborder" valign="top" width="18.22%" headers="mcps1.1.6.1.3 "><p id="p841064410359"><a name="p841064410359"></a><a name="p841064410359"></a>vpc:vpcs:delete</p>
</td>
<td class="cellrowborder" valign="top" width="14.530000000000001%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="24.59%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>√</p>
</td>
</tr>
</tbody>
</table>

