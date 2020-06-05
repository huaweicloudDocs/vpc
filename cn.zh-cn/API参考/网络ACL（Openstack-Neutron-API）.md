# 网络ACL（Openstack Neutron API）<a name="vpc_permission_0015"></a>

<a name="table138590164616"></a>
<table><thead align="left"><tr id="row2054710012466"><th class="cellrowborder" valign="top" width="15.418458154184583%" id="mcps1.1.6.1.1"><p id="p6174435204812"><a name="p6174435204812"></a><a name="p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="25.787421257874215%" id="mcps1.1.6.1.2"><p id="p8174113504816"><a name="p8174113504816"></a><a name="p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="26.757324267573246%" id="mcps1.1.6.1.3"><p id="p8701346133717"><a name="p8701346133717"></a><a name="p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="16.14838516148385%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="15.888411158884114%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row175475019467"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p38962449710"><a name="p38962449710"></a><a name="p38962449710"></a>查询所有网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p55474044610"><a name="p55474044610"></a><a name="p55474044610"></a>GET /v2.0/fwaas/firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p87832010154620"><a name="p87832010154620"></a><a name="p87832010154620"></a>vpc:firewallRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row954717015469"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p68961644874"><a name="p68961644874"></a><a name="p68961644874"></a>查询特定网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p854711012462"><a name="p854711012462"></a><a name="p854711012462"></a>GET /v2.0/fwaas/firewall_rules/{firewall_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p10249161204616"><a name="p10249161204616"></a><a name="p10249161204616"></a>vpc:firewallRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row754717018466"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p989619441578"><a name="p989619441578"></a><a name="p989619441578"></a>创建网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p25471074610"><a name="p25471074610"></a><a name="p25471074610"></a>POST /v2.0/fwaas/firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p1642771311465"><a name="p1642771311465"></a><a name="p1642771311465"></a>vpc:firewallRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row25472014464"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p10896844676"><a name="p10896844676"></a><a name="p10896844676"></a>更新网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p15471304466"><a name="p15471304466"></a><a name="p15471304466"></a>PUT /v2.0/fwaas/firewall_rules/{firewall_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p10998714144611"><a name="p10998714144611"></a><a name="p10998714144611"></a>vpc:firewallRules:update</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>×</p>
</td>
</tr>
<tr id="row2054713064610"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p128968441671"><a name="p128968441671"></a><a name="p128968441671"></a>删除网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p7547302464"><a name="p7547302464"></a><a name="p7547302464"></a>DELETE /v2.0/fwaas/firewall_rules/{firewall_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p0230316104616"><a name="p0230316104616"></a><a name="p0230316104616"></a>vpc:firewallRules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p1267045134615"><a name="p1267045134615"></a><a name="p1267045134615"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p6670155114465"><a name="p6670155114465"></a><a name="p6670155114465"></a>×</p>
</td>
</tr>
<tr id="row17547110134614"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p16896444478"><a name="p16896444478"></a><a name="p16896444478"></a>查询所有网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p13547604464"><a name="p13547604464"></a><a name="p13547604464"></a>GET /v2.0/fwaas/firewall_policies</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p1161211711468"><a name="p1161211711468"></a><a name="p1161211711468"></a>vpc:firewallPolicies:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p5670165120466"><a name="p5670165120466"></a><a name="p5670165120466"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p167055174612"><a name="p167055174612"></a><a name="p167055174612"></a>×</p>
</td>
</tr>
<tr id="row1554717012462"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p68961448715"><a name="p68961448715"></a><a name="p68961448715"></a>查询特定网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p1054790144617"><a name="p1054790144617"></a><a name="p1054790144617"></a>GET /v2.0/fwaas/firewall_policies/{firewall_policy_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p1018319193467"><a name="p1018319193467"></a><a name="p1018319193467"></a>vpc:firewallPolicies:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p9520861666"><a name="p9520861666"></a><a name="p9520861666"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p10520361611"><a name="p10520361611"></a><a name="p10520361611"></a>×</p>
</td>
</tr>
<tr id="row9547170204610"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p3896944179"><a name="p3896944179"></a><a name="p3896944179"></a>创建网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p155471102460"><a name="p155471102460"></a><a name="p155471102460"></a>POST /v2.0/fwaas/firewall_policies</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p1938032004613"><a name="p1938032004613"></a><a name="p1938032004613"></a>vpc:firewallPolicies:create</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p135201961968"><a name="p135201961968"></a><a name="p135201961968"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p17520461168"><a name="p17520461168"></a><a name="p17520461168"></a>×</p>
</td>
</tr>
<tr id="row18547001460"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p889654416711"><a name="p889654416711"></a><a name="p889654416711"></a>更新网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p1254713011460"><a name="p1254713011460"></a><a name="p1254713011460"></a>PUT /v2.0/fwaas/firewall_policies/{firewall_policy_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p625182414611"><a name="p625182414611"></a><a name="p625182414611"></a>vpc:firewallPolicies:update</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p252036665"><a name="p252036665"></a><a name="p252036665"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p1520106464"><a name="p1520106464"></a><a name="p1520106464"></a>×</p>
</td>
</tr>
<tr id="row205476084614"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p68974441376"><a name="p68974441376"></a><a name="p68974441376"></a>删除网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p1454710013464"><a name="p1454710013464"></a><a name="p1454710013464"></a>DELETE /v2.0/fwaas/firewall_policies/{firewall_policy_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p1761332616465"><a name="p1761332616465"></a><a name="p1761332616465"></a>vpc:firewallPolicies:delete</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p135218615612"><a name="p135218615612"></a><a name="p135218615612"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p752146463"><a name="p752146463"></a><a name="p752146463"></a>×</p>
</td>
</tr>
<tr id="row65472074610"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p689710445712"><a name="p689710445712"></a><a name="p689710445712"></a>插入网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p185471074618"><a name="p185471074618"></a><a name="p185471074618"></a>PUT /v2.0/fwaas/firewall_policies/{firewall_policy_id}/insert_rule</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><a name="ul194831710115410"></a><a name="ul194831710115410"></a><ul id="ul194831710115410"><li>vpc:firewallPolicies:addRule</li><li>vpc:firewallPolicies:get</li></ul>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p115245914612"><a name="p115245914612"></a><a name="p115245914612"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p11524169768"><a name="p11524169768"></a><a name="p11524169768"></a>×</p>
</td>
</tr>
<tr id="row7547190114619"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p168971144178"><a name="p168971144178"></a><a name="p168971144178"></a>移除网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p0547130134614"><a name="p0547130134614"></a><a name="p0547130134614"></a>PUT /v2.0/fwaas/firewall_policies/{firewall_policy_id}/remove_rule</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><a name="ul65475011468"></a><a name="ul65475011468"></a><ul id="ul65475011468"><li>vpc:firewallPolicies:removeRule</li><li>vpc:firewallPolicies:get</li></ul>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p185241699610"><a name="p185241699610"></a><a name="p185241699610"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p25241993610"><a name="p25241993610"></a><a name="p25241993610"></a>×</p>
</td>
</tr>
<tr id="row1154718015467"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p188978441979"><a name="p188978441979"></a><a name="p188978441979"></a>查询所有网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p115477044612"><a name="p115477044612"></a><a name="p115477044612"></a>GET /v2.0/fwaas/firewall_groups</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p153991240174616"><a name="p153991240174616"></a><a name="p153991240174616"></a>vpc:firewallGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p652411911620"><a name="p652411911620"></a><a name="p652411911620"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p6524191861"><a name="p6524191861"></a><a name="p6524191861"></a>×</p>
</td>
</tr>
<tr id="row165479014611"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p10897164410715"><a name="p10897164410715"></a><a name="p10897164410715"></a>查询特定网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p95471309469"><a name="p95471309469"></a><a name="p95471309469"></a>GET /v2.0/fwaas/firewall_groups/{firewall_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p5766194114618"><a name="p5766194114618"></a><a name="p5766194114618"></a>vpc:firewallGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p1152489668"><a name="p1152489668"></a><a name="p1152489668"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p135241591365"><a name="p135241591365"></a><a name="p135241591365"></a>×</p>
</td>
</tr>
<tr id="row1154718013461"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p88971344977"><a name="p88971344977"></a><a name="p88971344977"></a>创建网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p254914014462"><a name="p254914014462"></a><a name="p254914014462"></a>POST /v2.0/fwaas/firewall_groups</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p17963425464"><a name="p17963425464"></a><a name="p17963425464"></a>vpc:firewallGroups:create</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p106191011264"><a name="p106191011264"></a><a name="p106191011264"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p18619711162"><a name="p18619711162"></a><a name="p18619711162"></a>×</p>
</td>
</tr>
<tr id="row11549307461"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p389774420716"><a name="p389774420716"></a><a name="p389774420716"></a>更新网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p14549901464"><a name="p14549901464"></a><a name="p14549901464"></a>PUT /v2.0/fwaas/firewall_groups/{firewall_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p1171664394618"><a name="p1171664394618"></a><a name="p1171664394618"></a>vpc:firewallGroups:update</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p1619101119612"><a name="p1619101119612"></a><a name="p1619101119612"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p166197114615"><a name="p166197114615"></a><a name="p166197114615"></a>×</p>
</td>
</tr>
<tr id="row15549309464"><td class="cellrowborder" valign="top" width="15.418458154184583%" headers="mcps1.1.6.1.1 "><p id="p158974442715"><a name="p158974442715"></a><a name="p158974442715"></a>删除网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.787421257874215%" headers="mcps1.1.6.1.2 "><p id="p1654911084613"><a name="p1654911084613"></a><a name="p1654911084613"></a>DELETE /v2.0/fwaas/firewall_groups/{firewall_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="26.757324267573246%" headers="mcps1.1.6.1.3 "><p id="p182421245134619"><a name="p182421245134619"></a><a name="p182421245134619"></a>vpc:firewallGroups:delete</p>
</td>
<td class="cellrowborder" valign="top" width="16.14838516148385%" headers="mcps1.1.6.1.4 "><p id="p3619811765"><a name="p3619811765"></a><a name="p3619811765"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.888411158884114%" headers="mcps1.1.6.1.5 "><p id="p136195112612"><a name="p136195112612"></a><a name="p136195112612"></a>×</p>
</td>
</tr>
</tbody>
</table>

