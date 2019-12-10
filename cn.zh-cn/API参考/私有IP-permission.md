# 私有IP<a name="ZH-CN_TOPIC_0201534089"></a>

<a name="table967413133817"></a>
<table><thead align="left"><tr id="row9708231163820"><th class="cellrowborder" valign="top" width="37%" id="mcps1.1.5.1.1"><p id="p1970823143813"><a name="p1970823143813"></a><a name="p1970823143813"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.2"><p id="p12638211185918"><a name="p12638211185918"></a><a name="p12638211185918"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p137081931143810"><a name="p137081931143810"></a><a name="p137081931143810"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="26%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row197081331113817"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p17091031143815"><a name="p17091031143815"></a><a name="p17091031143815"></a>POST /v1/{project_id}/privateips</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p9638111155912"><a name="p9638111155912"></a><a name="p9638111155912"></a>申请私有IP</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p13892440173820"><a name="p13892440173820"></a><a name="p13892440173820"></a>vpc:privateIps:create</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul66241846203119"></a><a name="ul66241846203119"></a><ul id="ul66241846203119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row15709203163811"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p7709103117385"><a name="p7709103117385"></a><a name="p7709103117385"></a>GET /v1/{project_id}/privateips/{privateip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p363851114598"><a name="p363851114598"></a><a name="p363851114598"></a>查询私有IP</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p9226104210387"><a name="p9226104210387"></a><a name="p9226104210387"></a>vpc:privateIps:get</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul95023481322"></a><a name="ul95023481322"></a><ul id="ul95023481322"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1670914317388"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p17709831173812"><a name="p17709831173812"></a><a name="p17709831173812"></a>GET /v1/{project_id}/subnets/{subnet_id}/privateips</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p8638811165911"><a name="p8638811165911"></a><a name="p8638811165911"></a>查询私有IP列表</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p1724712431387"><a name="p1724712431387"></a><a name="p1724712431387"></a>vpc:privateIps:list</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul15513950173211"></a><a name="ul15513950173211"></a><ul id="ul15513950173211"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row6709163118385"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p14709143173818"><a name="p14709143173818"></a><a name="p14709143173818"></a>DELETE /v1/{project_id}/privateips/{privateip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p6638181175920"><a name="p6638181175920"></a><a name="p6638181175920"></a>删除私有IP</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p12681044203812"><a name="p12681044203812"></a><a name="p12681044203812"></a>vpc:privateIps:delete</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul33641652103217"></a><a name="ul33641652103217"></a><ul id="ul33641652103217"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
</tbody>
</table>

