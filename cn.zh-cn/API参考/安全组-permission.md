# 安全组<a name="vpc_permission_0008"></a>

<a name="table127217439395"></a>
<table><thead align="left"><tr id="row3757114311393"><th class="cellrowborder" valign="top" width="36%" id="mcps1.1.5.1.1"><p id="p16757164323917"><a name="p16757164323917"></a><a name="p16757164323917"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.1.5.1.2"><p id="p612618713010"><a name="p612618713010"></a><a name="p612618713010"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.3"><p id="p575717435398"><a name="p575717435398"></a><a name="p575717435398"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="33%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row475754333912"><td class="cellrowborder" valign="top" width="36%" headers="mcps1.1.5.1.1 "><p id="p12757143203913"><a name="p12757143203913"></a><a name="p12757143203913"></a>POST /v1/{project_id}/security-groups</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p61261475013"><a name="p61261475013"></a><a name="p61261475013"></a>创建安全组</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p1391450143917"><a name="p1391450143917"></a><a name="p1391450143917"></a>vpc:securityGroups:create</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.1.5.1.4 "><p id="p107185052510"><a name="p107185052510"></a><a name="p107185052510"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row14757144317398"><td class="cellrowborder" valign="top" width="36%" headers="mcps1.1.5.1.1 "><p id="p19757243113915"><a name="p19757243113915"></a><a name="p19757243113915"></a>GET /v1/{project_id}/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p1212614710015"><a name="p1212614710015"></a><a name="p1212614710015"></a>查询安全组</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p108251851153916"><a name="p108251851153916"></a><a name="p108251851153916"></a>vpc:securityGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.1.5.1.4 "><p id="p117181501259"><a name="p117181501259"></a><a name="p117181501259"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row1975744313399"><td class="cellrowborder" valign="top" width="36%" headers="mcps1.1.5.1.1 "><p id="p3757134393913"><a name="p3757134393913"></a><a name="p3757134393913"></a>GET /v1/{project_id}/security-groups</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p111266710018"><a name="p111266710018"></a><a name="p111266710018"></a>查询安全组列表</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p125905318398"><a name="p125905318398"></a><a name="p125905318398"></a>vpc:securityGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.1.5.1.4 "><p id="p1719903254"><a name="p1719903254"></a><a name="p1719903254"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row192911722404"><td class="cellrowborder" valign="top" width="36%" headers="mcps1.1.5.1.1 "><p id="p61961146134010"><a name="p61961146134010"></a><a name="p61961146134010"></a>DELETE /v1/{project_id}/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.1.5.1.2 "><p id="p71966469403"><a name="p71966469403"></a><a name="p71966469403"></a>删除安全组</p>
</td>
<td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.3 "><p id="p15196104617401"><a name="p15196104617401"></a><a name="p15196104617401"></a>vpc:securityGroups:delete</p>
</td>
<td class="cellrowborder" valign="top" width="33%" headers="mcps1.1.5.1.4 "><p id="p13598052174017"><a name="p13598052174017"></a><a name="p13598052174017"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
</tbody>
</table>

