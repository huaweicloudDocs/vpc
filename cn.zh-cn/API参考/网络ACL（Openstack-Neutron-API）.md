# 网络ACL（Openstack Neutron API）<a name="ZH-CN_TOPIC_0201534132"></a>

<a name="table138590164616"></a>
<table><thead align="left"><tr id="row2054710012466"><th class="cellrowborder" valign="top" width="25.540000000000003%" id="mcps1.1.5.1.1"><p id="p1754710018467"><a name="p1754710018467"></a><a name="p1754710018467"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="19.32%" id="mcps1.1.5.1.2"><p id="p1489614416718"><a name="p1489614416718"></a><a name="p1489614416718"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="25.4%" id="mcps1.1.5.1.3"><p id="p135474024612"><a name="p135474024612"></a><a name="p135474024612"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="29.74%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row175475019467"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p55474044610"><a name="p55474044610"></a><a name="p55474044610"></a>GET /v2.0/fwaas/firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p38962449710"><a name="p38962449710"></a><a name="p38962449710"></a>查询所有网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p87832010154620"><a name="p87832010154620"></a><a name="p87832010154620"></a>vpc:firewallRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul66241846203119"></a><a name="ul66241846203119"></a><ul id="ul66241846203119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row954717015469"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p854711012462"><a name="p854711012462"></a><a name="p854711012462"></a>GET /v2.0/fwaas/firewall_rules/{firewall_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p68961644874"><a name="p68961644874"></a><a name="p68961644874"></a>查询特定网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p10249161204616"><a name="p10249161204616"></a><a name="p10249161204616"></a>vpc:firewallRules:get</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul95023481322"></a><a name="ul95023481322"></a><ul id="ul95023481322"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row754717018466"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p25471074610"><a name="p25471074610"></a><a name="p25471074610"></a>POST /v2.0/fwaas/firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p989619441578"><a name="p989619441578"></a><a name="p989619441578"></a>创建网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p1642771311465"><a name="p1642771311465"></a><a name="p1642771311465"></a>vpc:firewallRules:create</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul15513950173211"></a><a name="ul15513950173211"></a><ul id="ul15513950173211"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row25472014464"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p15471304466"><a name="p15471304466"></a><a name="p15471304466"></a>PUT /v2.0/fwaas/firewall_rules/{firewall_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p10896844676"><a name="p10896844676"></a><a name="p10896844676"></a>更新网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p10998714144611"><a name="p10998714144611"></a><a name="p10998714144611"></a>vpc:firewallRules:update</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul33641652103217"></a><a name="ul33641652103217"></a><ul id="ul33641652103217"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row2054713064610"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p7547302464"><a name="p7547302464"></a><a name="p7547302464"></a>DELETE /v2.0/fwaas/firewall_rules/{firewall_rule_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p128968441671"><a name="p128968441671"></a><a name="p128968441671"></a>删除网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p0230316104616"><a name="p0230316104616"></a><a name="p0230316104616"></a>vpc:firewallRules:delete</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul185134914469"></a><a name="ul185134914469"></a><ul id="ul185134914469"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row17547110134614"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p13547604464"><a name="p13547604464"></a><a name="p13547604464"></a>GET /v2.0/fwaas/firewall_policies</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p16896444478"><a name="p16896444478"></a><a name="p16896444478"></a>查询所有网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p1161211711468"><a name="p1161211711468"></a><a name="p1161211711468"></a>vpc:firewallPolicies:get</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul189124502514"></a><a name="ul189124502514"></a><ul id="ul189124502514"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1554717012462"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p1054790144617"><a name="p1054790144617"></a><a name="p1054790144617"></a>GET /v2.0/fwaas/firewall_policies/{firewall_policy_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p68961448715"><a name="p68961448715"></a><a name="p68961448715"></a>查询特定网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p1018319193467"><a name="p1018319193467"></a><a name="p1018319193467"></a>vpc:firewallPolicies:get</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul2823195245119"></a><a name="ul2823195245119"></a><ul id="ul2823195245119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row9547170204610"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p155471102460"><a name="p155471102460"></a><a name="p155471102460"></a>POST /v2.0/fwaas/firewall_policies</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p3896944179"><a name="p3896944179"></a><a name="p3896944179"></a>创建网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p1938032004613"><a name="p1938032004613"></a><a name="p1938032004613"></a>vpc:firewallPolicies:create</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul15445547518"></a><a name="ul15445547518"></a><ul id="ul15445547518"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row18547001460"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p1254713011460"><a name="p1254713011460"></a><a name="p1254713011460"></a>PUT /v2.0/fwaas/firewall_policies/{firewall_policy_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p889654416711"><a name="p889654416711"></a><a name="p889654416711"></a>更新网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p625182414611"><a name="p625182414611"></a><a name="p625182414611"></a>vpc:firewallPolicies:update</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul177471564517"></a><a name="ul177471564517"></a><ul id="ul177471564517"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row205476084614"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p1454710013464"><a name="p1454710013464"></a><a name="p1454710013464"></a>DELETE /v2.0/fwaas/firewall_policies/{firewall_policy_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p68974441376"><a name="p68974441376"></a><a name="p68974441376"></a>删除网络ACL策略</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p1761332616465"><a name="p1761332616465"></a><a name="p1761332616465"></a>vpc:firewallPolicies:delete</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul3559658195119"></a><a name="ul3559658195119"></a><ul id="ul3559658195119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row65472074610"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p185471074618"><a name="p185471074618"></a><a name="p185471074618"></a>PUT /v2.0/fwaas/firewall_policies/{firewall_policy_id}/insert_rule</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p689710445712"><a name="p689710445712"></a><a name="p689710445712"></a>插入网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><a name="ul194831710115410"></a><a name="ul194831710115410"></a><ul id="ul194831710115410"><li>vpc:firewallPolicies:addRule</li><li>vpc:firewallPolicies:get</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul1865510155214"></a><a name="ul1865510155214"></a><ul id="ul1865510155214"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row7547190114619"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p0547130134614"><a name="p0547130134614"></a><a name="p0547130134614"></a>PUT /v2.0/fwaas/firewall_policies/{firewall_policy_id}/remove_rule</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p168971144178"><a name="p168971144178"></a><a name="p168971144178"></a>移除网络ACL规则</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><a name="ul65475011468"></a><a name="ul65475011468"></a><ul id="ul65475011468"><li>vpc:firewallPolicies:removeRule</li><li>vpc:firewallPolicies:get</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul6731041521"></a><a name="ul6731041521"></a><ul id="ul6731041521"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1154718015467"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p115477044612"><a name="p115477044612"></a><a name="p115477044612"></a>GET /v2.0/fwaas/firewall_groups</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p188978441979"><a name="p188978441979"></a><a name="p188978441979"></a>查询所有网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p153991240174616"><a name="p153991240174616"></a><a name="p153991240174616"></a>vpc:firewallGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul299613595215"></a><a name="ul299613595215"></a><ul id="ul299613595215"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row165479014611"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p95471309469"><a name="p95471309469"></a><a name="p95471309469"></a>GET /v2.0/fwaas/firewall_groups/{firewall_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p10897164410715"><a name="p10897164410715"></a><a name="p10897164410715"></a>查询特定网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p5766194114618"><a name="p5766194114618"></a><a name="p5766194114618"></a>vpc:firewallGroups:get</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul980514710527"></a><a name="ul980514710527"></a><ul id="ul980514710527"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1154718013461"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p254914014462"><a name="p254914014462"></a><a name="p254914014462"></a>POST /v2.0/fwaas/firewall_groups</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p88971344977"><a name="p88971344977"></a><a name="p88971344977"></a>创建网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p17963425464"><a name="p17963425464"></a><a name="p17963425464"></a>vpc:firewallGroups:create</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul5553113165211"></a><a name="ul5553113165211"></a><ul id="ul5553113165211"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row11549307461"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p14549901464"><a name="p14549901464"></a><a name="p14549901464"></a>PUT /v2.0/fwaas/firewall_groups/{firewall_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p389774420716"><a name="p389774420716"></a><a name="p389774420716"></a>更新网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p1171664394618"><a name="p1171664394618"></a><a name="p1171664394618"></a>vpc:firewallGroups:update</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul185917157522"></a><a name="ul185917157522"></a><ul id="ul185917157522"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row15549309464"><td class="cellrowborder" valign="top" width="25.540000000000003%" headers="mcps1.1.5.1.1 "><p id="p1654911084613"><a name="p1654911084613"></a><a name="p1654911084613"></a>DELETE /v2.0/fwaas/firewall_groups/{firewall_group_id}</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.1.5.1.2 "><p id="p158974442715"><a name="p158974442715"></a><a name="p158974442715"></a>删除网络ACL组</p>
</td>
<td class="cellrowborder" valign="top" width="25.4%" headers="mcps1.1.5.1.3 "><p id="p182421245134619"><a name="p182421245134619"></a><a name="p182421245134619"></a>vpc:firewallGroups:delete</p>
</td>
<td class="cellrowborder" valign="top" width="29.74%" headers="mcps1.1.5.1.4 "><a name="ul11884181712523"></a><a name="ul11884181712523"></a><ul id="ul11884181712523"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
</tbody>
</table>

