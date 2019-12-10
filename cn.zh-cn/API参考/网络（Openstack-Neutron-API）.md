# 网络（Openstack Neutron API）<a name="ZH-CN_TOPIC_0201534129"></a>

<a name="table11673171511413"></a>
<table><thead align="left"><tr id="row15732115164110"><th class="cellrowborder" valign="top" width="37%" id="mcps1.1.5.1.1"><p id="p17732101524116"><a name="p17732101524116"></a><a name="p17732101524116"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.1.5.1.2"><p id="p104751580113"><a name="p104751580113"></a><a name="p104751580113"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.3"><p id="p373241524117"><a name="p373241524117"></a><a name="p373241524117"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="32%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row157326156414"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p1173212156415"><a name="p1173212156415"></a><a name="p1173212156415"></a>GET /v2.0/networks</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p84753589117"><a name="p84753589117"></a><a name="p84753589117"></a>查询网络列表</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p135711055124116"><a name="p135711055124116"></a><a name="p135711055124116"></a>vpc:networks:get</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul66241846203119"></a><a name="ul66241846203119"></a><ul id="ul66241846203119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row77321415184117"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p1773241564114"><a name="p1773241564114"></a><a name="p1773241564114"></a>GET /v2.0/networks/{network_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p164756582018"><a name="p164756582018"></a><a name="p164756582018"></a>查询网络</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p1887275654110"><a name="p1887275654110"></a><a name="p1887275654110"></a>vpc:networks:get</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul95023481322"></a><a name="ul95023481322"></a><ul id="ul95023481322"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row6733181554110"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p6733515124120"><a name="p6733515124120"></a><a name="p6733515124120"></a>POST /v2.0/networks</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p947510581319"><a name="p947510581319"></a><a name="p947510581319"></a>创建网络</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p106995817411"><a name="p106995817411"></a><a name="p106995817411"></a>vpc:networks:create</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul15513950173211"></a><a name="ul15513950173211"></a><ul id="ul15513950173211"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1373361534112"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p4733101504111"><a name="p4733101504111"></a><a name="p4733101504111"></a>PUT /v2.0/networks/{network_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p4476165810113"><a name="p4476165810113"></a><a name="p4476165810113"></a>更新网络</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p202391459194120"><a name="p202391459194120"></a><a name="p202391459194120"></a>vpc:networks:update</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul33641652103217"></a><a name="ul33641652103217"></a><ul id="ul33641652103217"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row20733111574111"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p5733201511416"><a name="p5733201511416"></a><a name="p5733201511416"></a>DELETE /v2.0/networks/{network_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p247615588112"><a name="p247615588112"></a><a name="p247615588112"></a>删除网络</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p19356507425"><a name="p19356507425"></a><a name="p19356507425"></a>vpc:networks:delete</p>
</td>
<td class="cellrowborder" valign="top" width="32%" headers="mcps1.1.5.1.4 "><a name="ul185134914469"></a><a name="ul185134914469"></a><ul id="ul185134914469"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
</tbody>
</table>

