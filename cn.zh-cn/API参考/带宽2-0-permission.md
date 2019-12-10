# 带宽（V2.0）<a name="vpc_permission_0018"></a>

<a name="table11714123643216"></a>
<table><thead align="left"><tr id="row1189103603211"><th class="cellrowborder" valign="top" width="40.4040404040404%" id="mcps1.1.5.1.1"><p id="p489173603213"><a name="p489173603213"></a><a name="p489173603213"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.1.5.1.2"><p id="p128919363322"><a name="p128919363322"></a><a name="p128919363322"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="16.16161616161616%" id="mcps1.1.5.1.3"><p id="p1789316368323"><a name="p1789316368323"></a><a name="p1789316368323"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="26.26262626262626%" id="mcps1.1.5.1.4"><p id="p7952202310348"><a name="p7952202310348"></a><a name="p7952202310348"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row2893836163216"><td class="cellrowborder" valign="top" width="40.4040404040404%" headers="mcps1.1.5.1.1 "><p id="p189363623210"><a name="p189363623210"></a><a name="p189363623210"></a>POST /v2.0/{project_id}/bandwidths</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.5.1.2 "><p id="p289363693211"><a name="p289363693211"></a><a name="p289363693211"></a>创建共享带宽</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p16893436153218"><a name="p16893436153218"></a><a name="p16893436153218"></a>vpc:bandwidths:create</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p107185052510"><a name="p107185052510"></a><a name="p107185052510"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row198931336143219"><td class="cellrowborder" valign="top" width="40.4040404040404%" headers="mcps1.1.5.1.1 "><p id="p20893203693218"><a name="p20893203693218"></a><a name="p20893203693218"></a>DELETE /v2.0/{project_id}/bandwidths/{bandwidth_id}</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.5.1.2 "><p id="p19893536143218"><a name="p19893536143218"></a><a name="p19893536143218"></a>删除共享带宽</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p14893163623216"><a name="p14893163623216"></a><a name="p14893163623216"></a>vpc:bandwidths:delete</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p117181501259"><a name="p117181501259"></a><a name="p117181501259"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row1389333616321"><td class="cellrowborder" valign="top" width="40.4040404040404%" headers="mcps1.1.5.1.1 "><p id="p1489311368324"><a name="p1489311368324"></a><a name="p1489311368324"></a>POST /v2.0/{project_id}/bandwidths/{bandwidth_id}/insert</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.5.1.2 "><p id="p98935364327"><a name="p98935364327"></a><a name="p98935364327"></a>共享带宽插入弹性公网IP</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p589483603220"><a name="p589483603220"></a><a name="p589483603220"></a>vpc:publicIps:insert</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p1719903254"><a name="p1719903254"></a><a name="p1719903254"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row289412363329"><td class="cellrowborder" valign="top" width="40.4040404040404%" headers="mcps1.1.5.1.1 "><p id="p6894836163215"><a name="p6894836163215"></a><a name="p6894836163215"></a>POST /v2.0/{project_id}/bandwidths/{bandwidth_id}/remove</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.5.1.2 "><p id="p1989463618324"><a name="p1989463618324"></a><a name="p1989463618324"></a>共享带宽移除弹性公网IP</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p089443619327"><a name="p089443619327"></a><a name="p089443619327"></a>vpc:publicIps:remove</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p19290412354"><a name="p19290412354"></a><a name="p19290412354"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row3894113610320"><td class="cellrowborder" valign="top" width="40.4040404040404%" headers="mcps1.1.5.1.1 "><p id="p68942036153220"><a name="p68942036153220"></a><a name="p68942036153220"></a>PUT /v2.0/{project_id}/bandwidths/{bandwidth_id}</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.5.1.2 "><p id="p28948362320"><a name="p28948362320"></a><a name="p28948362320"></a>更新包周期带宽</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p2894336163213"><a name="p2894336163213"></a><a name="p2894336163213"></a>vpc:bandwidths:update</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p143613463514"><a name="p143613463514"></a><a name="p143613463514"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
</tbody>
</table>

