# 路由器API简介<a name="ZH-CN_TOPIC_0060495813"></a>

## 对象简介<a name="section45495122"></a>

对路由器资源进行管理和操作，包括查询路由器列表、创建路由器、查询指定路由器、删除路由器以及更新路由器等接口。

## 响应参数<a name="section56953834205730"></a>

**表 1**  router对象

<a name="table24153696181443"></a>
<table><thead align="left"><tr id="row11861342181443"><th class="cellrowborder" valign="top" width="15.101510151015102%" id="mcps1.2.8.1.1"><p id="p21244677181443"><a name="p21244677181443"></a><a name="p21244677181443"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="7.520752075207521%" id="mcps1.2.8.1.2"><p id="p981918394815"><a name="p981918394815"></a><a name="p981918394815"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.211321132113211%" id="mcps1.2.8.1.3"><p id="p43097239181443"><a name="p43097239181443"></a><a name="p43097239181443"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.43094309430943%" id="mcps1.2.8.1.4"><p id="p1215486181443"><a name="p1215486181443"></a><a name="p1215486181443"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="13.211321132113211%" id="mcps1.2.8.1.5"><p id="p31345570181443"><a name="p31345570181443"></a><a name="p31345570181443"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="13.211321132113211%" id="mcps1.2.8.1.6"><p id="p55963242181443"><a name="p55963242181443"></a><a name="p55963242181443"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="28.312831283128315%" id="mcps1.2.8.1.7"><p id="p36728767181443"><a name="p36728767181443"></a><a name="p36728767181443"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row22240136181443"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p56620590181443"><a name="p56620590181443"></a><a name="p56620590181443"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p08199313484"><a name="p08199313484"></a><a name="p08199313484"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p22865048181443"><a name="p22865048181443"></a><a name="p22865048181443"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p40129582181443"><a name="p40129582181443"></a><a name="p40129582181443"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p29270746181443"><a name="p29270746181443"></a><a name="p29270746181443"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p22120193181443"><a name="p22120193181443"></a><a name="p22120193181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p46905229181443"><a name="p46905229181443"></a><a name="p46905229181443"></a>路由器的id</p>
<p id="p121142486504"><a name="p121142486504"></a><a name="p121142486504"></a>【使用说明】在查询路由器列表时非必选</p>
</td>
</tr>
<tr id="row19493885181443"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p35500827181443"><a name="p35500827181443"></a><a name="p35500827181443"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p1881923164818"><a name="p1881923164818"></a><a name="p1881923164818"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p56994705181443"><a name="p56994705181443"></a><a name="p56994705181443"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p53168392181443"><a name="p53168392181443"></a><a name="p53168392181443"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p11672487181443"><a name="p11672487181443"></a><a name="p11672487181443"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p5947415181443"><a name="p5947415181443"></a><a name="p5947415181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p11978624181443"><a name="p11978624181443"></a><a name="p11978624181443"></a>路由器的名称。</p>
<p id="p30744457181443"><a name="p30744457181443"></a><a name="p30744457181443"></a>仅支持数字、字母、_(下划线)、-（中划线）、.（点）。</p>
</td>
</tr>
<tr id="row8264657181443"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p65457453181443"><a name="p65457453181443"></a><a name="p65457453181443"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p9819193104813"><a name="p9819193104813"></a><a name="p9819193104813"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p453502181443"><a name="p453502181443"></a><a name="p453502181443"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p36733740181443"><a name="p36733740181443"></a><a name="p36733740181443"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p22642974181443"><a name="p22642974181443"></a><a name="p22642974181443"></a>true</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p22141629181443"><a name="p22141629181443"></a><a name="p22141629181443"></a>true或false</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p48641520181443"><a name="p48641520181443"></a><a name="p48641520181443"></a>管理状态。</p>
<p id="p35120501181443"><a name="p35120501181443"></a><a name="p35120501181443"></a>只支持true。</p>
</td>
</tr>
<tr id="row47649056181443"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p34368308181443"><a name="p34368308181443"></a><a name="p34368308181443"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p168191337481"><a name="p168191337481"></a><a name="p168191337481"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p32369557181443"><a name="p32369557181443"></a><a name="p32369557181443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p4688426181443"><a name="p4688426181443"></a><a name="p4688426181443"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p44218203181443"><a name="p44218203181443"></a><a name="p44218203181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p24904722181443"><a name="p24904722181443"></a><a name="p24904722181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p4016564181443"><a name="p4016564181443"></a><a name="p4016564181443"></a>状态，可以为ACTIVE， DOWN，ERROR。</p>
</td>
</tr>
<tr id="row36149082181443"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p42394506181443"><a name="p42394506181443"></a><a name="p42394506181443"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p1081916312487"><a name="p1081916312487"></a><a name="p1081916312487"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p11402971181443"><a name="p11402971181443"></a><a name="p11402971181443"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p51225460181443"><a name="p51225460181443"></a><a name="p51225460181443"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p55621630181443"><a name="p55621630181443"></a><a name="p55621630181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p9058209181443"><a name="p9058209181443"></a><a name="p9058209181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p62626308181443"><a name="p62626308181443"></a><a name="p62626308181443"></a>项目ID。</p>
</td>
</tr>
<tr id="row26765861181443"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p20551115181443"><a name="p20551115181443"></a><a name="p20551115181443"></a>external_gateway_info</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p1281914344820"><a name="p1281914344820"></a><a name="p1281914344820"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p54027655181443"><a name="p54027655181443"></a><a name="p54027655181443"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p14163902181443"><a name="p14163902181443"></a><a name="p14163902181443"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p6425434181443"><a name="p6425434181443"></a><a name="p6425434181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p50698179181443"><a name="p50698179181443"></a><a name="p50698179181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p12911840181443"><a name="p12911840181443"></a><a name="p12911840181443"></a>扩展属性：外部网关信息，参见<a href="#ZH-CN_TOPIC_0060495813__table11448068181443">表2</a>。</p>
</td>
</tr>
<tr id="row49097702181443"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p17490925181443"><a name="p17490925181443"></a><a name="p17490925181443"></a>routes</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p12819143204816"><a name="p12819143204816"></a><a name="p12819143204816"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p7478812181443"><a name="p7478812181443"></a><a name="p7478812181443"></a>List(route)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p1804060181443"><a name="p1804060181443"></a><a name="p1804060181443"></a>RU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p11911189181443"><a name="p11911189181443"></a><a name="p11911189181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p25282222181443"><a name="p25282222181443"></a><a name="p25282222181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p5122123194853"><a name="p5122123194853"></a><a name="p5122123194853"></a>扩展属性：路由信息列表，<a href="#ZH-CN_TOPIC_0060495813__table18829650181443">表3</a>。</p>
</td>
</tr>
<tr id="row7278189151614"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p17700201411911"><a name="p17700201411911"></a><a name="p17700201411911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p15700614790"><a name="p15700614790"></a><a name="p15700614790"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p17000141292"><a name="p17000141292"></a><a name="p17000141292"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p1470010141396"><a name="p1470010141396"></a><a name="p1470010141396"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p870017141892"><a name="p870017141892"></a><a name="p870017141892"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p7700714691"><a name="p7700714691"></a><a name="p7700714691"></a>资源project_id</p>
</td>
</tr>
<tr id="row172292215166"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p6953241598"><a name="p6953241598"></a><a name="p6953241598"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p6953441993"><a name="p6953441993"></a><a name="p6953441993"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p11953164120911"><a name="p11953164120911"></a><a name="p11953164120911"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p595314119912"><a name="p595314119912"></a><a name="p595314119912"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间</p>
</td>
</tr>
<tr id="row106341917161611"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p33972541493"><a name="p33972541493"></a><a name="p33972541493"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p339716540919"><a name="p339716540919"></a><a name="p339716540919"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p1739717541895"><a name="p1739717541895"></a><a name="p1739717541895"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p12397054697"><a name="p12397054697"></a><a name="p12397054697"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间</p>
</td>
</tr>
</tbody>
</table>

