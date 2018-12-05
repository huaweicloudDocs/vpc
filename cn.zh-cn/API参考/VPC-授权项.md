# VPC<a name="zh-cn_topic_0132431179"></a>

<a name="table1351682493510"></a>
<table><thead align="left"><tr id="row1759512463518"><th class="cellrowborder" valign="top" width="26%" id="mcps1.1.5.1.1"><p id="p3595424163511"><a name="p3595424163511"></a><a name="p3595424163511"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.1.5.1.2"><p id="p19512155317473"><a name="p19512155317473"></a><a name="p19512155317473"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p19595172413511"><a name="p19595172413511"></a><a name="p19595172413511"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row15595192412355"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p1597124133519"><a name="p1597124133519"></a><a name="p1597124133519"></a>POST /v1/{tenant_id}/vpcs</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.1.5.1.2 "><p id="p8512185310471"><a name="p8512185310471"></a><a name="p8512185310471"></a>创建VPC</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p12647123593510"><a name="p12647123593510"></a><a name="p12647123593510"></a>vpc:vpcs:create</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p107185052510"><a name="p107185052510"></a><a name="p107185052510"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row959782416351"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p1859752463519"><a name="p1859752463519"></a><a name="p1859752463519"></a>GET /v1/{tenant_id}/vpcs/{vpc_id}</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.1.5.1.2 "><p id="p6512145316476"><a name="p6512145316476"></a><a name="p6512145316476"></a>查询VPC</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p01753719354"><a name="p01753719354"></a><a name="p01753719354"></a>vpc:vpcs:get</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p117181501259"><a name="p117181501259"></a><a name="p117181501259"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row459717246353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p145971624193510"><a name="p145971624193510"></a><a name="p145971624193510"></a>GET /v1/{tenant_id}/vpcs</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.1.5.1.2 "><p id="p0512125314718"><a name="p0512125314718"></a><a name="p0512125314718"></a>查询VPC列表</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p6748143803513"><a name="p6748143803513"></a><a name="p6748143803513"></a>vpc:vpcs:list</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p1719903254"><a name="p1719903254"></a><a name="p1719903254"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row1159792493517"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p1559702415358"><a name="p1559702415358"></a><a name="p1559702415358"></a>PUT /v1/{tenant_id}/vpcs/{vpc_id}</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.1.5.1.2 "><p id="p19513175384711"><a name="p19513175384711"></a><a name="p19513175384711"></a>更新VPC</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p1523118428359"><a name="p1523118428359"></a><a name="p1523118428359"></a>vpc:vpcs:update</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p4719701259"><a name="p4719701259"></a><a name="p4719701259"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
<tr id="row85979249353"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.5.1.1 "><p id="p115973243353"><a name="p115973243353"></a><a name="p115973243353"></a>DELETE /v1/{tenant_id}/vpcs/{vpc_id}</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.1.5.1.2 "><p id="p16513135334712"><a name="p16513135334712"></a><a name="p16513135334712"></a>删除VPC</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p841064410359"><a name="p841064410359"></a><a name="p841064410359"></a>vpc:vpcs:delete</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p324462512713"><a name="p324462512713"></a><a name="p324462512713"></a>支持：项目（Project）、企业项目（Enterprise Project）</p>
</td>
</tr>
</tbody>
</table>

