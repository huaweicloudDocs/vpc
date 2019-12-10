# 安全组（Openstack Neutron API）<a name="vpc_permission_0016"></a>

<a name="table111868166448"></a>
<table><thead align="left"><tr id="row202761516194420"><th class="cellrowborder" valign="top" width="27.08%" id="mcps1.1.5.1.1"><p id="p11276201616440"><a name="p11276201616440"></a><a name="p11276201616440"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="16.38%" id="mcps1.1.5.1.2"><p id="p1014003731317"><a name="p1014003731317"></a><a name="p1014003731317"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="23.119999999999997%" id="mcps1.1.5.1.3"><p id="p6276816124418"><a name="p6276816124418"></a><a name="p6276816124418"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="33.42%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row1327615166444"><td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.1.5.1.1 "><p id="p527614163445"><a name="p527614163445"></a><a name="p527614163445"></a>GET /v2.0/security-groups</p>
</td>
<td class="cellrowborder" valign="top" width="16.38%" headers="mcps1.1.5.1.2 "><p id="p121401137121311"><a name="p121401137121311"></a><a name="p121401137121311"></a>查询安全组</p>
</td>
<td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.5.1.3 "><p id="p98711213440"><a name="p98711213440"></a><a name="p98711213440"></a>vpc:securityGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="33.42%" headers="mcps1.1.5.1.4 "><a name="ul66241846203119"></a><a name="ul66241846203119"></a><ul id="ul66241846203119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1276141614415"><td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.1.5.1.1 "><p id="p7277416144413"><a name="p7277416144413"></a><a name="p7277416144413"></a>GET /v2.0/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16.38%" headers="mcps1.1.5.1.2 "><p id="p31401537101319"><a name="p31401537101319"></a><a name="p31401537101319"></a>查询安全组详情</p>
</td>
<td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.5.1.3 "><p id="p10403422194410"><a name="p10403422194410"></a><a name="p10403422194410"></a>vpc:securityGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="33.42%" headers="mcps1.1.5.1.4 "><a name="ul95023481322"></a><a name="ul95023481322"></a><ul id="ul95023481322"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row8277141624413"><td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.1.5.1.1 "><p id="p1827717168446"><a name="p1827717168446"></a><a name="p1827717168446"></a>POST /v2.0/security-groups</p>
</td>
<td class="cellrowborder" valign="top" width="16.38%" headers="mcps1.1.5.1.2 "><p id="p1114023711130"><a name="p1114023711130"></a><a name="p1114023711130"></a>创建安全组</p>
</td>
<td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.5.1.3 "><p id="p1849202313448"><a name="p1849202313448"></a><a name="p1849202313448"></a>vpc:securityGroups:create</p>
</td>
<td class="cellrowborder" valign="top" width="33.42%" headers="mcps1.1.5.1.4 "><a name="ul15513950173211"></a><a name="ul15513950173211"></a><ul id="ul15513950173211"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row6277111674416"><td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.1.5.1.1 "><p id="p3277616144414"><a name="p3277616144414"></a><a name="p3277616144414"></a>PUT /v2.0/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16.38%" headers="mcps1.1.5.1.2 "><p id="p14140113791317"><a name="p14140113791317"></a><a name="p14140113791317"></a>更新安全组</p>
</td>
<td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.5.1.3 "><p id="p138071424124410"><a name="p138071424124410"></a><a name="p138071424124410"></a>vpc:securityGroups:update</p>
</td>
<td class="cellrowborder" valign="top" width="33.42%" headers="mcps1.1.5.1.4 "><a name="ul33641652103217"></a><a name="ul33641652103217"></a><ul id="ul33641652103217"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row13278116104413"><td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.1.5.1.1 "><p id="p1927814164440"><a name="p1927814164440"></a><a name="p1927814164440"></a>DELETE /v2.0/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16.38%" headers="mcps1.1.5.1.2 "><p id="p1141133731317"><a name="p1141133731317"></a><a name="p1141133731317"></a>删除安全组</p>
</td>
<td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.5.1.3 "><p id="p893572614442"><a name="p893572614442"></a><a name="p893572614442"></a>vpc:securityGroups:delete</p>
</td>
<td class="cellrowborder" valign="top" width="33.42%" headers="mcps1.1.5.1.4 "><a name="ul185134914469"></a><a name="ul185134914469"></a><ul id="ul185134914469"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row627815168444"><td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.1.5.1.1 "><p id="p10278116124410"><a name="p10278116124410"></a><a name="p10278116124410"></a>GET /v2.0/security-group-rules</p>
</td>
<td class="cellrowborder" valign="top" width="16.38%" headers="mcps1.1.5.1.2 "><p id="p2014111373133"><a name="p2014111373133"></a><a name="p2014111373133"></a>查询安全组规则</p>
</td>
<td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.5.1.3 "><p id="p1358653024420"><a name="p1358653024420"></a><a name="p1358653024420"></a>vpc:securityGroupRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="33.42%" headers="mcps1.1.5.1.4 "><a name="ul01111305536"></a><a name="ul01111305536"></a><ul id="ul01111305536"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row13278171615443"><td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.1.5.1.1 "><p id="p827816164443"><a name="p827816164443"></a><a name="p827816164443"></a>GET /v2.0/security-group-rules/{rules_security_groups_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16.38%" headers="mcps1.1.5.1.2 "><p id="p414183714131"><a name="p414183714131"></a><a name="p414183714131"></a>查询安全组规则详情</p>
</td>
<td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.5.1.3 "><p id="p134853214444"><a name="p134853214444"></a><a name="p134853214444"></a>vpc:securityGroupRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="33.42%" headers="mcps1.1.5.1.4 "><a name="ul1175723117533"></a><a name="ul1175723117533"></a><ul id="ul1175723117533"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1427916168445"><td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.1.5.1.1 "><p id="p1627917161448"><a name="p1627917161448"></a><a name="p1627917161448"></a>POST /v2.0/security-group-rules</p>
</td>
<td class="cellrowborder" valign="top" width="16.38%" headers="mcps1.1.5.1.2 "><p id="p114120374136"><a name="p114120374136"></a><a name="p114120374136"></a>创建安全组规则</p>
</td>
<td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.5.1.3 "><p id="p327293419443"><a name="p327293419443"></a><a name="p327293419443"></a>vpc:securityGroupRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="33.42%" headers="mcps1.1.5.1.4 "><a name="ul373493335316"></a><a name="ul373493335316"></a><ul id="ul373493335316"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1927921619447"><td class="cellrowborder" valign="top" width="27.08%" headers="mcps1.1.5.1.1 "><p id="p19279141614412"><a name="p19279141614412"></a><a name="p19279141614412"></a>DELETE /v2.0/security-group-rules/{rules_security_groups_id}</p>
</td>
<td class="cellrowborder" valign="top" width="16.38%" headers="mcps1.1.5.1.2 "><p id="p014143715135"><a name="p014143715135"></a><a name="p014143715135"></a>删除安全组规则</p>
</td>
<td class="cellrowborder" valign="top" width="23.119999999999997%" headers="mcps1.1.5.1.3 "><p id="p18887113614448"><a name="p18887113614448"></a><a name="p18887113614448"></a>vpc:securityGroupRules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="33.42%" headers="mcps1.1.5.1.4 "><a name="ul553512350533"></a><a name="ul553512350533"></a><ul id="ul553512350533"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
</tbody>
</table>

