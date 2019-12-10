# 对等连接<a name="vpc_permission_0005"></a>

<a name="table967413133817"></a>
<table><thead align="left"><tr id="row9708231163820"><th class="cellrowborder" valign="top" width="37%" id="mcps1.1.5.1.1"><p id="p1970823143813"><a name="p1970823143813"></a><a name="p1970823143813"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.2"><p id="p12638211185918"><a name="p12638211185918"></a><a name="p12638211185918"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p137081931143810"><a name="p137081931143810"></a><a name="p137081931143810"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="26%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row197081331113817"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p143974820139"><a name="p143974820139"></a><a name="p143974820139"></a>GET /v2.0/vpc/peerings</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p7482131816133"><a name="p7482131816133"></a><a name="p7482131816133"></a>查询对等连接列表</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p13892440173820"><a name="p13892440173820"></a><a name="p13892440173820"></a>vpc:peerings:get</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul66241846203119"></a><a name="ul66241846203119"></a><ul id="ul66241846203119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row15709203163811"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p17649343101319"><a name="p17649343101319"></a><a name="p17649343101319"></a>GET /v2.0/vpc/peerings/{peering_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p1549015468132"><a name="p1549015468132"></a><a name="p1549015468132"></a>查询对等连接</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p1940834512014"><a name="p1940834512014"></a><a name="p1940834512014"></a>vpc:peerings:get</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul95023481322"></a><a name="ul95023481322"></a><ul id="ul95023481322"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1670914317388"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p181448651411"><a name="p181448651411"></a><a name="p181448651411"></a>POST /v2.0/vpc/peerings</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p8638811165911"><a name="p8638811165911"></a><a name="p8638811165911"></a>创建对等连接</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p1724712431387"><a name="p1724712431387"></a><a name="p1724712431387"></a>vpc:peerings:create</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul15513950173211"></a><a name="ul15513950173211"></a><ul id="ul15513950173211"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row6709163118385"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p206275422143"><a name="p206275422143"></a><a name="p206275422143"></a>PUT /v2.0/vpc/peerings/{peering_id}/accept</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p135991634111413"><a name="p135991634111413"></a><a name="p135991634111413"></a>接受对等连接请求</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p383524711173"><a name="p383524711173"></a><a name="p383524711173"></a>vpc:peerings:accept</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul33641652103217"></a><a name="ul33641652103217"></a><ul id="ul33641652103217"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1821415719143"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p11214957111419"><a name="p11214957111419"></a><a name="p11214957111419"></a>PUT /v2.0/vpc/peerings/{peering_id}/reject</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p1921455713144"><a name="p1921455713144"></a><a name="p1921455713144"></a>拒绝对等连接请求</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p02142057171419"><a name="p02142057171419"></a><a name="p02142057171419"></a>vpc:peerings:reject</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul117422611618"></a><a name="ul117422611618"></a><ul id="ul117422611618"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row134257015151"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p13307113415152"><a name="p13307113415152"></a><a name="p13307113415152"></a>PUT /v2.0/vpc/peerings/{peering_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p74251013151"><a name="p74251013151"></a><a name="p74251013151"></a>更新对等连接</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p2720085191"><a name="p2720085191"></a><a name="p2720085191"></a>vpc:peerings:update</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul758314891613"></a><a name="ul758314891613"></a><ul id="ul758314891613"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row629817252151"><td class="cellrowborder" valign="top" width="37%" headers="mcps1.1.5.1.1 "><p id="p1629862511519"><a name="p1629862511519"></a><a name="p1629862511519"></a>DELETE /v2.0/vpc/peerings/{peering_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p1129816255153"><a name="p1129816255153"></a><a name="p1129816255153"></a>删除对等连接</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p1381162919184"><a name="p1381162919184"></a><a name="p1381162919184"></a>vpc:peerings:delete</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.4 "><a name="ul14304121011169"></a><a name="ul14304121011169"></a><ul id="ul14304121011169"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
</tbody>
</table>

