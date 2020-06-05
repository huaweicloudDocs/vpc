# 安全组（Openstack Neutron API）<a name="vpc_permission_0016"></a>

<a name="table111868166448"></a>
<table><thead align="left"><tr id="row202761516194420"><th class="cellrowborder" valign="top" width="11.46%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="28.850000000000005%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="24.17%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="17.080000000000002%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="18.440000000000005%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row1327615166444"><td class="cellrowborder" valign="top" width="11.46%" headers="mcps1.1.6.1.1 "><p id="p121401137121311"><a name="p121401137121311"></a><a name="p121401137121311"></a>查询安全组</p>
</td>
<td class="cellrowborder" valign="top" width="28.850000000000005%" headers="mcps1.1.6.1.2 "><p id="p527614163445"><a name="p527614163445"></a><a name="p527614163445"></a>GET /v2.0/security-groups</p>
</td>
<td class="cellrowborder" valign="top" width="24.17%" headers="mcps1.1.6.1.3 "><p id="p98711213440"><a name="p98711213440"></a><a name="p98711213440"></a>vpc:securityGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.440000000000005%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row1276141614415"><td class="cellrowborder" valign="top" width="11.46%" headers="mcps1.1.6.1.1 "><p id="p31401537101319"><a name="p31401537101319"></a><a name="p31401537101319"></a>查询安全组详情</p>
</td>
<td class="cellrowborder" valign="top" width="28.850000000000005%" headers="mcps1.1.6.1.2 "><p id="p7277416144413"><a name="p7277416144413"></a><a name="p7277416144413"></a>GET /v2.0/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.17%" headers="mcps1.1.6.1.3 "><p id="p10403422194410"><a name="p10403422194410"></a><a name="p10403422194410"></a>vpc:securityGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.440000000000005%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row8277141624413"><td class="cellrowborder" valign="top" width="11.46%" headers="mcps1.1.6.1.1 "><p id="p1114023711130"><a name="p1114023711130"></a><a name="p1114023711130"></a>创建安全组</p>
</td>
<td class="cellrowborder" valign="top" width="28.850000000000005%" headers="mcps1.1.6.1.2 "><p id="p1827717168446"><a name="p1827717168446"></a><a name="p1827717168446"></a>POST /v2.0/security-groups</p>
</td>
<td class="cellrowborder" valign="top" width="24.17%" headers="mcps1.1.6.1.3 "><p id="p1849202313448"><a name="p1849202313448"></a><a name="p1849202313448"></a>vpc:securityGroups:create</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.440000000000005%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row6277111674416"><td class="cellrowborder" valign="top" width="11.46%" headers="mcps1.1.6.1.1 "><p id="p14140113791317"><a name="p14140113791317"></a><a name="p14140113791317"></a>更新安全组</p>
</td>
<td class="cellrowborder" valign="top" width="28.850000000000005%" headers="mcps1.1.6.1.2 "><p id="p3277616144414"><a name="p3277616144414"></a><a name="p3277616144414"></a>PUT /v2.0/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.17%" headers="mcps1.1.6.1.3 "><p id="p138071424124410"><a name="p138071424124410"></a><a name="p138071424124410"></a>vpc:securityGroups:update</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.440000000000005%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>×</p>
</td>
</tr>
<tr id="row13278116104413"><td class="cellrowborder" valign="top" width="11.46%" headers="mcps1.1.6.1.1 "><p id="p1141133731317"><a name="p1141133731317"></a><a name="p1141133731317"></a>删除安全组</p>
</td>
<td class="cellrowborder" valign="top" width="28.850000000000005%" headers="mcps1.1.6.1.2 "><p id="p1927814164440"><a name="p1927814164440"></a><a name="p1927814164440"></a>DELETE /v2.0/security-groups/{security_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.17%" headers="mcps1.1.6.1.3 "><p id="p893572614442"><a name="p893572614442"></a><a name="p893572614442"></a>vpc:securityGroups:delete</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.1.6.1.4 "><p id="p7890391778"><a name="p7890391778"></a><a name="p7890391778"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.440000000000005%" headers="mcps1.1.6.1.5 "><p id="p089193915720"><a name="p089193915720"></a><a name="p089193915720"></a>×</p>
</td>
</tr>
<tr id="row627815168444"><td class="cellrowborder" valign="top" width="11.46%" headers="mcps1.1.6.1.1 "><p id="p2014111373133"><a name="p2014111373133"></a><a name="p2014111373133"></a>查询安全组规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.850000000000005%" headers="mcps1.1.6.1.2 "><p id="p10278116124410"><a name="p10278116124410"></a><a name="p10278116124410"></a>GET /v2.0/security-group-rules</p>
</td>
<td class="cellrowborder" valign="top" width="24.17%" headers="mcps1.1.6.1.3 "><p id="p1358653024420"><a name="p1358653024420"></a><a name="p1358653024420"></a>vpc:securityGroupRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.1.6.1.4 "><p id="p208913917720"><a name="p208913917720"></a><a name="p208913917720"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.440000000000005%" headers="mcps1.1.6.1.5 "><p id="p189143911712"><a name="p189143911712"></a><a name="p189143911712"></a>×</p>
</td>
</tr>
<tr id="row13278171615443"><td class="cellrowborder" valign="top" width="11.46%" headers="mcps1.1.6.1.1 "><p id="p414183714131"><a name="p414183714131"></a><a name="p414183714131"></a>查询安全组规则详情</p>
</td>
<td class="cellrowborder" valign="top" width="28.850000000000005%" headers="mcps1.1.6.1.2 "><p id="p827816164443"><a name="p827816164443"></a><a name="p827816164443"></a>GET /v2.0/security-group-rules/{rules_security_groups_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.17%" headers="mcps1.1.6.1.3 "><p id="p134853214444"><a name="p134853214444"></a><a name="p134853214444"></a>vpc:securityGroupRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.1.6.1.4 "><p id="p9895391278"><a name="p9895391278"></a><a name="p9895391278"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.440000000000005%" headers="mcps1.1.6.1.5 "><p id="p15895391873"><a name="p15895391873"></a><a name="p15895391873"></a>×</p>
</td>
</tr>
<tr id="row1427916168445"><td class="cellrowborder" valign="top" width="11.46%" headers="mcps1.1.6.1.1 "><p id="p114120374136"><a name="p114120374136"></a><a name="p114120374136"></a>创建安全组规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.850000000000005%" headers="mcps1.1.6.1.2 "><p id="p1627917161448"><a name="p1627917161448"></a><a name="p1627917161448"></a>POST /v2.0/security-group-rules</p>
</td>
<td class="cellrowborder" valign="top" width="24.17%" headers="mcps1.1.6.1.3 "><p id="p327293419443"><a name="p327293419443"></a><a name="p327293419443"></a>vpc:securityGroupRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.1.6.1.4 "><p id="p128963917718"><a name="p128963917718"></a><a name="p128963917718"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.440000000000005%" headers="mcps1.1.6.1.5 "><p id="p15898395714"><a name="p15898395714"></a><a name="p15898395714"></a>×</p>
</td>
</tr>
<tr id="row1927921619447"><td class="cellrowborder" valign="top" width="11.46%" headers="mcps1.1.6.1.1 "><p id="p014143715135"><a name="p014143715135"></a><a name="p014143715135"></a>删除安全组规则</p>
</td>
<td class="cellrowborder" valign="top" width="28.850000000000005%" headers="mcps1.1.6.1.2 "><p id="p19279141614412"><a name="p19279141614412"></a><a name="p19279141614412"></a>DELETE /v2.0/security-group-rules/{rules_security_groups_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24.17%" headers="mcps1.1.6.1.3 "><p id="p18887113614448"><a name="p18887113614448"></a><a name="p18887113614448"></a>vpc:securityGroupRules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.1.6.1.4 "><p id="p0212644973"><a name="p0212644973"></a><a name="p0212644973"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="18.440000000000005%" headers="mcps1.1.6.1.5 "><p id="p821214415714"><a name="p821214415714"></a><a name="p821214415714"></a>×</p>
</td>
</tr>
</tbody>
</table>

