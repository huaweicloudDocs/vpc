# 查询子网列表<a name="vpc_subnet02_0001"></a>

## 功能介绍<a name="section47928120"></a>

查询提交请求的租户的所有子网，单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section28699899"></a>

GET /v2.0/subnets

样例：

```
GET https://{Endpoint}/v2.0/subnets?name={subnet_name}&ip_version={ip_version}&network_id={network_id}&cidr={subnet_cidr_address}&gateway_ip={subnet_gateway}&tenant_id={tenant_id}&enable_dhcp={is_enable_dhcp}
```

分页查询样例：

```
GET https://{Endpoint}/v2.0/subnets?limit=2&marker=011fc878-5521-4654-a1ad-f5b0b5820302&page_reverse=False
```

参数说明请参见[表1](#table3825412149)。

**表 1**  参数说明

<a name="table3825412149"></a>
<table><thead align="left"><tr id="row72051741191419"><th class="cellrowborder" valign="top" width="17.091709170917092%" id="mcps1.2.5.1.1"><p id="p11205114113148"><a name="p11205114113148"></a><a name="p11205114113148"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.271927192719275%" id="mcps1.2.5.1.2"><p id="p1205124171417"><a name="p1205124171417"></a><a name="p1205124171417"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.63166316631663%" id="mcps1.2.5.1.3"><p id="p4205124191411"><a name="p4205124191411"></a><a name="p4205124191411"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="47.004700470047%" id="mcps1.2.5.1.4"><p id="p3205144151413"><a name="p3205144151413"></a><a name="p3205144151413"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8205041111418"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p92051641151419"><a name="p92051641151419"></a><a name="p92051641151419"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p220544113147"><a name="p220544113147"></a><a name="p220544113147"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p162059412145"><a name="p162059412145"></a><a name="p162059412145"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p1205841111418"><a name="p1205841111418"></a><a name="p1205841111418"></a>按照子网对应的ID过滤查询</p>
</td>
</tr>
<tr id="row192054417143"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p620694131411"><a name="p620694131411"></a><a name="p620694131411"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p820619412149"><a name="p820619412149"></a><a name="p820619412149"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p18206114120146"><a name="p18206114120146"></a><a name="p18206114120146"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p920612418149"><a name="p920612418149"></a><a name="p920612418149"></a>按照子网的名称过滤查询</p>
</td>
</tr>
<tr id="row520664131419"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p1206441191420"><a name="p1206441191420"></a><a name="p1206441191420"></a>enable_dhcp</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p16206104131414"><a name="p16206104131414"></a><a name="p16206104131414"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p1206104119142"><a name="p1206104119142"></a><a name="p1206104119142"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p144291518141512"><a name="p144291518141512"></a><a name="p144291518141512"></a>按照子网是否开启dhcp过滤查询</p>
<p id="p142063410146"><a name="p142063410146"></a><a name="p142063410146"></a>取值范围：true or false</p>
</td>
</tr>
<tr id="row4206441171415"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p4206174161415"><a name="p4206174161415"></a><a name="p4206174161415"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p16206104111145"><a name="p16206104111145"></a><a name="p16206104111145"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p0206541121416"><a name="p0206541121416"></a><a name="p0206541121416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p3206164161418"><a name="p3206164161418"></a><a name="p3206164161418"></a>按照子网的cidr过滤查询</p>
</td>
</tr>
<tr id="row720664119147"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p120684191415"><a name="p120684191415"></a><a name="p120684191415"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p020604117141"><a name="p020604117141"></a><a name="p020604117141"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p10206204131416"><a name="p10206204131416"></a><a name="p10206204131416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p192061641131415"><a name="p192061641131415"></a><a name="p192061641131415"></a>按照子网所属network_id过滤查询</p>
</td>
</tr>
<tr id="row1120614111148"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p13206641111413"><a name="p13206641111413"></a><a name="p13206641111413"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p14206154181414"><a name="p14206154181414"></a><a name="p14206154181414"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p11206184161418"><a name="p11206184161418"></a><a name="p11206184161418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p17206134120140"><a name="p17206134120140"></a><a name="p17206134120140"></a>按照子网的IP协议版本过滤查询</p>
</td>
</tr>
<tr id="row122065416145"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p16206114181418"><a name="p16206114181418"></a><a name="p16206114181418"></a>gateway_ip</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p11206941191418"><a name="p11206941191418"></a><a name="p11206941191418"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p6206141191413"><a name="p6206141191413"></a><a name="p6206141191413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p92061741171417"><a name="p92061741171417"></a><a name="p92061741171417"></a>按照子网的网关IP过滤查询</p>
</td>
</tr>
<tr id="row10206174112140"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p420620416149"><a name="p420620416149"></a><a name="p420620416149"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p1620612416148"><a name="p1620612416148"></a><a name="p1620612416148"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p1420620410148"><a name="p1420620410148"></a><a name="p1420620410148"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p72071941181420"><a name="p72071941181420"></a><a name="p72071941181420"></a>按照子网所属的项目ID过滤查询</p>
</td>
</tr>
<tr id="row1720744110145"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p112071541201414"><a name="p112071541201414"></a><a name="p112071541201414"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p7207841141412"><a name="p7207841141412"></a><a name="p7207841141412"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p1207114117140"><a name="p1207114117140"></a><a name="p1207114117140"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p20207341121416"><a name="p20207341121416"></a><a name="p20207341121416"></a>分页查询起始的资源ID，为空时为查询第一页</p>
</td>
</tr>
<tr id="row220774110141"><td class="cellrowborder" valign="top" width="17.091709170917092%" headers="mcps1.2.5.1.1 "><p id="p82075416148"><a name="p82075416148"></a><a name="p82075416148"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="19.271927192719275%" headers="mcps1.2.5.1.2 "><p id="p1720714413143"><a name="p1720714413143"></a><a name="p1720714413143"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63166316631663%" headers="mcps1.2.5.1.3 "><p id="p1620714117148"><a name="p1620714117148"></a><a name="p1620714117148"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="47.004700470047%" headers="mcps1.2.5.1.4 "><p id="p2518132611514"><a name="p2518132611514"></a><a name="p2518132611514"></a>每页返回的个数</p>
<p id="p1420704119149"><a name="p1420704119149"></a><a name="p1420704119149"></a>取值范围：0~intmax</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section42990474"></a>

无。

## 响应消息<a name="section51369953"></a>

**表 2**  响应参数

<a name="table51277242"></a>
<table><thead align="left"><tr id="row64740644"><th class="cellrowborder" valign="top" width="23.122312231223123%" id="mcps1.2.4.1.1"><p id="p9500791"><a name="p9500791"></a><a name="p9500791"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.552555255525554%" id="mcps1.2.4.1.2"><p id="p31366578"><a name="p31366578"></a><a name="p31366578"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.325132513251326%" id="mcps1.2.4.1.3"><p id="p40344834"><a name="p40344834"></a><a name="p40344834"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46706151"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p25101909"><a name="p25101909"></a><a name="p25101909"></a>subnets</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p21426146239"><a name="p21426146239"></a><a name="p21426146239"></a>Array of <a href="#table176735992713">subnet</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p15291872"><a name="p15291872"></a><a name="p15291872"></a>subnet对象列表，参见<a href="#table176735992713">表3</a>。</p>
</td>
</tr>
<tr id="row9988173210387"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p12599163715385"><a name="p12599163715385"></a><a name="p12599163715385"></a>subnets_links</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p9599173717383"><a name="p9599173717383"></a><a name="p9599173717383"></a>Array of <a href="#table10817112933915">subnets_link</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p155991337143818"><a name="p155991337143818"></a><a name="p155991337143818"></a>分页信息，参见<a href="#table10817112933915">表6</a> 。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  subnet对象

<a name="table176735992713"></a>
<table><thead align="left"><tr id="row176713593276"><th class="cellrowborder" valign="top" width="28.332833283328334%" id="mcps1.2.4.1.1"><p id="p136755912715"><a name="p136755912715"></a><a name="p136755912715"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="28.292829282928288%" id="mcps1.2.4.1.2"><p id="p667105912718"><a name="p667105912718"></a><a name="p667105912718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.37433743374337%" id="mcps1.2.4.1.3"><p id="p26855915275"><a name="p26855915275"></a><a name="p26855915275"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row28303131105515"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p2014344105614"><a name="p2014344105614"></a><a name="p2014344105614"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p28944191105614"><a name="p28944191105614"></a><a name="p28944191105614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p53796361105614"><a name="p53796361105614"></a><a name="p53796361105614"></a>子网的id</p>
<p id="p2677113954519"><a name="p2677113954519"></a><a name="p2677113954519"></a>【使用说明】在查询子网列表时非必选</p>
</td>
</tr>
<tr id="row1868135972719"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p37015595272"><a name="p37015595272"></a><a name="p37015595272"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p18706591271"><a name="p18706591271"></a><a name="p18706591271"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p1870259172715"><a name="p1870259172715"></a><a name="p1870259172715"></a>子网的名称</p>
</td>
</tr>
<tr id="row670165910271"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p187012596279"><a name="p187012596279"></a><a name="p187012596279"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p137095922720"><a name="p137095922720"></a><a name="p137095922720"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p870155932715"><a name="p870155932715"></a><a name="p870155932715"></a>IP版本</p>
<p id="p10708598273"><a name="p10708598273"></a><a name="p10708598273"></a>【使用说明】只支持IPv4</p>
</td>
</tr>
<tr id="row1270135915274"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p1770105919271"><a name="p1770105919271"></a><a name="p1770105919271"></a>ipv6_address_mode</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p1370205912279"><a name="p1370205912279"></a><a name="p1370205912279"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p5701759142713"><a name="p5701759142713"></a><a name="p5701759142713"></a>IPv6寻址模式</p>
</td>
</tr>
<tr id="row57075913279"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p070195972715"><a name="p070195972715"></a><a name="p070195972715"></a>ipv6_ra_mode</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p1970559102716"><a name="p1970559102716"></a><a name="p1970559102716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p19701959152712"><a name="p19701959152712"></a><a name="p19701959152712"></a>IPv6路由广播模式</p>
</td>
</tr>
<tr id="row970185911274"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p5719599271"><a name="p5719599271"></a><a name="p5719599271"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p1671105982710"><a name="p1671105982710"></a><a name="p1671105982710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p1071259102716"><a name="p1071259102716"></a><a name="p1071259102716"></a>所属网络的id</p>
</td>
</tr>
<tr id="row9711659142718"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p1471155922712"><a name="p1471155922712"></a><a name="p1471155922712"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p1871155912279"><a name="p1871155912279"></a><a name="p1871155912279"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p471115972720"><a name="p471115972720"></a><a name="p471115972720"></a>CIDR格式</p>
<p id="p171105952717"><a name="p171105952717"></a><a name="p171105952717"></a>【使用说明】只支持10.0.0.0/8,172.16.0.0/12,192.168.0.0/16三个网段内的地址，掩码长度不能大于28。</p>
</td>
</tr>
<tr id="row373659122718"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p173195914274"><a name="p173195914274"></a><a name="p173195914274"></a>gateway_ip</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p16733594272"><a name="p16733594272"></a><a name="p16733594272"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p167319597276"><a name="p167319597276"></a><a name="p167319597276"></a>网关IP不允许和allocation_pools地址块冲突。</p>
<p id="p1773175918271"><a name="p1773175918271"></a><a name="p1773175918271"></a>【使用说明】不支持修改。</p>
</td>
</tr>
<tr id="row6733598278"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p37325918273"><a name="p37325918273"></a><a name="p37325918273"></a>allocation_pools</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p166911588244"><a name="p166911588244"></a><a name="p166911588244"></a>Array of <a href="#table1777145918276">allocation_pool</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p13740597271"><a name="p13740597271"></a><a name="p13740597271"></a>可用的IP池，allocation_pool对象参见<a href="#table1777145918276">表3 allocation_pool对象</a></p>
<p id="p137415915279"><a name="p137415915279"></a><a name="p137415915279"></a>例如：[ { "start": "10.0.0.2", "end": "10.0.0.251"} ]</p>
<p id="p167414592279"><a name="p167414592279"></a><a name="p167414592279"></a>每个子网的第1个和最后3个IP地址为系统保留地址。以192.168.1.0/24为例，192.168.1.0、 192.168.1.253、192.168.1.254和192.168.1.255这些地址是系统保留地址。系统预留地址默认不在allocation_pool范围内。</p>
<p id="p074359192720"><a name="p074359192720"></a><a name="p074359192720"></a>约束：更新时allocation_pool范围不能包含网关和广播地址的所有IP。</p>
</td>
</tr>
<tr id="row474205911270"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p774105972720"><a name="p774105972720"></a><a name="p774105972720"></a>dns_nameservers</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p1474155952710"><a name="p1474155952710"></a><a name="p1474155952710"></a>Array&nbsp;of&nbsp;strings</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p10743593273"><a name="p10743593273"></a><a name="p10743593273"></a>dns服务器</p>
<p id="p97485912712"><a name="p97485912712"></a><a name="p97485912712"></a>例如："dns_nameservers": ["8.xx.xx.8","8.xx.xx.4"]</p>
</td>
</tr>
<tr id="row6741659182714"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p574959122713"><a name="p574959122713"></a><a name="p574959122713"></a>host_routes</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p18246193118245"><a name="p18246193118245"></a><a name="p18246193118245"></a>Array of <a href="#table177865912715">host_route</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p2074459132712"><a name="p2074459132712"></a><a name="p2074459132712"></a>虚拟机静态路由，参见“<a href="#table177865912715">表5</a></p>
<p id="p1674359172717"><a name="p1674359172717"></a><a name="p1674359172717"></a>【使用说明】不支持，忽略输入信息</p>
</td>
</tr>
<tr id="row42017779105653"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p5182838910577"><a name="p5182838910577"></a><a name="p5182838910577"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p3734998010577"><a name="p3734998010577"></a><a name="p3734998010577"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row97535914274"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p475959202718"><a name="p475959202718"></a><a name="p475959202718"></a>enable_dhcp</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p2755596279"><a name="p2755596279"></a><a name="p2755596279"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p47595962710"><a name="p47595962710"></a><a name="p47595962710"></a>是否启动dhcp，false表示不提供dhcp服务的能力</p>
<p id="p57535914276"><a name="p57535914276"></a><a name="p57535914276"></a>【使用说明】只支持true</p>
</td>
</tr>
<tr id="row63315321123"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p45641422124917"><a name="p45641422124917"></a><a name="p45641422124917"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p113781259182412"><a name="p113781259182412"></a><a name="p113781259182412"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row126291040191211"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间，UTC时间</p>
<p id="p65980291419"><a name="p65980291419"></a><a name="p65980291419"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row1084513362123"><td class="cellrowborder" valign="top" width="28.332833283328334%" headers="mcps1.2.4.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.292829282928288%" headers="mcps1.2.4.1.2 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.37433743374337%" headers="mcps1.2.4.1.3 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间，UTC时间</p>
<p id="p10406183916467"><a name="p10406183916467"></a><a name="p10406183916467"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

**表 4**  allocation\_pool对象

<a name="table1777145918276"></a>
<table><thead align="left"><tr id="row11772597275"><th class="cellrowborder" valign="top" width="23.65%" id="mcps1.2.4.1.1"><p id="p1477155962713"><a name="p1477155962713"></a><a name="p1477155962713"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="24.610000000000003%" id="mcps1.2.4.1.2"><p id="p1077859162717"><a name="p1077859162717"></a><a name="p1077859162717"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.739999999999995%" id="mcps1.2.4.1.3"><p id="p5771159182718"><a name="p5771159182718"></a><a name="p5771159182718"></a>备注</p>
</th>
</tr>
</thead>
<tbody><tr id="row167785982711"><td class="cellrowborder" valign="top" width="23.65%" headers="mcps1.2.4.1.1 "><p id="p1077159182720"><a name="p1077159182720"></a><a name="p1077159182720"></a>start</p>
</td>
<td class="cellrowborder" valign="top" width="24.610000000000003%" headers="mcps1.2.4.1.2 "><p id="p2077125912718"><a name="p2077125912718"></a><a name="p2077125912718"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.739999999999995%" headers="mcps1.2.4.1.3 "><p id="p2078205910275"><a name="p2078205910275"></a><a name="p2078205910275"></a>网络池起始IP</p>
</td>
</tr>
<tr id="row1782594271"><td class="cellrowborder" valign="top" width="23.65%" headers="mcps1.2.4.1.1 "><p id="p9781459162717"><a name="p9781459162717"></a><a name="p9781459162717"></a>end</p>
</td>
<td class="cellrowborder" valign="top" width="24.610000000000003%" headers="mcps1.2.4.1.2 "><p id="p1778115952719"><a name="p1778115952719"></a><a name="p1778115952719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.739999999999995%" headers="mcps1.2.4.1.3 "><p id="p187825911271"><a name="p187825911271"></a><a name="p187825911271"></a>网络池结束IP</p>
</td>
</tr>
</tbody>
</table>

**表 5**  host\_route对象

<a name="table177865912715"></a>
<table><thead align="left"><tr id="row1779145992719"><th class="cellrowborder" valign="top" width="23.712371237123715%" id="mcps1.2.4.1.1"><p id="p2794593271"><a name="p2794593271"></a><a name="p2794593271"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="24.4024402440244%" id="mcps1.2.4.1.2"><p id="p14791594271"><a name="p14791594271"></a><a name="p14791594271"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.88518851885189%" id="mcps1.2.4.1.3"><p id="p14791459172716"><a name="p14791459172716"></a><a name="p14791459172716"></a>备注</p>
</th>
</tr>
</thead>
<tbody><tr id="row1379165919277"><td class="cellrowborder" valign="top" width="23.712371237123715%" headers="mcps1.2.4.1.1 "><p id="p979165972710"><a name="p979165972710"></a><a name="p979165972710"></a>destination</p>
</td>
<td class="cellrowborder" valign="top" width="24.4024402440244%" headers="mcps1.2.4.1.2 "><p id="p37995952710"><a name="p37995952710"></a><a name="p37995952710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.88518851885189%" headers="mcps1.2.4.1.3 "><p id="p10791559172714"><a name="p10791559172714"></a><a name="p10791559172714"></a>路由目的子网</p>
</td>
</tr>
<tr id="row1779185915279"><td class="cellrowborder" valign="top" width="23.712371237123715%" headers="mcps1.2.4.1.1 "><p id="p6791359102719"><a name="p6791359102719"></a><a name="p6791359102719"></a>nexthop</p>
</td>
<td class="cellrowborder" valign="top" width="24.4024402440244%" headers="mcps1.2.4.1.2 "><p id="p107935942717"><a name="p107935942717"></a><a name="p107935942717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.88518851885189%" headers="mcps1.2.4.1.3 "><p id="p87975920278"><a name="p87975920278"></a><a name="p87975920278"></a>路由下一跳IP</p>
</td>
</tr>
</tbody>
</table>

**表 6**  subnets\_link对象

<a name="table10817112933915"></a>
<table><thead align="left"><tr id="row988812911394"><th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.1"><p id="p2888112916394"><a name="p2888112916394"></a><a name="p2888112916394"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.2"><p id="p488802911392"><a name="p488802911392"></a><a name="p488802911392"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="71.72%" id="mcps1.2.4.1.3"><p id="p68883299394"><a name="p68883299394"></a><a name="p68883299394"></a>备注</p>
</th>
</tr>
</thead>
<tbody><tr id="row0888172913919"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p18888162993911"><a name="p18888162993911"></a><a name="p18888162993911"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p1888842943911"><a name="p1888842943911"></a><a name="p1888842943911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p88882295396"><a name="p88882295396"></a><a name="p88882295396"></a>API链接</p>
</td>
</tr>
<tr id="row4888172913395"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p1288872918396"><a name="p1288872918396"></a><a name="p1288872918396"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p1889929143911"><a name="p1889929143911"></a><a name="p1889929143911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p48899296394"><a name="p48899296394"></a><a name="p48899296394"></a>API链接与该API版本的关系</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section64320104111236"></a>

请求样例

```
GET https://{Endpoint}/v2.0/subnets?limit=1
```

响应样例

```
{
    "subnets": [
        {
            "name": "kesmdemeet",
            "cidr": "172.16.236.0/24",
            "id": "011fc878-5521-4654-a1ad-f5b0b5820302",
            "enable_dhcp": true,
            "network_id": "48efad0c-079d-4cc8-ace0-dce35d584124",
            "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
            "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
            "dns_nameservers": [],
            "allocation_pools": [
                {
                    "start": "172.16.236.2",
                    "end": "172.16.236.251"
                }
            ],
            "host_routes": [],
            "ip_version": 4,
            "gateway_ip": "172.16.236.1",
            "created_at": "2018-03-26T08:23:43",
            "updated_at": "2018-03-26T08:23:44"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

