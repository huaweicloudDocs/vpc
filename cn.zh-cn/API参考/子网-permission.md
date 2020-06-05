# 子网<a name="vpc_permission_0001"></a>

<a name="table66427163617"></a>
<table><thead align="left"><tr id="row112617733610"><th class="cellrowborder" valign="top" width="14.881488148814881%" id="mcps1.1.6.1.1"><p id="p1710122835012"><a name="p1710122835012"></a><a name="p1710122835012"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="28.772877287728775%" id="mcps1.1.6.1.2"><p id="p3595424163511"><a name="p3595424163511"></a><a name="p3595424163511"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="23.352335233523352%" id="mcps1.1.6.1.3"><p id="p181272070365"><a name="p181272070365"></a><a name="p181272070365"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="17.121712171217123%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目</p>
<p id="p1985173683019"><a name="p1985173683019"></a><a name="p1985173683019"></a>(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="15.871587158715872%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目</p>
<p id="p3985193610306"><a name="p3985193610306"></a><a name="p3985193610306"></a>(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row212797103612"><td class="cellrowborder" valign="top" width="14.881488148814881%" headers="mcps1.1.6.1.1 "><p id="p7106283509"><a name="p7106283509"></a><a name="p7106283509"></a>创建子网</p>
</td>
<td class="cellrowborder" valign="top" width="28.772877287728775%" headers="mcps1.1.6.1.2 "><p id="p7127187193615"><a name="p7127187193615"></a><a name="p7127187193615"></a>POST /v1/{project_id}/subnets</p>
</td>
<td class="cellrowborder" valign="top" width="23.352335233523352%" headers="mcps1.1.6.1.3 "><p id="p22919239360"><a name="p22919239360"></a><a name="p22919239360"></a>vpc:subnets:create</p>
</td>
<td class="cellrowborder" valign="top" width="17.121712171217123%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.871587158715872%" headers="mcps1.1.6.1.5 "><p id="p193691154133112"><a name="p193691154133112"></a><a name="p193691154133112"></a>√</p>
</td>
</tr>
<tr id="row101271718364"><td class="cellrowborder" valign="top" width="14.881488148814881%" headers="mcps1.1.6.1.1 "><p id="p191020283509"><a name="p191020283509"></a><a name="p191020283509"></a>查询子网</p>
</td>
<td class="cellrowborder" valign="top" width="28.772877287728775%" headers="mcps1.1.6.1.2 "><p id="p412715783613"><a name="p412715783613"></a><a name="p412715783613"></a>GET /v1/{project_id}/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="23.352335233523352%" headers="mcps1.1.6.1.3 "><p id="p18822246369"><a name="p18822246369"></a><a name="p18822246369"></a>vpc:subnets:get</p>
</td>
<td class="cellrowborder" valign="top" width="17.121712171217123%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.871587158715872%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>√</p>
</td>
</tr>
<tr id="row51276723611"><td class="cellrowborder" valign="top" width="14.881488148814881%" headers="mcps1.1.6.1.1 "><p id="p2108282501"><a name="p2108282501"></a><a name="p2108282501"></a>查询子网列表</p>
</td>
<td class="cellrowborder" valign="top" width="28.772877287728775%" headers="mcps1.1.6.1.2 "><p id="p1712767123613"><a name="p1712767123613"></a><a name="p1712767123613"></a>GET /v1/{project_id}/subnets</p>
</td>
<td class="cellrowborder" valign="top" width="23.352335233523352%" headers="mcps1.1.6.1.3 "><p id="p991414252366"><a name="p991414252366"></a><a name="p991414252366"></a>vpc:subnets:get</p>
</td>
<td class="cellrowborder" valign="top" width="17.121712171217123%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.871587158715872%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>√</p>
</td>
</tr>
<tr id="row31282793612"><td class="cellrowborder" valign="top" width="14.881488148814881%" headers="mcps1.1.6.1.1 "><p id="p201018282502"><a name="p201018282502"></a><a name="p201018282502"></a>更新子网</p>
</td>
<td class="cellrowborder" valign="top" width="28.772877287728775%" headers="mcps1.1.6.1.2 "><p id="p11283773611"><a name="p11283773611"></a><a name="p11283773611"></a>PUT /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="23.352335233523352%" headers="mcps1.1.6.1.3 "><p id="p17254142793617"><a name="p17254142793617"></a><a name="p17254142793617"></a>vpc:subnets:update</p>
</td>
<td class="cellrowborder" valign="top" width="17.121712171217123%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.871587158715872%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>√</p>
</td>
</tr>
<tr id="row61286783611"><td class="cellrowborder" valign="top" width="14.881488148814881%" headers="mcps1.1.6.1.1 "><p id="p111062815013"><a name="p111062815013"></a><a name="p111062815013"></a>删除子网</p>
</td>
<td class="cellrowborder" valign="top" width="28.772877287728775%" headers="mcps1.1.6.1.2 "><p id="p191286723616"><a name="p191286723616"></a><a name="p191286723616"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="23.352335233523352%" headers="mcps1.1.6.1.3 "><p id="p5216172818362"><a name="p5216172818362"></a><a name="p5216172818362"></a>vpc:subnets:delete</p>
</td>
<td class="cellrowborder" valign="top" width="17.121712171217123%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.871587158715872%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>√</p>
</td>
</tr>
</tbody>
</table>

