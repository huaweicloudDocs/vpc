# 安全组<a name="vpc_permission_0008"></a>

<a name="table127217439395"></a>
<table><thead align="left"><tr id="row3757114311393"><th class="cellrowborder" valign="top" width="15.738426157384264%" id="mcps1.1.6.1.1"><p id="p1446941614480"><a name="p1446941614480"></a><a name="p1446941614480"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="20.897910208979102%" id="mcps1.1.6.1.2"><p id="p6469816154818"><a name="p6469816154818"></a><a name="p6469816154818"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="24.717528247175284%" id="mcps1.1.6.1.3"><p id="p575717435398"><a name="p575717435398"></a><a name="p575717435398"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="19.018098190180982%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="19.628037196280374%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row475754333912"><td class="cellrowborder" valign="top" width="15.738426157384264%" headers="mcps1.1.6.1.1 "><p id="p61261475013"><a name="p61261475013"></a><a name="p61261475013"></a>创建安全组</p>
</td>
<td class="cellrowborder" valign="top" width="20.897910208979102%" headers="mcps1.1.6.1.2 "><p id="p12757143203913"><a name="p12757143203913"></a><a name="p12757143203913"></a>POST /v1/{project_id}/security-groups</p>
</td>
<td class="cellrowborder" valign="top" width="24.717528247175284%" headers="mcps1.1.6.1.3 "><p id="p1391450143917"><a name="p1391450143917"></a><a name="p1391450143917"></a>vpc:securityGroups:create</p>
</td>
<td class="cellrowborder" valign="top" width="19.018098190180982%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="19.628037196280374%" headers="mcps1.1.6.1.5 "><p id="p193691154133112"><a name="p193691154133112"></a><a name="p193691154133112"></a>√</p>
</td>
</tr>
<tr id="row14757144317398"><td class="cellrowborder" valign="top" width="15.738426157384264%" headers="mcps1.1.6.1.1 "><p id="p1212614710015"><a name="p1212614710015"></a><a name="p1212614710015"></a>查询安全组</p>
</td>
<td class="cellrowborder" valign="top" width="20.897910208979102%" headers="mcps1.1.6.1.2 "><p id="p19757243113915"><a name="p19757243113915"></a><a name="p19757243113915"></a>GET /v1/{project_id}/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.717528247175284%" headers="mcps1.1.6.1.3 "><p id="p108251851153916"><a name="p108251851153916"></a><a name="p108251851153916"></a>vpc:securityGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.018098190180982%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="19.628037196280374%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>√</p>
</td>
</tr>
<tr id="row1975744313399"><td class="cellrowborder" valign="top" width="15.738426157384264%" headers="mcps1.1.6.1.1 "><p id="p111266710018"><a name="p111266710018"></a><a name="p111266710018"></a>查询安全组列表</p>
</td>
<td class="cellrowborder" valign="top" width="20.897910208979102%" headers="mcps1.1.6.1.2 "><p id="p3757134393913"><a name="p3757134393913"></a><a name="p3757134393913"></a>GET /v1/{project_id}/security-groups</p>
</td>
<td class="cellrowborder" valign="top" width="24.717528247175284%" headers="mcps1.1.6.1.3 "><p id="p125905318398"><a name="p125905318398"></a><a name="p125905318398"></a>vpc:securityGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="19.018098190180982%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="19.628037196280374%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>√</p>
</td>
</tr>
<tr id="row192911722404"><td class="cellrowborder" valign="top" width="15.738426157384264%" headers="mcps1.1.6.1.1 "><p id="p71966469403"><a name="p71966469403"></a><a name="p71966469403"></a>删除安全组</p>
</td>
<td class="cellrowborder" valign="top" width="20.897910208979102%" headers="mcps1.1.6.1.2 "><p id="p61961146134010"><a name="p61961146134010"></a><a name="p61961146134010"></a>DELETE /v1/{project_id}/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.717528247175284%" headers="mcps1.1.6.1.3 "><p id="p15196104617401"><a name="p15196104617401"></a><a name="p15196104617401"></a>vpc:securityGroups:delete</p>
</td>
<td class="cellrowborder" valign="top" width="19.018098190180982%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="19.628037196280374%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>√</p>
</td>
</tr>
</tbody>
</table>