**表 2**  external\_gateway\_info对象

<a name="table11448068181443"></a>
<table><thead align="left"><tr id="row58732356181443"><th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.7.1.1"><p id="p59700400181443"><a name="p59700400181443"></a><a name="p59700400181443"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.7.1.2"><p id="p3894228181443"><a name="p3894228181443"></a><a name="p3894228181443"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.1989801019898%" id="mcps1.2.7.1.3"><p id="p46997081181443"><a name="p46997081181443"></a><a name="p46997081181443"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.7.1.4"><p id="p48667239181443"><a name="p48667239181443"></a><a name="p48667239181443"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.7.1.5"><p id="p49732261181443"><a name="p49732261181443"></a><a name="p49732261181443"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="30.606939306069393%" id="mcps1.2.7.1.6"><p id="p1781307181443"><a name="p1781307181443"></a><a name="p1781307181443"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row10068178181443"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.7.1.1 "><p id="p10216081181443"><a name="p10216081181443"></a><a name="p10216081181443"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.2 "><p id="p22196257181443"><a name="p22196257181443"></a><a name="p22196257181443"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="10.1989801019898%" headers="mcps1.2.7.1.3 "><p id="p53066410181443"><a name="p53066410181443"></a><a name="p53066410181443"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.4 "><p id="p3411923181443"><a name="p3411923181443"></a><a name="p3411923181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.5 "><p id="p7930308181443"><a name="p7930308181443"></a><a name="p7930308181443"></a>Ｎ/A</p>
</td>
<td class="cellrowborder" valign="top" width="30.606939306069393%" headers="mcps1.2.7.1.6 "><p id="p38375206181443"><a name="p38375206181443"></a><a name="p38375206181443"></a>外部网络的UUID。</p>
<p id="p21383968181443"><a name="p21383968181443"></a><a name="p21383968181443"></a>外部网络的信息请通过GET /v2.0/networks?router:external=True或neutron net-external-list方式查询。</p>
</td>
</tr>
<tr id="row58237990181443"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.7.1.1 "><p id="p19656760181443"><a name="p19656760181443"></a><a name="p19656760181443"></a>enable_snat</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.2 "><p id="p48693751181443"><a name="p48693751181443"></a><a name="p48693751181443"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="10.1989801019898%" headers="mcps1.2.7.1.3 "><p id="p623311010589"><a name="p623311010589"></a><a name="p623311010589"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.4 "><p id="p41510554181443"><a name="p41510554181443"></a><a name="p41510554181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.5 "><p id="p6911694181443"><a name="p6911694181443"></a><a name="p6911694181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="30.606939306069393%" headers="mcps1.2.7.1.6 "><p id="p22976335181443"><a name="p22976335181443"></a><a name="p22976335181443"></a>是否启用SNAT。</p>
<p id="p49143812181443"><a name="p49143812181443"></a><a name="p49143812181443"></a>默认为false。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  route对象

