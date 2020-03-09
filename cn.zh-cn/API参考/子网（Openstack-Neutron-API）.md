# 子网（Openstack Neutron API）<a name="vpc_permission_0012"></a>

<a name="table9659193744115"></a>
<table><thead align="left"><tr id="row071163754111"><th class="cellrowborder" valign="top" width="37%" id="mcps1.1.5.1.1"><p id="p1771111373414"><a name="p1771111373414"></a><a name="p1771111373414"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.1.5.1.2"><p id="p10211361931"><a name="p10211361931"></a><a name="p10211361931"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.3"><p id="p1271153710410"><a name="p1271153710410"></a><a name="p1271153710410"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="32%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row0711337154111"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p2071117371413"><a name="p2071117371413"></a><a name="p2071117371413"></a>GET /v2.0/subnets</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p1921436431"><a name="p1921436431"></a><a name="p1921436431"></a>查询子网列表</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p059364534118"><a name="p059364534118"></a><a name="p059364534118"></a>vpc:subnets:get</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul66241846203119"></a><a name="ul66241846203119"></a><ul id="ul66241846203119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row14711537104116"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p15711113716411"><a name="p15711113716411"></a><a name="p15711113716411"></a>GET /v2.0/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p42536536"><a name="p42536536"></a><a name="p42536536"></a>查询子网</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p0174248154115"><a name="p0174248154115"></a><a name="p0174248154115"></a>vpc:subnets:get</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul95023481322"></a><a name="ul95023481322"></a><ul id="ul95023481322"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row13712143724114"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p1271213714120"><a name="p1271213714120"></a><a name="p1271213714120"></a>POST /v2.0/subnets</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p92836933"><a name="p92836933"></a><a name="p92836933"></a>创建子网</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p208115493416"><a name="p208115493416"></a><a name="p208115493416"></a>vpc:subnets:create</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul15513950173211"></a><a name="ul15513950173211"></a><ul id="ul15513950173211"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row471283794113"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p19712163774111"><a name="p19712163774111"></a><a name="p19712163774111"></a>PUT /v2.0/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p12215367317"><a name="p12215367317"></a><a name="p12215367317"></a>更新子网</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p1575419512413"><a name="p1575419512413"></a><a name="p1575419512413"></a>vpc:subnets:update</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul33641652103217"></a><a name="ul33641652103217"></a><ul id="ul33641652103217"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row177121437194112"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p6712133734118"><a name="p6712133734118"></a><a name="p6712133734118"></a>DELETE /v2.0/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p1253619313"><a name="p1253619313"></a><a name="p1253619313"></a>删除子网</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p7221453164112"><a name="p7221453164112"></a><a name="p7221453164112"></a>vpc:subnets:delete</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul185134914469"></a><a name="ul185134914469"></a><ul id="ul185134914469"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
</tbody>
</table>

