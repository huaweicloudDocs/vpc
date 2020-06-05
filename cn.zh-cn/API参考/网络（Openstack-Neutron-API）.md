# 网络（Openstack Neutron API）<a name="vpc_permission_0011"></a>

<a name="table11673171511413"></a>
<table><thead align="left"><tr id="row15732115164110"><th class="cellrowborder" valign="top" width="10.67%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="27.6%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="21.39%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="19.759999999999998%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="20.580000000000002%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row157326156414"><td class="cellrowborder" valign="top" width="10.67%" headers="mcps1.1.6.1.1 "><p id="p84753589117"><a name="p84753589117"></a><a name="p84753589117"></a>查询网络列表</p>
</td>
<td class="cellrowborder" valign="top" width="27.6%" headers="mcps1.1.6.1.2 "><p id="p1173212156415"><a name="p1173212156415"></a><a name="p1173212156415"></a>GET /v2.0/networks</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.3 "><p id="p135711055124116"><a name="p135711055124116"></a><a name="p135711055124116"></a>vpc:networks:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.759999999999998%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.580000000000002%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row77321415184117"><td class="cellrowborder" valign="top" width="10.67%" headers="mcps1.1.6.1.1 "><p id="p164756582018"><a name="p164756582018"></a><a name="p164756582018"></a>查询网络</p>
</td>
<td class="cellrowborder" valign="top" width="27.6%" headers="mcps1.1.6.1.2 "><p id="p1773241564114"><a name="p1773241564114"></a><a name="p1773241564114"></a>GET /v2.0/networks/{network_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.3 "><p id="p1887275654110"><a name="p1887275654110"></a><a name="p1887275654110"></a>vpc:networks:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.759999999999998%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.580000000000002%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row6733181554110"><td class="cellrowborder" valign="top" width="10.67%" headers="mcps1.1.6.1.1 "><p id="p947510581319"><a name="p947510581319"></a><a name="p947510581319"></a>创建网络</p>
</td>
<td class="cellrowborder" valign="top" width="27.6%" headers="mcps1.1.6.1.2 "><p id="p6733515124120"><a name="p6733515124120"></a><a name="p6733515124120"></a>POST /v2.0/networks</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.3 "><p id="p106995817411"><a name="p106995817411"></a><a name="p106995817411"></a>vpc:networks:create</p>
</td>
<td class="cellrowborder" valign="top" width="19.759999999999998%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.580000000000002%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row1373361534112"><td class="cellrowborder" valign="top" width="10.67%" headers="mcps1.1.6.1.1 "><p id="p4476165810113"><a name="p4476165810113"></a><a name="p4476165810113"></a>更新网络</p>
</td>
<td class="cellrowborder" valign="top" width="27.6%" headers="mcps1.1.6.1.2 "><p id="p4733101504111"><a name="p4733101504111"></a><a name="p4733101504111"></a>PUT /v2.0/networks/{network_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.3 "><p id="p202391459194120"><a name="p202391459194120"></a><a name="p202391459194120"></a>vpc:networks:update</p>
</td>
<td class="cellrowborder" valign="top" width="19.759999999999998%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.580000000000002%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>×</p>
</td>
</tr>
<tr id="row20733111574111"><td class="cellrowborder" valign="top" width="10.67%" headers="mcps1.1.6.1.1 "><p id="p247615588112"><a name="p247615588112"></a><a name="p247615588112"></a>删除网络</p>
</td>
<td class="cellrowborder" valign="top" width="27.6%" headers="mcps1.1.6.1.2 "><p id="p5733201511416"><a name="p5733201511416"></a><a name="p5733201511416"></a>DELETE /v2.0/networks/{network_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.39%" headers="mcps1.1.6.1.3 "><p id="p19356507425"><a name="p19356507425"></a><a name="p19356507425"></a>vpc:networks:delete</p>
</td>
<td class="cellrowborder" valign="top" width="19.759999999999998%" headers="mcps1.1.6.1.4 "><p id="p1267045134615"><a name="p1267045134615"></a><a name="p1267045134615"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.580000000000002%" headers="mcps1.1.6.1.5 "><p id="p6670155114465"><a name="p6670155114465"></a><a name="p6670155114465"></a>×</p>
</td>
</tr>
</tbody>
</table>

