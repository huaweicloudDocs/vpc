# 浮动IP（Openstack Neutron API）<a name="ZH-CN_TOPIC_0103208474"></a>

<a name="table620116613438"></a>
<table><thead align="left"><tr id="row122422612431"><th class="cellrowborder" valign="top" width="27.272727272727277%" id="mcps1.1.5.1.1"><p id="p18242167434"><a name="p18242167434"></a><a name="p18242167434"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="12.121212121212121%" id="mcps1.1.5.1.2"><p id="p1742017470614"><a name="p1742017470614"></a><a name="p1742017470614"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.3"><p id="p132426674312"><a name="p132426674312"></a><a name="p132426674312"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="42.42424242424242%" id="mcps1.1.5.1.4"><p id="p1366363695811"><a name="p1366363695811"></a><a name="p1366363695811"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row11242186124315"><td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.1 "><p id="p16242156154311"><a name="p16242156154311"></a><a name="p16242156154311"></a>GET /v2.0/floatingips</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.1.5.1.2 "><p id="p1942012471564"><a name="p1942012471564"></a><a name="p1942012471564"></a>查询浮动IP列表</p>
</td>
<td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.3 "><p id="p5358141413439"><a name="p5358141413439"></a><a name="p5358141413439"></a>vpc:floatingIps:get</p>
</td>
<td class="cellrowborder" valign="top" width="42.42424242424242%" headers="mcps1.1.5.1.4 "><a name="ul66241846203119"></a><a name="ul66241846203119"></a><ul id="ul66241846203119"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1424216134314"><td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.1 "><p id="p1124219664317"><a name="p1124219664317"></a><a name="p1124219664317"></a>GET /v2.0/floatingips/{floatingip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.1.5.1.2 "><p id="p9420164712614"><a name="p9420164712614"></a><a name="p9420164712614"></a>查询浮动IP</p>
</td>
<td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.3 "><p id="p1818716161433"><a name="p1818716161433"></a><a name="p1818716161433"></a>vpc:floatingIps:get</p>
</td>
<td class="cellrowborder" valign="top" width="42.42424242424242%" headers="mcps1.1.5.1.4 "><a name="ul95023481322"></a><a name="ul95023481322"></a><ul id="ul95023481322"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row192471262439"><td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.1 "><p id="p92473619434"><a name="p92473619434"></a><a name="p92473619434"></a>POST /v2.0/floatingips</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.1.5.1.2 "><p id="p13420547366"><a name="p13420547366"></a><a name="p13420547366"></a>创建浮动IP</p>
</td>
<td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.3 "><p id="p142981517134319"><a name="p142981517134319"></a><a name="p142981517134319"></a>vpc:floatingIps:create</p>
</td>
<td class="cellrowborder" valign="top" width="42.42424242424242%" headers="mcps1.1.5.1.4 "><a name="ul15513950173211"></a><a name="ul15513950173211"></a><ul id="ul15513950173211"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row1724719674312"><td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.1 "><p id="p1224756134320"><a name="p1224756134320"></a><a name="p1224756134320"></a>PUT /v2.0/floatingips/{floatingip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.1.5.1.2 "><p id="p16420347065"><a name="p16420347065"></a><a name="p16420347065"></a>更新浮动IP</p>
</td>
<td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.3 "><p id="p17326101812436"><a name="p17326101812436"></a><a name="p17326101812436"></a>vpc:floatingIps:update</p>
</td>
<td class="cellrowborder" valign="top" width="42.42424242424242%" headers="mcps1.1.5.1.4 "><a name="ul33641652103217"></a><a name="ul33641652103217"></a><ul id="ul33641652103217"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
<tr id="row102470615434"><td class="cellrowborder" valign="top" width="27.272727272727277%" headers="mcps1.1.5.1.1 "><p id="p9247126204318"><a name="p9247126204318"></a><a name="p9247126204318"></a>DELETE /v2.0/floatingips/{floatingip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.1.5.1.2 "><p id="p1542119471269"><a name="p1542119471269"></a><a name="p1542119471269"></a>删除浮动IP</p>
</td>
<td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.3 "><p id="p64451919134314"><a name="p64451919134314"></a><a name="p64451919134314"></a>vpc:floatingIps:delete</p>
</td>
<td class="cellrowborder" valign="top" width="42.42424242424242%" headers="mcps1.1.5.1.4 "><a name="ul185134914469"></a><a name="ul185134914469"></a><ul id="ul185134914469"><li>支持：项目（Project）</li><li>不支持：企业项目（Enterprise Project）</li></ul>
</td>
</tr>
</tbody>
</table>

