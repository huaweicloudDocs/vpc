# 路由器（Openstack Neutron API）<a name="vpc_permission_0013"></a>

<a name="table12370152544218"></a>
<table><thead align="left"><tr id="row54522258420"><th class="cellrowborder" valign="top" width="12.959999999999999%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="30.42%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="26.650000000000002%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="15.21%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="14.760000000000002%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row184535258423"><td class="cellrowborder" valign="top" width="12.959999999999999%" headers="mcps1.1.6.1.1 "><p id="p739783814417"><a name="p739783814417"></a><a name="p739783814417"></a>查询路由器列表</p>
</td>
<td class="cellrowborder" valign="top" width="30.42%" headers="mcps1.1.6.1.2 "><p id="p18453152554210"><a name="p18453152554210"></a><a name="p18453152554210"></a>GET /v2.0/routers</p>
</td>
<td class="cellrowborder" valign="top" width="26.650000000000002%" headers="mcps1.1.6.1.3 "><p id="p155319335423"><a name="p155319335423"></a><a name="p155319335423"></a>vpc:routers:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.760000000000002%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row745342513426"><td class="cellrowborder" valign="top" width="12.959999999999999%" headers="mcps1.1.6.1.1 "><p id="p153978386410"><a name="p153978386410"></a><a name="p153978386410"></a>查询路由器</p>
</td>
<td class="cellrowborder" valign="top" width="30.42%" headers="mcps1.1.6.1.2 "><p id="p345362534211"><a name="p345362534211"></a><a name="p345362534211"></a>GET /v2.0/routers/{router_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.650000000000002%" headers="mcps1.1.6.1.3 "><p id="p5859534164219"><a name="p5859534164219"></a><a name="p5859534164219"></a>vpc:routers:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.760000000000002%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row54531525184217"><td class="cellrowborder" valign="top" width="12.959999999999999%" headers="mcps1.1.6.1.1 "><p id="p103976387420"><a name="p103976387420"></a><a name="p103976387420"></a>创建路由器</p>
</td>
<td class="cellrowborder" valign="top" width="30.42%" headers="mcps1.1.6.1.2 "><p id="p15453925114210"><a name="p15453925114210"></a><a name="p15453925114210"></a>POST /v2.0/routers</p>
</td>
<td class="cellrowborder" valign="top" width="26.650000000000002%" headers="mcps1.1.6.1.3 "><p id="p2990735114210"><a name="p2990735114210"></a><a name="p2990735114210"></a>vpc:routers:create</p>
</td>
<td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.760000000000002%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row174531925144217"><td class="cellrowborder" valign="top" width="12.959999999999999%" headers="mcps1.1.6.1.1 "><p id="p1139718381747"><a name="p1139718381747"></a><a name="p1139718381747"></a>更新路由器</p>
</td>
<td class="cellrowborder" valign="top" width="30.42%" headers="mcps1.1.6.1.2 "><p id="p84531425114218"><a name="p84531425114218"></a><a name="p84531425114218"></a>PUT /v2.0/routers/{router_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.650000000000002%" headers="mcps1.1.6.1.3 "><p id="p1124333711420"><a name="p1124333711420"></a><a name="p1124333711420"></a>vpc:routers:update</p>
</td>
<td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.760000000000002%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>×</p>
</td>
</tr>
<tr id="row1345318250425"><td class="cellrowborder" valign="top" width="12.959999999999999%" headers="mcps1.1.6.1.1 "><p id="p143970384417"><a name="p143970384417"></a><a name="p143970384417"></a>删除路由器</p>
</td>
<td class="cellrowborder" valign="top" width="30.42%" headers="mcps1.1.6.1.2 "><p id="p1045312259426"><a name="p1045312259426"></a><a name="p1045312259426"></a>DELETE /v2.0/routers/{router_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.650000000000002%" headers="mcps1.1.6.1.3 "><p id="p1094017388427"><a name="p1094017388427"></a><a name="p1094017388427"></a>vpc:routers:delete</p>
</td>
<td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.6.1.4 "><p id="p1267045134615"><a name="p1267045134615"></a><a name="p1267045134615"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.760000000000002%" headers="mcps1.1.6.1.5 "><p id="p6670155114465"><a name="p6670155114465"></a><a name="p6670155114465"></a>×</p>
</td>
</tr>
<tr id="row545315256423"><td class="cellrowborder" valign="top" width="12.959999999999999%" headers="mcps1.1.6.1.1 "><p id="p1339716386413"><a name="p1339716386413"></a><a name="p1339716386413"></a>添加路由器接口</p>
</td>
<td class="cellrowborder" valign="top" width="30.42%" headers="mcps1.1.6.1.2 "><p id="p1045312515428"><a name="p1045312515428"></a><a name="p1045312515428"></a>PUT /v2.0/routers/{router_id}/add_router_interface</p>
</td>
<td class="cellrowborder" valign="top" width="26.650000000000002%" headers="mcps1.1.6.1.3 "><a name="ul15454162520421"></a><a name="ul15454162520421"></a><ul id="ul15454162520421"><li>vpc:routers:addInterface</li><li>vpc:routers:get</li></ul>
</td>
<td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.6.1.4 "><p id="p5670165120466"><a name="p5670165120466"></a><a name="p5670165120466"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.760000000000002%" headers="mcps1.1.6.1.5 "><p id="p167055174612"><a name="p167055174612"></a><a name="p167055174612"></a>×</p>
</td>
</tr>
<tr id="row145472554213"><td class="cellrowborder" valign="top" width="12.959999999999999%" headers="mcps1.1.6.1.1 "><p id="p1539712389410"><a name="p1539712389410"></a><a name="p1539712389410"></a>删除路由器接口</p>
</td>
<td class="cellrowborder" valign="top" width="30.42%" headers="mcps1.1.6.1.2 "><p id="p1745412518421"><a name="p1745412518421"></a><a name="p1745412518421"></a>PUT /v2.0/routers/{router_id}/remove_router_interface</p>
</td>
<td class="cellrowborder" valign="top" width="26.650000000000002%" headers="mcps1.1.6.1.3 "><a name="ul18454122574216"></a><a name="ul18454122574216"></a><ul id="ul18454122574216"><li>vpc:routers:removeInterface</li><li>vpc:routers:get</li></ul>
</td>
<td class="cellrowborder" valign="top" width="15.21%" headers="mcps1.1.6.1.4 "><p id="p124481181145"><a name="p124481181145"></a><a name="p124481181145"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="14.760000000000002%" headers="mcps1.1.6.1.5 "><p id="p1448587419"><a name="p1448587419"></a><a name="p1448587419"></a>×</p>
</td>
</tr>
</tbody>
</table>

