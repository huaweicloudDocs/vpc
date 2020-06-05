# VPC标签<a name="vpc_permission_0021"></a>

<a name="table8513144254019"></a>
<table><thead align="left"><tr id="row1557354254011"><th class="cellrowborder" valign="top" width="16.881688168816883%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="27.722772277227726%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="21.19211921192119%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="16.28162816281628%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="17.92179217921792%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row11573842194015"><td class="cellrowborder" valign="top" width="16.881688168816883%" headers="mcps1.1.6.1.1 "><p id="p970935115520"><a name="p970935115520"></a><a name="p970935115520"></a>创建VPC资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.1.6.1.2 "><p id="p1994810358574"><a name="p1994810358574"></a><a name="p1994810358574"></a>POST /v2.0/{project_id}/vpcs/{vpc_id}/tags</p>
</td>
<td class="cellrowborder" valign="top" width="21.19211921192119%" headers="mcps1.1.6.1.3 "><p id="p6708115185520"><a name="p6708115185520"></a><a name="p6708115185520"></a>vpc:vpcTags:create</p>
</td>
<td class="cellrowborder" valign="top" width="16.28162816281628%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.92179217921792%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row16573114224014"><td class="cellrowborder" valign="top" width="16.881688168816883%" headers="mcps1.1.6.1.1 "><p id="p157011510557"><a name="p157011510557"></a><a name="p157011510557"></a>查询VPC资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.1.6.1.2 "><p id="p1970318535520"><a name="p1970318535520"></a><a name="p1970318535520"></a>GET /v2.0/{project_id}/vpcs/{vpc_id}/tags</p>
</td>
<td class="cellrowborder" valign="top" width="21.19211921192119%" headers="mcps1.1.6.1.3 "><p id="p470015195511"><a name="p470015195511"></a><a name="p470015195511"></a>vpc:vpcTags:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.28162816281628%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.92179217921792%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row195739423404"><td class="cellrowborder" valign="top" width="16.881688168816883%" headers="mcps1.1.6.1.1 "><p id="p126964517555"><a name="p126964517555"></a><a name="p126964517555"></a>删除VPC资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.1.6.1.2 "><p id="p206975519551"><a name="p206975519551"></a><a name="p206975519551"></a>DELETE /v2.0/{project_id}/vpcs/{vpc_id}/tags/{key}</p>
</td>
<td class="cellrowborder" valign="top" width="21.19211921192119%" headers="mcps1.1.6.1.3 "><p id="p1669515510552"><a name="p1669515510552"></a><a name="p1669515510552"></a>vpc:vpcTags:delete</p>
</td>
<td class="cellrowborder" valign="top" width="16.28162816281628%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.92179217921792%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row2057334214016"><td class="cellrowborder" valign="top" width="16.881688168816883%" headers="mcps1.1.6.1.1 "><p id="p11686259551"><a name="p11686259551"></a><a name="p11686259551"></a>批量创建和删除VPC资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.1.6.1.2 "><p id="p668914517552"><a name="p668914517552"></a><a name="p668914517552"></a>POST /v2.0/{project_id}/vpcs/{vpc_id}/tags/action</p>
</td>
<td class="cellrowborder" valign="top" width="21.19211921192119%" headers="mcps1.1.6.1.3 "><p id="p12618529014"><a name="p12618529014"></a><a name="p12618529014"></a>vpc:vpcTags:create</p>
<p id="p568585115519"><a name="p568585115519"></a><a name="p568585115519"></a>vpc:vpcTags:delete</p>
</td>
<td class="cellrowborder" valign="top" width="16.28162816281628%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.92179217921792%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>×</p>
</td>
</tr>
<tr id="row1141921219586"><td class="cellrowborder" valign="top" width="16.881688168816883%" headers="mcps1.1.6.1.1 "><p id="p1242216120589"><a name="p1242216120589"></a><a name="p1242216120589"></a>查询VPC资源实例</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.1.6.1.2 "><p id="p842291235811"><a name="p842291235811"></a><a name="p842291235811"></a>POST /v2.0/{project_id}/vpcs/resource_instances/action</p>
</td>
<td class="cellrowborder" valign="top" width="21.19211921192119%" headers="mcps1.1.6.1.3 "><p id="p16422151245812"><a name="p16422151245812"></a><a name="p16422151245812"></a>vpc:vpcTags:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.28162816281628%" headers="mcps1.1.6.1.4 "><p id="p1267045134615"><a name="p1267045134615"></a><a name="p1267045134615"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.92179217921792%" headers="mcps1.1.6.1.5 "><p id="p6670155114465"><a name="p6670155114465"></a><a name="p6670155114465"></a>×</p>
</td>
</tr>
<tr id="row65981915155810"><td class="cellrowborder" valign="top" width="16.881688168816883%" headers="mcps1.1.6.1.1 "><p id="p11599181585812"><a name="p11599181585812"></a><a name="p11599181585812"></a>查询VPC项目标签</p>
</td>
<td class="cellrowborder" valign="top" width="27.722772277227726%" headers="mcps1.1.6.1.2 "><p id="p117106575512"><a name="p117106575512"></a><a name="p117106575512"></a>GET /v2.0/{project_id}/vpcs/tags</p>
</td>
<td class="cellrowborder" valign="top" width="21.19211921192119%" headers="mcps1.1.6.1.3 "><p id="p5599171518589"><a name="p5599171518589"></a><a name="p5599171518589"></a>vpc:vpcTags:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.28162816281628%" headers="mcps1.1.6.1.4 "><p id="p5670165120466"><a name="p5670165120466"></a><a name="p5670165120466"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.92179217921792%" headers="mcps1.1.6.1.5 "><p id="p167055174612"><a name="p167055174612"></a><a name="p167055174612"></a>×</p>
</td>
</tr>
</tbody>
</table>

