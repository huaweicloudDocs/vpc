# 端口（Openstack Neutron API）<a name="vpc_permission_0010"></a>

<a name="table8513144254019"></a>
<table><thead align="left"><tr id="row1557354254011"><th class="cellrowborder" valign="top" width="12.261226122612262%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="30.763076307630765%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="21.452145214521455%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="17.761776177617765%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="17.761776177617765%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row11573842194015"><td class="cellrowborder" valign="top" width="12.261226122612262%" headers="mcps1.1.6.1.1 "><p id="p3754115316017"><a name="p3754115316017"></a><a name="p3754115316017"></a>查询端口列表</p>
</td>
<td class="cellrowborder" valign="top" width="30.763076307630765%" headers="mcps1.1.6.1.2 "><p id="p1557374210407"><a name="p1557374210407"></a><a name="p1557374210407"></a>GET /v2.0/ports</p>
</td>
<td class="cellrowborder" valign="top" width="21.452145214521455%" headers="mcps1.1.6.1.3 "><p id="p561665274013"><a name="p561665274013"></a><a name="p561665274013"></a>vpc:ports:get</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row16573114224014"><td class="cellrowborder" valign="top" width="12.261226122612262%" headers="mcps1.1.6.1.1 "><p id="p1875475316019"><a name="p1875475316019"></a><a name="p1875475316019"></a>查询端口</p>
</td>
<td class="cellrowborder" valign="top" width="30.763076307630765%" headers="mcps1.1.6.1.2 "><p id="p135731542134017"><a name="p135731542134017"></a><a name="p135731542134017"></a>GET /v2.0/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.452145214521455%" headers="mcps1.1.6.1.3 "><p id="p8780553184014"><a name="p8780553184014"></a><a name="p8780553184014"></a>vpc:ports:get</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row195739423404"><td class="cellrowborder" valign="top" width="12.261226122612262%" headers="mcps1.1.6.1.1 "><p id="p197544533019"><a name="p197544533019"></a><a name="p197544533019"></a>创建端口</p>
</td>
<td class="cellrowborder" valign="top" width="30.763076307630765%" headers="mcps1.1.6.1.2 "><p id="p5573204234020"><a name="p5573204234020"></a><a name="p5573204234020"></a>POST /v2.0/ports</p>
</td>
<td class="cellrowborder" valign="top" width="21.452145214521455%" headers="mcps1.1.6.1.3 "><p id="p566195516404"><a name="p566195516404"></a><a name="p566195516404"></a>vpc:ports:create</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row2057334214016"><td class="cellrowborder" valign="top" width="12.261226122612262%" headers="mcps1.1.6.1.1 "><p id="p1275411531907"><a name="p1275411531907"></a><a name="p1275411531907"></a>更新端口</p>
</td>
<td class="cellrowborder" valign="top" width="30.763076307630765%" headers="mcps1.1.6.1.2 "><p id="p13573194234019"><a name="p13573194234019"></a><a name="p13573194234019"></a>PUT /v2.0/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.452145214521455%" headers="mcps1.1.6.1.3 "><p id="p161533568406"><a name="p161533568406"></a><a name="p161533568406"></a>vpc:ports:update</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>×</p>
</td>
</tr>
<tr id="row12574642194019"><td class="cellrowborder" valign="top" width="12.261226122612262%" headers="mcps1.1.6.1.1 "><p id="p197543532019"><a name="p197543532019"></a><a name="p197543532019"></a>删除端口</p>
</td>
<td class="cellrowborder" valign="top" width="30.763076307630765%" headers="mcps1.1.6.1.2 "><p id="p757464244015"><a name="p757464244015"></a><a name="p757464244015"></a>DELETE /v2.0/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.452145214521455%" headers="mcps1.1.6.1.3 "><p id="p0115195711407"><a name="p0115195711407"></a><a name="p0115195711407"></a>vpc:ports:delete</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.4 "><p id="p1267045134615"><a name="p1267045134615"></a><a name="p1267045134615"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.761776177617765%" headers="mcps1.1.6.1.5 "><p id="p6670155114465"><a name="p6670155114465"></a><a name="p6670155114465"></a>×</p>
</td>
</tr>
</tbody>
</table>