<a name="table18829650181443"></a>
<table><thead align="left"><tr id="row60542282181443"><th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.7.1.1"><p id="p4977811181443"><a name="p4977811181443"></a><a name="p4977811181443"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.7.1.2"><p id="p549581181443"><a name="p549581181443"></a><a name="p549581181443"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.1989801019898%" id="mcps1.2.7.1.3"><p id="p44516128181443"><a name="p44516128181443"></a><a name="p44516128181443"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.7.1.4"><p id="p49036595181443"><a name="p49036595181443"></a><a name="p49036595181443"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.7.1.5"><p id="p12541230181443"><a name="p12541230181443"></a><a name="p12541230181443"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="30.606939306069393%" id="mcps1.2.7.1.6"><p id="p9206714181443"><a name="p9206714181443"></a><a name="p9206714181443"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7546366181443"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.7.1.1 "><p id="p7275939181443"><a name="p7275939181443"></a><a name="p7275939181443"></a>destination</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.2 "><p id="p52480209181443"><a name="p52480209181443"></a><a name="p52480209181443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.1989801019898%" headers="mcps1.2.7.1.3 "><p id="p23038511181443"><a name="p23038511181443"></a><a name="p23038511181443"></a>RU</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.4 "><p id="p54180069181443"><a name="p54180069181443"></a><a name="p54180069181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.5 "><p id="p26509468181443"><a name="p26509468181443"></a><a name="p26509468181443"></a>前缀不能和直连路由重复</p>
</td>
<td class="cellrowborder" valign="top" width="30.606939306069393%" headers="mcps1.2.7.1.6 "><p id="p66892155181443"><a name="p66892155181443"></a><a name="p66892155181443"></a>IP地址段</p>
</td>
</tr>
<tr id="row65158490181443"><td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.7.1.1 "><p id="p43346313181443"><a name="p43346313181443"></a><a name="p43346313181443"></a>nexthop</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.2 "><p id="p21390453181443"><a name="p21390453181443"></a><a name="p21390453181443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10.1989801019898%" headers="mcps1.2.7.1.3 "><p id="p54905093181443"><a name="p54905093181443"></a><a name="p54905093181443"></a>RU</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.4 "><p id="p18127521181443"><a name="p18127521181443"></a><a name="p18127521181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.7.1.5 "><p id="p59043122181443"><a name="p59043122181443"></a><a name="p59043122181443"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="30.606939306069393%" headers="mcps1.2.7.1.6 "><p id="p17763616181443"><a name="p17763616181443"></a><a name="p17763616181443"></a>下一跳IP地址，nexthop仅支持是router所关联的子网范围内IP地址</p>
</td>
</tr>
</tbody>
</table>

