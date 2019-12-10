# 端口<a name="ZH-CN_TOPIC_0201534290"></a>

<a name="table165141341536"></a>
<table><thead align="left"><tr id="row1060515405312"><th class="cellrowborder" valign="top" width="35.35353535353536%" id="mcps1.1.5.1.1"><p id="p460514415534"><a name="p460514415534"></a><a name="p460514415534"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.1.5.1.2"><p id="p260518435315"><a name="p260518435315"></a><a name="p260518435315"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="16.16161616161616%" id="mcps1.1.5.1.3"><p id="p46053435317"><a name="p46053435317"></a><a name="p46053435317"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="26.26262626262626%" id="mcps1.1.5.1.4"><p id="p960524165312"><a name="p960524165312"></a><a name="p960524165312"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row1260584195313"><td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.5.1.1 "><p id="p176058485311"><a name="p176058485311"></a><a name="p176058485311"></a>GET /v1/{project_id}/ports</p>
</td>
<td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.1.5.1.2 "><p id="p15605144135314"><a name="p15605144135314"></a><a name="p15605144135314"></a>查询端口</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p206058414532"><a name="p206058414532"></a><a name="p206058414532"></a>vpc:ports:get</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p146050419539"><a name="p146050419539"></a><a name="p146050419539"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row260518425310"><td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.5.1.1 "><p id="p76051344536"><a name="p76051344536"></a><a name="p76051344536"></a>GET /v1/{project_id}/ports<strong id="b72361288312"><a name="b72361288312"></a><a name="b72361288312"></a>/</strong>{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.1.5.1.2 "><p id="p1060513425310"><a name="p1060513425310"></a><a name="p1060513425310"></a>查询端口详情</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p1060514125318"><a name="p1060514125318"></a><a name="p1060514125318"></a>vpc:ports:get</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p1260620485312"><a name="p1260620485312"></a><a name="p1260620485312"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row1560612416538"><td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.5.1.1 "><p id="p3606045534"><a name="p3606045534"></a><a name="p3606045534"></a>PUT /v1/{project_id}/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.1.5.1.2 "><p id="p176062475310"><a name="p176062475310"></a><a name="p176062475310"></a>更新端口</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p1606154165312"><a name="p1606154165312"></a><a name="p1606154165312"></a>vpc:ports:update</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p86061542539"><a name="p86061542539"></a><a name="p86061542539"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row126061241530"><td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.5.1.1 "><p id="p66061846533"><a name="p66061846533"></a><a name="p66061846533"></a>DELETE /v1/{project_id}/ports/{port_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.1.5.1.2 "><p id="p1760674135315"><a name="p1760674135315"></a><a name="p1760674135315"></a>删除端口</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p86062411533"><a name="p86062411533"></a><a name="p86062411533"></a>vpc:ports:delete</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p206061845535"><a name="p206061845535"></a><a name="p206061845535"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row16606164125318"><td class="cellrowborder" valign="top" width="35.35353535353536%" headers="mcps1.1.5.1.1 "><p id="p8606174115313"><a name="p8606174115313"></a><a name="p8606174115313"></a>POST / v1/{project_id}/ports</p>
</td>
<td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.1.5.1.2 "><p id="p860617414533"><a name="p860617414533"></a><a name="p860617414533"></a>创建端口</p>
</td>
<td class="cellrowborder" valign="top" width="16.16161616161616%" headers="mcps1.1.5.1.3 "><p id="p13606154135312"><a name="p13606154135312"></a><a name="p13606154135312"></a>vpc:ports:create</p>
</td>
<td class="cellrowborder" valign="top" width="26.26262626262626%" headers="mcps1.1.5.1.4 "><p id="p116066418531"><a name="p116066418531"></a><a name="p116066418531"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
</tbody>
</table>

