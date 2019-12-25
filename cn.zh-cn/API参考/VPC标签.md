# VPC标签<a name="vpc_permission_0021"></a>

<a name="table8513144254019"></a>
<table><thead align="left"><tr id="row1557354254011"><th class="cellrowborder" valign="top" width="33.27722772277228%" id="mcps1.1.5.1.1"><p id="p657310421400"><a name="p657310421400"></a><a name="p657310421400"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="15.237623762376238%" id="mcps1.1.5.1.2"><p id="p6754165316015"><a name="p6754165316015"></a><a name="p6754165316015"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="18.475247524752476%" id="mcps1.1.5.1.3"><p id="p185735424405"><a name="p185735424405"></a><a name="p185735424405"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="33.009900990099005%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row11573842194015"><td class="cellrowborder" valign="top" width="33.27722772277228%" headers="mcps1.1.5.1.1 "><p id="p1994810358574"><a name="p1994810358574"></a><a name="p1994810358574"></a>POST /v2.0/{project_id}/vpcs/{vpc_id}/tags</p>
</td>
<td class="cellrowborder" valign="top" width="15.237623762376238%" headers="mcps1.1.5.1.2 "><p id="p970935115520"><a name="p970935115520"></a><a name="p970935115520"></a>创建VPC资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="18.475247524752476%" headers="mcps1.1.5.1.3 "><p id="p6708115185520"><a name="p6708115185520"></a><a name="p6708115185520"></a>vpc:vpcTags:create</p>
</td>
<td class="cellrowborder" valign="top" width="33.009900990099005%" headers="mcps1.1.5.1.4 "><a name="ul1698036164514"></a><a name="ul1698036164514"></a><ul id="ul1698036164514"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row16573114224014"><td class="cellrowborder" valign="top" width="33.27722772277228%" headers="mcps1.1.5.1.1 "><p id="p1970318535520"><a name="p1970318535520"></a><a name="p1970318535520"></a>GET /v2.0/{project_id}/vpcs/{vpc_id}/tags</p>
</td>
<td class="cellrowborder" valign="top" width="15.237623762376238%" headers="mcps1.1.5.1.2 "><p id="p157011510557"><a name="p157011510557"></a><a name="p157011510557"></a>查询VPC资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="18.475247524752476%" headers="mcps1.1.5.1.3 "><p id="p470015195511"><a name="p470015195511"></a><a name="p470015195511"></a>vpc:vpcTags:get</p>
</td>
<td class="cellrowborder" valign="top" width="33.009900990099005%" headers="mcps1.1.5.1.4 "><a name="ul1982018556594"></a><a name="ul1982018556594"></a><ul id="ul1982018556594"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row195739423404"><td class="cellrowborder" valign="top" width="33.27722772277228%" headers="mcps1.1.5.1.1 "><p id="p206975519551"><a name="p206975519551"></a><a name="p206975519551"></a>DELETE /v2.0/{project_id}/vpcs/{vpc_id}/tags/{key}</p>
</td>
<td class="cellrowborder" valign="top" width="15.237623762376238%" headers="mcps1.1.5.1.2 "><p id="p126964517555"><a name="p126964517555"></a><a name="p126964517555"></a>删除VPC资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="18.475247524752476%" headers="mcps1.1.5.1.3 "><p id="p1669515510552"><a name="p1669515510552"></a><a name="p1669515510552"></a>vpc:vpcTags:delete</p>
</td>
<td class="cellrowborder" valign="top" width="33.009900990099005%" headers="mcps1.1.5.1.4 "><a name="ul1381845613592"></a><a name="ul1381845613592"></a><ul id="ul1381845613592"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row2057334214016"><td class="cellrowborder" valign="top" width="33.27722772277228%" headers="mcps1.1.5.1.1 "><p id="p668914517552"><a name="p668914517552"></a><a name="p668914517552"></a>POST /v2.0/{project_id}/vpcs/{vpc_id}/tags/action</p>
</td>
<td class="cellrowborder" valign="top" width="15.237623762376238%" headers="mcps1.1.5.1.2 "><p id="p11686259551"><a name="p11686259551"></a><a name="p11686259551"></a>批量创建和删除VPC资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="18.475247524752476%" headers="mcps1.1.5.1.3 "><p id="p12618529014"><a name="p12618529014"></a><a name="p12618529014"></a>vpc:vpcTags:create</p>
<p id="p568585115519"><a name="p568585115519"></a><a name="p568585115519"></a>vpc:vpcTags:delete</p>
</td>
<td class="cellrowborder" valign="top" width="33.009900990099005%" headers="mcps1.1.5.1.4 "><a name="ul66121457145918"></a><a name="ul66121457145918"></a><ul id="ul66121457145918"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1141921219586"><td class="cellrowborder" valign="top" width="33.27722772277228%" headers="mcps1.1.5.1.1 "><p id="p842291235811"><a name="p842291235811"></a><a name="p842291235811"></a>POST /v2.0/{project_id}/vpcs/resource_instances/action</p>
</td>
<td class="cellrowborder" valign="top" width="15.237623762376238%" headers="mcps1.1.5.1.2 "><p id="p1242216120589"><a name="p1242216120589"></a><a name="p1242216120589"></a>查询VPC资源实例</p>
</td>
<td class="cellrowborder" valign="top" width="18.475247524752476%" headers="mcps1.1.5.1.3 "><p id="p16422151245812"><a name="p16422151245812"></a><a name="p16422151245812"></a>vpc:vpcTags:get</p>
</td>
<td class="cellrowborder" valign="top" width="33.009900990099005%" headers="mcps1.1.5.1.4 "><a name="ul1155955819590"></a><a name="ul1155955819590"></a><ul id="ul1155955819590"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row65981915155810"><td class="cellrowborder" valign="top" width="33.27722772277228%" headers="mcps1.1.5.1.1 "><p id="p117106575512"><a name="p117106575512"></a><a name="p117106575512"></a>GET /v2.0/{project_id}/vpcs/tags</p>
</td>
<td class="cellrowborder" valign="top" width="15.237623762376238%" headers="mcps1.1.5.1.2 "><p id="p11599181585812"><a name="p11599181585812"></a><a name="p11599181585812"></a>查询VPC项目标签</p>
</td>
<td class="cellrowborder" valign="top" width="18.475247524752476%" headers="mcps1.1.5.1.3 "><p id="p5599171518589"><a name="p5599171518589"></a><a name="p5599171518589"></a>vpc:vpcTags:get</p>
</td>
<td class="cellrowborder" valign="top" width="33.009900990099005%" headers="mcps1.1.5.1.4 "><a name="ul21791902013"></a><a name="ul21791902013"></a><ul id="ul21791902013"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
</tbody>
</table>

