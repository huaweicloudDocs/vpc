# 弹性公网IP<a name="ZH-CN_TOPIC_0201534207"></a>

<a name="table3381441153612"></a>
<table><thead align="left"><tr id="row134361241153612"><th class="cellrowborder" valign="top" width="34%" id="mcps1.1.5.1.1"><p id="p24367414363"><a name="p24367414363"></a><a name="p24367414363"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.2"><p id="p423285813514"><a name="p423285813514"></a><a name="p423285813514"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p2436194193616"><a name="p2436194193616"></a><a name="p2436194193616"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="28.999999999999996%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row943674133617"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p144365416368"><a name="p144365416368"></a><a name="p144365416368"></a>POST /v1/{project_id}/publicips</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p13232958145117"><a name="p13232958145117"></a><a name="p13232958145117"></a>申请弹性公网IP</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p17904175011365"><a name="p17904175011365"></a><a name="p17904175011365"></a>vpc:publicIps:create</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><p id="p107185052510"><a name="p107185052510"></a><a name="p107185052510"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row343704173619"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p174371341133618"><a name="p174371341133618"></a><a name="p174371341133618"></a>GET /v1/{project_id}/publicips/{publicip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p1623218589512"><a name="p1623218589512"></a><a name="p1623218589512"></a>查询弹性公网IP</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p8360152113611"><a name="p8360152113611"></a><a name="p8360152113611"></a>vpc:publicIps:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><p id="p117181501259"><a name="p117181501259"></a><a name="p117181501259"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row34371241143616"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p16437174193619"><a name="p16437174193619"></a><a name="p16437174193619"></a>GET /v1/{project_id}/publicips</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p182321558155116"><a name="p182321558155116"></a><a name="p182321558155116"></a>查询弹性公网IP列表</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p35961753143612"><a name="p35961753143612"></a><a name="p35961753143612"></a>vpc:publicIps:list</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><p id="p1719903254"><a name="p1719903254"></a><a name="p1719903254"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row443713412363"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p4437194193614"><a name="p4437194193614"></a><a name="p4437194193614"></a>PUT /v1/{project_id}/publicips/{publicip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p623295805113"><a name="p623295805113"></a><a name="p623295805113"></a>更新弹性公网IP</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p1060705413366"><a name="p1060705413366"></a><a name="p1060705413366"></a>vpc:publicIps:update</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><p id="p4719701259"><a name="p4719701259"></a><a name="p4719701259"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row10437144143617"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p2437114115362"><a name="p2437114115362"></a><a name="p2437114115362"></a>DELETE /v1/{project_id}/publicips/{publicip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p923213587517"><a name="p923213587517"></a><a name="p923213587517"></a>删除弹性公网IP</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p986195516362"><a name="p986195516362"></a><a name="p986195516362"></a>vpc:publicIps:delete</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><p id="p324462512713"><a name="p324462512713"></a><a name="p324462512713"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row06971339262"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.1.5.1.1 "><p id="p17435812172618"><a name="p17435812172618"></a><a name="p17435812172618"></a>POST /v2.0/{project_id}/publicips</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p643581217266"><a name="p643581217266"></a><a name="p643581217266"></a>申请包周期弹性公网IP</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p343511262614"><a name="p343511262614"></a><a name="p343511262614"></a>vpc:publicIps:create</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><p id="p5485132562616"><a name="p5485132562616"></a><a name="p5485132562616"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
</tbody>
</table>

