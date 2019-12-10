# 端口（Openstack Neutron API）<a name="vpc_permission_0010"></a>

<a name="table8513144254019"></a>
<table><thead align="left"><tr id="row1557354254011"><th class="cellrowborder" valign="top" width="30.07920792079208%" id="mcps1.1.5.1.1"><p id="p657310421400"><a name="p657310421400"></a><a name="p657310421400"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="18.435643564356436%" id="mcps1.1.5.1.2"><p id="p6754165316015"><a name="p6754165316015"></a><a name="p6754165316015"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="18.81188118811881%" id="mcps1.1.5.1.3"><p id="p185735424405"><a name="p185735424405"></a><a name="p185735424405"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="32.67326732673268%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row11573842194015"><td class="cellrowborder" valign="top" width="30.07920792079208%" headers="mcps1.1.5.1.1 "><p id="p1557374210407"><a name="p1557374210407"></a><a name="p1557374210407"></a>GET /v2.0/ports</p>
</td>
<td class="cellrowborder" valign="top" width="18.435643564356436%" headers="mcps1.1.5.1.2 "><p id="p3754115316017"><a name="p3754115316017"></a><a name="p3754115316017"></a>查询端口列表</p>
</td>
<td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.3 "><p id="p561665274013"><a name="p561665274013"></a><a name="p561665274013"></a>vpc:ports:get</p>
</td>
<td class="cellrowborder" valign="top" width="32.67326732673268%" headers="mcps1.1.5.1.4 "><a name="ul66241846203119"></a><a name="ul66241846203119"></a><ul id="ul66241846203119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row16573114224014"><td class="cellrowborder" valign="top" width="30.07920792079208%" headers="mcps1.1.5.1.1 "><p id="p135731542134017"><a name="p135731542134017"></a><a name="p135731542134017"></a>GET /v2.0/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="18.435643564356436%" headers="mcps1.1.5.1.2 "><p id="p1875475316019"><a name="p1875475316019"></a><a name="p1875475316019"></a>查询端口</p>
</td>
<td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.3 "><p id="p8780553184014"><a name="p8780553184014"></a><a name="p8780553184014"></a>vpc:ports:get</p>
</td>
<td class="cellrowborder" valign="top" width="32.67326732673268%" headers="mcps1.1.5.1.4 "><a name="ul95023481322"></a><a name="ul95023481322"></a><ul id="ul95023481322"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row195739423404"><td class="cellrowborder" valign="top" width="30.07920792079208%" headers="mcps1.1.5.1.1 "><p id="p5573204234020"><a name="p5573204234020"></a><a name="p5573204234020"></a>POST /v2.0/ports</p>
</td>
<td class="cellrowborder" valign="top" width="18.435643564356436%" headers="mcps1.1.5.1.2 "><p id="p197544533019"><a name="p197544533019"></a><a name="p197544533019"></a>创建端口</p>
</td>
<td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.3 "><p id="p566195516404"><a name="p566195516404"></a><a name="p566195516404"></a>vpc:ports:create</p>
</td>
<td class="cellrowborder" valign="top" width="32.67326732673268%" headers="mcps1.1.5.1.4 "><a name="ul15513950173211"></a><a name="ul15513950173211"></a><ul id="ul15513950173211"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row2057334214016"><td class="cellrowborder" valign="top" width="30.07920792079208%" headers="mcps1.1.5.1.1 "><p id="p13573194234019"><a name="p13573194234019"></a><a name="p13573194234019"></a>PUT /v2.0/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="18.435643564356436%" headers="mcps1.1.5.1.2 "><p id="p1275411531907"><a name="p1275411531907"></a><a name="p1275411531907"></a>更新端口</p>
</td>
<td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.3 "><p id="p161533568406"><a name="p161533568406"></a><a name="p161533568406"></a>vpc:ports:update</p>
</td>
<td class="cellrowborder" valign="top" width="32.67326732673268%" headers="mcps1.1.5.1.4 "><a name="ul33641652103217"></a><a name="ul33641652103217"></a><ul id="ul33641652103217"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row12574642194019"><td class="cellrowborder" valign="top" width="30.07920792079208%" headers="mcps1.1.5.1.1 "><p id="p757464244015"><a name="p757464244015"></a><a name="p757464244015"></a>DELETE /v2.0/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="18.435643564356436%" headers="mcps1.1.5.1.2 "><p id="p197543532019"><a name="p197543532019"></a><a name="p197543532019"></a>删除端口</p>
</td>
<td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.3 "><p id="p0115195711407"><a name="p0115195711407"></a><a name="p0115195711407"></a>vpc:ports:delete</p>
</td>
<td class="cellrowborder" valign="top" width="32.67326732673268%" headers="mcps1.1.5.1.4 "><a name="ul185134914469"></a><a name="ul185134914469"></a><ul id="ul185134914469"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
</tbody>
</table>

