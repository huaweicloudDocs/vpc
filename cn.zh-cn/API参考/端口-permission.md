# 端口<a name="vpc_permission_0004"></a>

<a name="table165141341536"></a>
<table><thead align="left"><tr id="row1060515405312"><th class="cellrowborder" valign="top" width="11.65%" id="mcps1.1.6.1.1"><p id="p3808155143811"><a name="p3808155143811"></a><a name="p3808155143811"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="31.53%" id="mcps1.1.6.1.2"><p id="p158081855113816"><a name="p158081855113816"></a><a name="p158081855113816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="17.4%" id="mcps1.1.6.1.3"><p id="p580815563812"><a name="p580815563812"></a><a name="p580815563812"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="21.39%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="18.029999999999998%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row1260584195313"><td class="cellrowborder" valign="top" width="11.65%" headers="mcps1.1.6.1.1 "><p id="p15605144135314"><a name="p15605144135314"></a><a name="p15605144135314"></a>查询端口</p>
</td>
<td class="cellrowborder" valign="top" width="31.53%" headers="mcps1.1.6.1.2 "><p id="p176058485311"><a name="p176058485311"></a><a name="p176058485311"></a>GET /v1/{project_id}/ports</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.1.6.1.3 "><p id="p206058414532"><a name="p206058414532"></a><a name="p206058414532"></a>vpc:ports:get</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.029999999999998%" headers="mcps1.1.6.1.5 "><p id="p193691154133112"><a name="p193691154133112"></a><a name="p193691154133112"></a>√</p>
</td>
</tr>
<tr id="row260518425310"><td class="cellrowborder" valign="top" width="11.65%" headers="mcps1.1.6.1.1 "><p id="p1060513425310"><a name="p1060513425310"></a><a name="p1060513425310"></a>查询端口详情</p>
</td>
<td class="cellrowborder" valign="top" width="31.53%" headers="mcps1.1.6.1.2 "><p id="p76051344536"><a name="p76051344536"></a><a name="p76051344536"></a>GET /v1/{project_id}/ports<strong id="b72361288312"><a name="b72361288312"></a><a name="b72361288312"></a>/</strong>{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.1.6.1.3 "><p id="p1060514125318"><a name="p1060514125318"></a><a name="p1060514125318"></a>vpc:ports:get</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.029999999999998%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>√</p>
</td>
</tr>
<tr id="row1560612416538"><td class="cellrowborder" valign="top" width="11.65%" headers="mcps1.1.6.1.1 "><p id="p176062475310"><a name="p176062475310"></a><a name="p176062475310"></a>更新端口</p>
</td>
<td class="cellrowborder" valign="top" width="31.53%" headers="mcps1.1.6.1.2 "><p id="p3606045534"><a name="p3606045534"></a><a name="p3606045534"></a>PUT /v1/{project_id}/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.1.6.1.3 "><p id="p1606154165312"><a name="p1606154165312"></a><a name="p1606154165312"></a>vpc:ports:update</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.029999999999998%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>√</p>
</td>
</tr>
<tr id="row126061241530"><td class="cellrowborder" valign="top" width="11.65%" headers="mcps1.1.6.1.1 "><p id="p1760674135315"><a name="p1760674135315"></a><a name="p1760674135315"></a>删除端口</p>
</td>
<td class="cellrowborder" valign="top" width="31.53%" headers="mcps1.1.6.1.2 "><p id="p66061846533"><a name="p66061846533"></a><a name="p66061846533"></a>DELETE /v1/{project_id}/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.1.6.1.3 "><p id="p86062411533"><a name="p86062411533"></a><a name="p86062411533"></a>vpc:ports:delete</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.029999999999998%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>√</p>
</td>
</tr>
<tr id="row16606164125318"><td class="cellrowborder" valign="top" width="11.65%" headers="mcps1.1.6.1.1 "><p id="p860617414533"><a name="p860617414533"></a><a name="p860617414533"></a>创建端口</p>
</td>
<td class="cellrowborder" valign="top" width="31.53%" headers="mcps1.1.6.1.2 "><p id="p8606174115313"><a name="p8606174115313"></a><a name="p8606174115313"></a>POST / v1/{project_id}/ports</p>
</td>
<td class="cellrowborder" valign="top" width="17.4%" headers="mcps1.1.6.1.3 "><p id="p13606154135312"><a name="p13606154135312"></a><a name="p13606154135312"></a>vpc:ports:create</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.029999999999998%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>√</p>
</td>
</tr>
</tbody>
</table>

