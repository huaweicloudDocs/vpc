# 对等连接<a name="vpc_permission_0005"></a>

<a name="table967413133817"></a>
<table><thead align="left"><tr id="row9708231163820"><th class="cellrowborder" valign="top" width="12.25%" id="mcps1.1.6.1.1"><p id="p3808155143811"><a name="p3808155143811"></a><a name="p3808155143811"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="31.669999999999998%" id="mcps1.1.6.1.2"><p id="p158081855113816"><a name="p158081855113816"></a><a name="p158081855113816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="23.27%" id="mcps1.1.6.1.3"><p id="p580815563812"><a name="p580815563812"></a><a name="p580815563812"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="15.329999999999998%" id="mcps1.1.6.1.4"><p id="p5985736163016"><a name="p5985736163016"></a><a name="p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="17.48%" id="mcps1.1.6.1.5"><p id="p8985133619300"><a name="p8985133619300"></a><a name="p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="row197081331113817"><td class="cellrowborder" valign="top" width="12.25%" headers="mcps1.1.6.1.1 "><p id="p7482131816133"><a name="p7482131816133"></a><a name="p7482131816133"></a>查询对等连接列表</p>
</td>
<td class="cellrowborder" valign="top" width="31.669999999999998%" headers="mcps1.1.6.1.2 "><p id="p143974820139"><a name="p143974820139"></a><a name="p143974820139"></a>GET /v2.0/vpc/peerings</p>
</td>
<td class="cellrowborder" valign="top" width="23.27%" headers="mcps1.1.6.1.3 "><p id="p13892440173820"><a name="p13892440173820"></a><a name="p13892440173820"></a>vpc:peerings:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.329999999999998%" headers="mcps1.1.6.1.4 "><p id="p15756115919276"><a name="p15756115919276"></a><a name="p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.1.6.1.5 "><p id="p54871102411"><a name="p54871102411"></a><a name="p54871102411"></a>×</p>
</td>
</tr>
<tr id="row15709203163811"><td class="cellrowborder" valign="top" width="12.25%" headers="mcps1.1.6.1.1 "><p id="p1549015468132"><a name="p1549015468132"></a><a name="p1549015468132"></a>查询对等连接</p>
</td>
<td class="cellrowborder" valign="top" width="31.669999999999998%" headers="mcps1.1.6.1.2 "><p id="p17649343101319"><a name="p17649343101319"></a><a name="p17649343101319"></a>GET /v2.0/vpc/peerings/{peering_id}</p>
</td>
<td class="cellrowborder" valign="top" width="23.27%" headers="mcps1.1.6.1.3 "><p id="p1940834512014"><a name="p1940834512014"></a><a name="p1940834512014"></a>vpc:peerings:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.329999999999998%" headers="mcps1.1.6.1.4 "><p id="p1475655902719"><a name="p1475655902719"></a><a name="p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.1.6.1.5 "><p id="p153706545313"><a name="p153706545313"></a><a name="p153706545313"></a>×</p>
</td>
</tr>
<tr id="row1670914317388"><td class="cellrowborder" valign="top" width="12.25%" headers="mcps1.1.6.1.1 "><p id="p8638811165911"><a name="p8638811165911"></a><a name="p8638811165911"></a>创建对等连接</p>
</td>
<td class="cellrowborder" valign="top" width="31.669999999999998%" headers="mcps1.1.6.1.2 "><p id="p181448651411"><a name="p181448651411"></a><a name="p181448651411"></a>POST /v2.0/vpc/peerings</p>
</td>
<td class="cellrowborder" valign="top" width="23.27%" headers="mcps1.1.6.1.3 "><p id="p1724712431387"><a name="p1724712431387"></a><a name="p1724712431387"></a>vpc:peerings:create</p>
</td>
<td class="cellrowborder" valign="top" width="15.329999999999998%" headers="mcps1.1.6.1.4 "><p id="p167561459142711"><a name="p167561459142711"></a><a name="p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.1.6.1.5 "><p id="p1370175418319"><a name="p1370175418319"></a><a name="p1370175418319"></a>×</p>
</td>
</tr>
<tr id="row6709163118385"><td class="cellrowborder" valign="top" width="12.25%" headers="mcps1.1.6.1.1 "><p id="p135991634111413"><a name="p135991634111413"></a><a name="p135991634111413"></a>接受对等连接请求</p>
</td>
<td class="cellrowborder" valign="top" width="31.669999999999998%" headers="mcps1.1.6.1.2 "><p id="p206275422143"><a name="p206275422143"></a><a name="p206275422143"></a>PUT /v2.0/vpc/peerings/{peering_id}/accept</p>
</td>
<td class="cellrowborder" valign="top" width="23.27%" headers="mcps1.1.6.1.3 "><p id="p383524711173"><a name="p383524711173"></a><a name="p383524711173"></a>vpc:peerings:accept</p>
</td>
<td class="cellrowborder" valign="top" width="15.329999999999998%" headers="mcps1.1.6.1.4 "><p id="p9757145912271"><a name="p9757145912271"></a><a name="p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.1.6.1.5 "><p id="p19370155411318"><a name="p19370155411318"></a><a name="p19370155411318"></a>×</p>
</td>
</tr>
<tr id="row1821415719143"><td class="cellrowborder" valign="top" width="12.25%" headers="mcps1.1.6.1.1 "><p id="p1921455713144"><a name="p1921455713144"></a><a name="p1921455713144"></a>拒绝对等连接请求</p>
</td>
<td class="cellrowborder" valign="top" width="31.669999999999998%" headers="mcps1.1.6.1.2 "><p id="p11214957111419"><a name="p11214957111419"></a><a name="p11214957111419"></a>PUT /v2.0/vpc/peerings/{peering_id}/reject</p>
</td>
<td class="cellrowborder" valign="top" width="23.27%" headers="mcps1.1.6.1.3 "><p id="p02142057171419"><a name="p02142057171419"></a><a name="p02142057171419"></a>vpc:peerings:reject</p>
</td>
<td class="cellrowborder" valign="top" width="15.329999999999998%" headers="mcps1.1.6.1.4 "><p id="p187577594276"><a name="p187577594276"></a><a name="p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.1.6.1.5 "><p id="p10370105493116"><a name="p10370105493116"></a><a name="p10370105493116"></a>×</p>
</td>
</tr>
<tr id="row134257015151"><td class="cellrowborder" valign="top" width="12.25%" headers="mcps1.1.6.1.1 "><p id="p74251013151"><a name="p74251013151"></a><a name="p74251013151"></a>更新对等连接</p>
</td>
<td class="cellrowborder" valign="top" width="31.669999999999998%" headers="mcps1.1.6.1.2 "><p id="p13307113415152"><a name="p13307113415152"></a><a name="p13307113415152"></a>PUT /v2.0/vpc/peerings/{peering_id}</p>
</td>
<td class="cellrowborder" valign="top" width="23.27%" headers="mcps1.1.6.1.3 "><p id="p2720085191"><a name="p2720085191"></a><a name="p2720085191"></a>vpc:peerings:update</p>
</td>
<td class="cellrowborder" valign="top" width="15.329999999999998%" headers="mcps1.1.6.1.4 "><p id="p427183920454"><a name="p427183920454"></a><a name="p427183920454"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.1.6.1.5 "><p id="p1010941313249"><a name="p1010941313249"></a><a name="p1010941313249"></a>×</p>
</td>
</tr>
<tr id="row629817252151"><td class="cellrowborder" valign="top" width="12.25%" headers="mcps1.1.6.1.1 "><p id="p1129816255153"><a name="p1129816255153"></a><a name="p1129816255153"></a>删除对等连接</p>
</td>
<td class="cellrowborder" valign="top" width="31.669999999999998%" headers="mcps1.1.6.1.2 "><p id="p1629862511519"><a name="p1629862511519"></a><a name="p1629862511519"></a>DELETE /v2.0/vpc/peerings/{peering_id}</p>
</td>
<td class="cellrowborder" valign="top" width="23.27%" headers="mcps1.1.6.1.3 "><p id="p1381162919184"><a name="p1381162919184"></a><a name="p1381162919184"></a>vpc:peerings:delete</p>
</td>
<td class="cellrowborder" valign="top" width="15.329999999999998%" headers="mcps1.1.6.1.4 "><p id="p1727839174518"><a name="p1727839174518"></a><a name="p1727839174518"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.1.6.1.5 "><p id="p12273391459"><a name="p12273391459"></a><a name="p12273391459"></a>×</p>
</td>
</tr>
</tbody>
</table>

