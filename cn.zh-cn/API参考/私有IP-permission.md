# 私有IP<a name="vpc_permission_0007"></a>

<a name="table967413133817"></a>
<table><thead align="left"><tr id="row9708231163820"><th class="cellrowborder" valign="top" width="11.48114811481148%" id="mcps1.1.6.1.1"><p id="p12888132144112"><a name="p12888132144112"></a><a name="p12888132144112"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="27.57275727572757%" id="mcps1.1.6.1.2"><p id="p158881932134115"><a name="p158881932134115"></a><a name="p158881932134115"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="23.32233223322332%" id="mcps1.1.6.1.3"><p id="p1936201424312"><a name="p1936201424312"></a><a name="p1936201424312"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="19.65196519651965%" id="mcps1.1.6.1.4"><p id="p1840915704317"><a name="p1840915704317"></a><a name="p1840915704317"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="17.97179717971797%" id="mcps1.1.6.1.5"><p id="p94098719436"><a name="p94098719436"></a><a name="p94098719436"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row197081331113817"><td class="cellrowborder" valign="top" width="11.48114811481148%" headers="mcps1.1.6.1.1 "><p id="p9638111155912"><a name="p9638111155912"></a><a name="p9638111155912"></a>申请私有IP</p>
</td>
<td class="cellrowborder" valign="top" width="27.57275727572757%" headers="mcps1.1.6.1.2 "><p id="p17091031143815"><a name="p17091031143815"></a><a name="p17091031143815"></a>POST /v1/{project_id}/privateips</p>
</td>
<td class="cellrowborder" valign="top" width="23.32233223322332%" headers="mcps1.1.6.1.3 "><p id="p13892440173820"><a name="p13892440173820"></a><a name="p13892440173820"></a>vpc:privateIps:create</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.97179717971797%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row15709203163811"><td class="cellrowborder" valign="top" width="11.48114811481148%" headers="mcps1.1.6.1.1 "><p id="p363851114598"><a name="p363851114598"></a><a name="p363851114598"></a>查询私有IP</p>
</td>
<td class="cellrowborder" valign="top" width="27.57275727572757%" headers="mcps1.1.6.1.2 "><p id="p7709103117385"><a name="p7709103117385"></a><a name="p7709103117385"></a>GET /v1/{project_id}/privateips/{privateip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="23.32233223322332%" headers="mcps1.1.6.1.3 "><p id="p9226104210387"><a name="p9226104210387"></a><a name="p9226104210387"></a>vpc:privateIps:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.97179717971797%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row1670914317388"><td class="cellrowborder" valign="top" width="11.48114811481148%" headers="mcps1.1.6.1.1 "><p id="p8638811165911"><a name="p8638811165911"></a><a name="p8638811165911"></a>查询私有IP列表</p>
</td>
<td class="cellrowborder" valign="top" width="27.57275727572757%" headers="mcps1.1.6.1.2 "><p id="p17709831173812"><a name="p17709831173812"></a><a name="p17709831173812"></a>GET /v1/{project_id}/subnets/{subnet_id}/privateips</p>
</td>
<td class="cellrowborder" valign="top" width="23.32233223322332%" headers="mcps1.1.6.1.3 "><p id="p1724712431387"><a name="p1724712431387"></a><a name="p1724712431387"></a>vpc:privateIps:list</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.97179717971797%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row6709163118385"><td class="cellrowborder" valign="top" width="11.48114811481148%" headers="mcps1.1.6.1.1 "><p id="p6638181175920"><a name="p6638181175920"></a><a name="p6638181175920"></a>删除私有IP</p>
</td>
<td class="cellrowborder" valign="top" width="27.57275727572757%" headers="mcps1.1.6.1.2 "><p id="p14709143173818"><a name="p14709143173818"></a><a name="p14709143173818"></a>DELETE /v1/{project_id}/privateips/{privateip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="23.32233223322332%" headers="mcps1.1.6.1.3 "><p id="p12681044203812"><a name="p12681044203812"></a><a name="p12681044203812"></a>vpc:privateIps:delete</p>
</td>
<td class="cellrowborder" valign="top" width="19.65196519651965%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.97179717971797%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>×</p>
</td>
</tr>
</tbody>
</table>

