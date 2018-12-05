# 浮动IP API简介<a name="ZH-CN_TOPIC_0060634441"></a>

## 对象简介<a name="section42616019164"></a>

对浮动IP资源进行管理和操作，包括查询浮动IP、创建浮动IP、查询指定浮动IP、删除浮动IP以及更新浮动IP等接口。

>![](public_sys-resources/icon-note.gif) **说明：**   
>浮动IP（原生Openstack接口）与[弹性公网IP](弹性公网IP.md)功能类似，主要不同点在于浮动IP接口无法配置带宽参数。  

## 对象模型<a name="section4223558419164"></a>

**表 1**  浮动IP对象

<a name="table5388109319164"></a>
<table><thead align="left"><tr id="row6462628919164"><th class="cellrowborder" valign="top" width="14.948505149485051%" id="mcps1.2.8.1.1"><p id="p23806019164"><a name="p23806019164"></a><a name="p23806019164"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="7.519248075192481%" id="mcps1.2.8.1.2"><p id="p868823916540"><a name="p868823916540"></a><a name="p868823916540"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.078692130786921%" id="mcps1.2.8.1.3"><p id="p1928287519164"><a name="p1928287519164"></a><a name="p1928287519164"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.339066093390661%" id="mcps1.2.8.1.4"><p id="p1840903119164"><a name="p1840903119164"></a><a name="p1840903119164"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="13.078692130786921%" id="mcps1.2.8.1.5"><p id="p1473650319164"><a name="p1473650319164"></a><a name="p1473650319164"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="13.078692130786921%" id="mcps1.2.8.1.6"><p id="p5280606719164"><a name="p5280606719164"></a><a name="p5280606719164"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="28.957104289571046%" id="mcps1.2.8.1.7"><p id="p4943306019164"><a name="p4943306019164"></a><a name="p4943306019164"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4465496219164"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p6028218019164"><a name="p6028218019164"></a><a name="p6028218019164"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p14688133913546"><a name="p14688133913546"></a><a name="p14688133913546"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p5101843519164"><a name="p5101843519164"></a><a name="p5101843519164"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p3885256619164"><a name="p3885256619164"></a><a name="p3885256619164"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p6005015019164"><a name="p6005015019164"></a><a name="p6005015019164"></a>DOWN</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p3222396219164"><a name="p3222396219164"></a><a name="p3222396219164"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p6000412319164"><a name="p6000412319164"></a><a name="p6000412319164"></a>网络状态，可以为ACTIVE， DOWN或ERROR。</p>
</td>
</tr>
<tr id="row316619519164"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p5513524919164"><a name="p5513524919164"></a><a name="p5513524919164"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p0689103915411"><a name="p0689103915411"></a><a name="p0689103915411"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p3677022419164"><a name="p3677022419164"></a><a name="p3677022419164"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p2559820019164"><a name="p2559820019164"></a><a name="p2559820019164"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p6018830419164"><a name="p6018830419164"></a><a name="p6018830419164"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p4341443219164"><a name="p4341443219164"></a><a name="p4341443219164"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p2690811319164"><a name="p2690811319164"></a><a name="p2690811319164"></a>浮动IP地址的id。</p>
<p id="p6641157838"><a name="p6641157838"></a><a name="p6641157838"></a>【使用说明】创建浮动IP时不选。</p>
</td>
</tr>
<tr id="row4084642919164"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p2022646619164"><a name="p2022646619164"></a><a name="p2022646619164"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p17689839165418"><a name="p17689839165418"></a><a name="p17689839165418"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p2773103519164"><a name="p2773103519164"></a><a name="p2773103519164"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p3162136119164"><a name="p3162136119164"></a><a name="p3162136119164"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p1119341919164"><a name="p1119341919164"></a><a name="p1119341919164"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p3425172919164"><a name="p3425172919164"></a><a name="p3425172919164"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p2292670119164"><a name="p2292670119164"></a><a name="p2292670119164"></a>浮动IP地址。</p>
</td>
</tr>
<tr id="row501371719164"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p345796219164"><a name="p345796219164"></a><a name="p345796219164"></a>floating_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p1068933955414"><a name="p1068933955414"></a><a name="p1068933955414"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p1165952819164"><a name="p1165952819164"></a><a name="p1165952819164"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p489768619164"><a name="p489768619164"></a><a name="p489768619164"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p6116825219164"><a name="p6116825219164"></a><a name="p6116825219164"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p5568137919164"><a name="p5568137919164"></a><a name="p5568137919164"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p1389784219164"><a name="p1389784219164"></a><a name="p1389784219164"></a>外部网络的id。</p>
<p id="p5797172119164"><a name="p5797172119164"></a><a name="p5797172119164"></a>只能使用固定的外网，外部网络的信息请通过GET /v2.0/networks?router:external=True或GET /v2.0/networks?name={floating_network}或neutron net-external-list方式查询。</p>
</td>
</tr>
<tr id="row5198344219164"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p4990929119164"><a name="p4990929119164"></a><a name="p4990929119164"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p196892395545"><a name="p196892395545"></a><a name="p196892395545"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p1612074019164"><a name="p1612074019164"></a><a name="p1612074019164"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p3071152519164"><a name="p3071152519164"></a><a name="p3071152519164"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p460559119164"><a name="p460559119164"></a><a name="p460559119164"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p3750857719164"><a name="p3750857719164"></a><a name="p3750857719164"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p1829591619164"><a name="p1829591619164"></a><a name="p1829591619164"></a>所属路由器id。</p>
<p id="p3044552119164"><a name="p3044552119164"></a><a name="p3044552119164"></a></p>
</td>
</tr>
<tr id="row557424019164"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p4886025919164"><a name="p4886025919164"></a><a name="p4886025919164"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p1868973975414"><a name="p1868973975414"></a><a name="p1868973975414"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p6536694419164"><a name="p6536694419164"></a><a name="p6536694419164"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p6023110119164"><a name="p6023110119164"></a><a name="p6023110119164"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p4688099419164"><a name="p4688099419164"></a><a name="p4688099419164"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p3926418419164"><a name="p3926418419164"></a><a name="p3926418419164"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p2628234219164"><a name="p2628234219164"></a><a name="p2628234219164"></a>端口id</p>
</td>
</tr>
<tr id="row3521449419164"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p3380179719164"><a name="p3380179719164"></a><a name="p3380179719164"></a>fixed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p368912399543"><a name="p368912399543"></a><a name="p368912399543"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p5359099919164"><a name="p5359099919164"></a><a name="p5359099919164"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p4590367819164"><a name="p4590367819164"></a><a name="p4590367819164"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p2721046619164"><a name="p2721046619164"></a><a name="p2721046619164"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p5656413819164"><a name="p5656413819164"></a><a name="p5656413819164"></a>IP地址或空</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p1829247919164"><a name="p1829247919164"></a><a name="p1829247919164"></a>关联端口的私有IP地址。</p>
</td>
</tr>
<tr id="row529581619164"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p2630795019164"><a name="p2630795019164"></a><a name="p2630795019164"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p5689123914544"><a name="p5689123914544"></a><a name="p5689123914544"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p5056917619164"><a name="p5056917619164"></a><a name="p5056917619164"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p246257419164"><a name="p246257419164"></a><a name="p246257419164"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p6525084219164"><a name="p6525084219164"></a><a name="p6525084219164"></a>当前认证租户</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p5082681719164"><a name="p5082681719164"></a><a name="p5082681719164"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p2333153319164"><a name="p2333153319164"></a><a name="p2333153319164"></a>项目ID。</p>
</td>
</tr>
<tr id="row43561298173"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p17700201411911"><a name="p17700201411911"></a><a name="p17700201411911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p137605535468"><a name="p137605535468"></a><a name="p137605535468"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p17000141292"><a name="p17000141292"></a><a name="p17000141292"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p1470010141396"><a name="p1470010141396"></a><a name="p1470010141396"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p870017141892"><a name="p870017141892"></a><a name="p870017141892"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p7700714691"><a name="p7700714691"></a><a name="p7700714691"></a>资源project_id</p>
</td>
</tr>
<tr id="row153664173177"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p6953241598"><a name="p6953241598"></a><a name="p6953241598"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p6953441993"><a name="p6953441993"></a><a name="p6953441993"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p11953164120911"><a name="p11953164120911"></a><a name="p11953164120911"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p595314119912"><a name="p595314119912"></a><a name="p595314119912"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间</p>
</td>
</tr>
<tr id="row871312131173"><td class="cellrowborder" valign="top" width="14.948505149485051%" headers="mcps1.2.8.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.8.1.2 "><p id="p33972541493"><a name="p33972541493"></a><a name="p33972541493"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.3 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.339066093390661%" headers="mcps1.2.8.1.4 "><p id="p339716540919"><a name="p339716540919"></a><a name="p339716540919"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.5 "><p id="p1739717541895"><a name="p1739717541895"></a><a name="p1739717541895"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.078692130786921%" headers="mcps1.2.8.1.6 "><p id="p12397054697"><a name="p12397054697"></a><a name="p12397054697"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.957104289571046%" headers="mcps1.2.8.1.7 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间</p>
</td>
</tr>
</tbody>
</table>

