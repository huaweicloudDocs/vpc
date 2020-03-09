# 子网<a name="vpc_permission_0001"></a>

<a name="table66427163617"></a>
<table><thead align="left"><tr id="row112617733610"><th class="cellrowborder" valign="top" width="34%" id="mcps1.1.5.1.1"><p id="p15126127173610"><a name="p15126127173610"></a><a name="p15126127173610"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.2"><p id="p1710122835012"><a name="p1710122835012"></a><a name="p1710122835012"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p181272070365"><a name="p181272070365"></a><a name="p181272070365"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row212797103612"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p7127187193615"><a name="p7127187193615"></a><a name="p7127187193615"></a>POST /v1/{project_id}/subnets</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p7106283509"><a name="p7106283509"></a><a name="p7106283509"></a>创建子网</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p22919239360"><a name="p22919239360"></a><a name="p22919239360"></a>vpc:subnets:create</p>
</td>
<td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.4 "><p id="p107185052510"><a name="p107185052510"></a><a name="p107185052510"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row101271718364"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p412715783613"><a name="p412715783613"></a><a name="p412715783613"></a>GET /v1/{project_id}/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p191020283509"><a name="p191020283509"></a><a name="p191020283509"></a>查询子网</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p18822246369"><a name="p18822246369"></a><a name="p18822246369"></a>vpc:subnets:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.4 "><p id="p117181501259"><a name="p117181501259"></a><a name="p117181501259"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row51276723611"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p1712767123613"><a name="p1712767123613"></a><a name="p1712767123613"></a>GET /v1/{project_id}/subnets</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p2108282501"><a name="p2108282501"></a><a name="p2108282501"></a>查询子网列表</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p991414252366"><a name="p991414252366"></a><a name="p991414252366"></a>vpc:subnets:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.4 "><p id="p1719903254"><a name="p1719903254"></a><a name="p1719903254"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row31282793612"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p11283773611"><a name="p11283773611"></a><a name="p11283773611"></a>PUT /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p201018282502"><a name="p201018282502"></a><a name="p201018282502"></a>更新子网</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p17254142793617"><a name="p17254142793617"></a><a name="p17254142793617"></a>vpc:subnets:update</p>
</td>
<td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.4 "><p id="p4719701259"><a name="p4719701259"></a><a name="p4719701259"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row61286783611"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p191286723616"><a name="p191286723616"></a><a name="p191286723616"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p111062815013"><a name="p111062815013"></a><a name="p111062815013"></a>删除子网</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p5216172818362"><a name="p5216172818362"></a><a name="p5216172818362"></a>vpc:subnets:delete</p>
</td>
<td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.4 "><p id="p324462512713"><a name="p324462512713"></a><a name="p324462512713"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
</tbody>
</table>

