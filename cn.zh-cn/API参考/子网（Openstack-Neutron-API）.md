# 子网（Openstack Neutron API）<a name="vpc_permission_0012"></a>

<a name="table9659193744115"></a>
<table><thead align="left"><tr id="row071163754111"><th class="cellrowborder" valign="top" width="11.98%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="26.63%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="21.240000000000002%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="20.06%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="20.09%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row0711337154111"><td class="cellrowborder" valign="top" width="11.98%" headers="mcps1.1.6.1.1 "><p id="p1921436431"><a name="p1921436431"></a><a name="p1921436431"></a>查询子网列表</p>
</td>
<td class="cellrowborder" valign="top" width="26.63%" headers="mcps1.1.6.1.2 "><p id="p2071117371413"><a name="p2071117371413"></a><a name="p2071117371413"></a>GET /v2.0/subnets</p>
</td>
<td class="cellrowborder" valign="top" width="21.240000000000002%" headers="mcps1.1.6.1.3 "><p id="p059364534118"><a name="p059364534118"></a><a name="p059364534118"></a>vpc:subnets:get</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row14711537104116"><td class="cellrowborder" valign="top" width="11.98%" headers="mcps1.1.6.1.1 "><p id="p42536536"><a name="p42536536"></a><a name="p42536536"></a>查询子网</p>
</td>
<td class="cellrowborder" valign="top" width="26.63%" headers="mcps1.1.6.1.2 "><p id="p15711113716411"><a name="p15711113716411"></a><a name="p15711113716411"></a>GET /v2.0/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.240000000000002%" headers="mcps1.1.6.1.3 "><p id="p0174248154115"><a name="p0174248154115"></a><a name="p0174248154115"></a>vpc:subnets:get</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row13712143724114"><td class="cellrowborder" valign="top" width="11.98%" headers="mcps1.1.6.1.1 "><p id="p92836933"><a name="p92836933"></a><a name="p92836933"></a>创建子网</p>
</td>
<td class="cellrowborder" valign="top" width="26.63%" headers="mcps1.1.6.1.2 "><p id="p1271213714120"><a name="p1271213714120"></a><a name="p1271213714120"></a>POST /v2.0/subnets</p>
</td>
<td class="cellrowborder" valign="top" width="21.240000000000002%" headers="mcps1.1.6.1.3 "><p id="p208115493416"><a name="p208115493416"></a><a name="p208115493416"></a>vpc:subnets:create</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row471283794113"><td class="cellrowborder" valign="top" width="11.98%" headers="mcps1.1.6.1.1 "><p id="p12215367317"><a name="p12215367317"></a><a name="p12215367317"></a>更新子网</p>
</td>
<td class="cellrowborder" valign="top" width="26.63%" headers="mcps1.1.6.1.2 "><p id="p19712163774111"><a name="p19712163774111"></a><a name="p19712163774111"></a>PUT /v2.0/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.240000000000002%" headers="mcps1.1.6.1.3 "><p id="p1575419512413"><a name="p1575419512413"></a><a name="p1575419512413"></a>vpc:subnets:update</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>×</p>
</td>
</tr>
<tr id="row177121437194112"><td class="cellrowborder" valign="top" width="11.98%" headers="mcps1.1.6.1.1 "><p id="p1253619313"><a name="p1253619313"></a><a name="p1253619313"></a>删除子网</p>
</td>
<td class="cellrowborder" valign="top" width="26.63%" headers="mcps1.1.6.1.2 "><p id="p6712133734118"><a name="p6712133734118"></a><a name="p6712133734118"></a>DELETE /v2.0/subnets/{subnet_id}</p>
</td>
<td class="cellrowborder" valign="top" width="21.240000000000002%" headers="mcps1.1.6.1.3 "><p id="p7221453164112"><a name="p7221453164112"></a><a name="p7221453164112"></a>vpc:subnets:delete</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.4 "><p id="p1267045134615"><a name="p1267045134615"></a><a name="p1267045134615"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.1.6.1.5 "><p id="p6670155114465"><a name="p6670155114465"></a><a name="p6670155114465"></a>×</p>
</td>
</tr>
</tbody>
</table>

