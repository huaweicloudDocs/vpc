# 安全组API简介<a name="ZH-CN_TOPIC_0060595063"></a>

## 对象简介<a name="section218654311607"></a>

对安全组和规则资源进行管理和操作，包括查询安全组和规则列表、创建安全组和规则、查询安全组和规则、删除安全组和规则以及更新安全组等接口。

## 对象模型<a name="section104214421607"></a>

**表 1**  Security Group对象

<a name="table513726041607"></a>
<table><thead align="left"><tr id="row72893461607"><th class="cellrowborder" valign="top" width="15.101510151015102%" id="mcps1.2.8.1.1"><p id="p647825491607"><a name="p647825491607"></a><a name="p647825491607"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="7.520752075207521%" id="mcps1.2.8.1.2"><p id="p1075015422371"><a name="p1075015422371"></a><a name="p1075015422371"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.211321132113211%" id="mcps1.2.8.1.3"><p id="p245230881607"><a name="p245230881607"></a><a name="p245230881607"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.43094309430943%" id="mcps1.2.8.1.4"><p id="p53546411607"><a name="p53546411607"></a><a name="p53546411607"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="13.211321132113211%" id="mcps1.2.8.1.5"><p id="p565943611607"><a name="p565943611607"></a><a name="p565943611607"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="13.211321132113211%" id="mcps1.2.8.1.6"><p id="p251586331607"><a name="p251586331607"></a><a name="p251586331607"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="28.312831283128315%" id="mcps1.2.8.1.7"><p id="p4542071607"><a name="p4542071607"></a><a name="p4542071607"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row284118681607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p6322881607"><a name="p6322881607"></a><a name="p6322881607"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p8750342123719"><a name="p8750342123719"></a><a name="p8750342123719"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p206339641607"><a name="p206339641607"></a><a name="p206339641607"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p56892461607"><a name="p56892461607"></a><a name="p56892461607"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p341979111607"><a name="p341979111607"></a><a name="p341979111607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p628665521607"><a name="p628665521607"></a><a name="p628665521607"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p538811831607"><a name="p538811831607"></a><a name="p538811831607"></a>安全组的id</p>
<p id="p7631141813810"><a name="p7631141813810"></a><a name="p7631141813810"></a>【使用说明】查询安全组列表非必选</p>
</td>
</tr>
<tr id="row487759591607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p499705331607"><a name="p499705331607"></a><a name="p499705331607"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p67501642163712"><a name="p67501642163712"></a><a name="p67501642163712"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p26621541607"><a name="p26621541607"></a><a name="p26621541607"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p359616371607"><a name="p359616371607"></a><a name="p359616371607"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p353077361607"><a name="p353077361607"></a><a name="p353077361607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p71422101607"><a name="p71422101607"></a><a name="p71422101607"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p650489631607"><a name="p650489631607"></a><a name="p650489631607"></a>项目ID。</p>
</td>
</tr>
<tr id="row356666781607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p270644691607"><a name="p270644691607"></a><a name="p270644691607"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p87501142163712"><a name="p87501142163712"></a><a name="p87501142163712"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p426717071607"><a name="p426717071607"></a><a name="p426717071607"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p181712411607"><a name="p181712411607"></a><a name="p181712411607"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p332356771607"><a name="p332356771607"></a><a name="p332356771607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p570183281607"><a name="p570183281607"></a><a name="p570183281607"></a>创建，更新name参数不能为default</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p29740751607"><a name="p29740751607"></a><a name="p29740751607"></a>安全组名称</p>
</td>
</tr>
<tr id="row5261561607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p76095411607"><a name="p76095411607"></a><a name="p76095411607"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p11750124243714"><a name="p11750124243714"></a><a name="p11750124243714"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p597100051607"><a name="p597100051607"></a><a name="p597100051607"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p132543321607"><a name="p132543321607"></a><a name="p132543321607"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p631207611607"><a name="p631207611607"></a><a name="p631207611607"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p115521421607"><a name="p115521421607"></a><a name="p115521421607"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p40269061607"><a name="p40269061607"></a><a name="p40269061607"></a>安全组描述</p>
<p id="p523872461607"><a name="p523872461607"></a><a name="p523872461607"></a></p>
</td>
</tr>
<tr id="row141788771607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p574773991607"><a name="p574773991607"></a><a name="p574773991607"></a>security_group_rules</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p475034216371"><a name="p475034216371"></a><a name="p475034216371"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p263715271607"><a name="p263715271607"></a><a name="p263715271607"></a>List(security_group_rule)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p528679511607"><a name="p528679511607"></a><a name="p528679511607"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p228109261607"><a name="p228109261607"></a><a name="p228109261607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p202491241607"><a name="p202491241607"></a><a name="p202491241607"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p577222241607"><a name="p577222241607"></a><a name="p577222241607"></a>security_group_rule列表，参见<a href="#ZH-CN_TOPIC_0060595063__table655457801607">表2</a>。</p>
</td>
</tr>
<tr id="row19560720141817"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
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
<tr id="row5768162761818"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
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
<tr id="row4242824111816"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
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

**表 2**  Security Group Rule对象

<a name="table655457801607"></a>
<table><thead align="left"><tr id="row54478641607"><th class="cellrowborder" valign="top" width="15.101510151015102%" id="mcps1.2.8.1.1"><p id="p389969021607"><a name="p389969021607"></a><a name="p389969021607"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="7.520752075207521%" id="mcps1.2.8.1.2"><p id="p07415175392"><a name="p07415175392"></a><a name="p07415175392"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.211321132113211%" id="mcps1.2.8.1.3"><p id="p36789391607"><a name="p36789391607"></a><a name="p36789391607"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.43094309430943%" id="mcps1.2.8.1.4"><p id="p1790641607"><a name="p1790641607"></a><a name="p1790641607"></a>CRUD</p>
</th>
<th class="cellrowborder" valign="top" width="13.211321132113211%" id="mcps1.2.8.1.5"><p id="p47694351607"><a name="p47694351607"></a><a name="p47694351607"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="13.211321132113211%" id="mcps1.2.8.1.6"><p id="p331820531607"><a name="p331820531607"></a><a name="p331820531607"></a>约束</p>
</th>
<th class="cellrowborder" valign="top" width="28.312831283128315%" id="mcps1.2.8.1.7"><p id="p433861031607"><a name="p433861031607"></a><a name="p433861031607"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row134774871607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p269083981607"><a name="p269083981607"></a><a name="p269083981607"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p12741217173916"><a name="p12741217173916"></a><a name="p12741217173916"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p630670281607"><a name="p630670281607"></a><a name="p630670281607"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p636327701607"><a name="p636327701607"></a><a name="p636327701607"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p398258781607"><a name="p398258781607"></a><a name="p398258781607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p527794411607"><a name="p527794411607"></a><a name="p527794411607"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p334792201607"><a name="p334792201607"></a><a name="p334792201607"></a>安全组规则id</p>
<p id="p529374054010"><a name="p529374054010"></a><a name="p529374054010"></a>【使用说明】查询安全组规则非必选</p>
</td>
</tr>
<tr id="row250554771607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p254411021607"><a name="p254411021607"></a><a name="p254411021607"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p27411717193910"><a name="p27411717193910"></a><a name="p27411717193910"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p505368621607"><a name="p505368621607"></a><a name="p505368621607"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p534679091607"><a name="p534679091607"></a><a name="p534679091607"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p332581461607"><a name="p332581461607"></a><a name="p332581461607"></a>空</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p83864551607"><a name="p83864551607"></a><a name="p83864551607"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p480145951607"><a name="p480145951607"></a><a name="p480145951607"></a>安全组规则描述</p>
</td>
</tr>
<tr id="row569401671607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p115724181607"><a name="p115724181607"></a><a name="p115724181607"></a>security_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p10741111717399"><a name="p10741111717399"></a><a name="p10741111717399"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p615991711607"><a name="p615991711607"></a><a name="p615991711607"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p439354031607"><a name="p439354031607"></a><a name="p439354031607"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p481773071607"><a name="p481773071607"></a><a name="p481773071607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p561870571607"><a name="p561870571607"></a><a name="p561870571607"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p587796621607"><a name="p587796621607"></a><a name="p587796621607"></a>所属安全组id</p>
</td>
</tr>
<tr id="row654332091607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p113008931607"><a name="p113008931607"></a><a name="p113008931607"></a>remote_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p374111793919"><a name="p374111793919"></a><a name="p374111793919"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p170542961607"><a name="p170542961607"></a><a name="p170542961607"></a>Uuid-str</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p651571941607"><a name="p651571941607"></a><a name="p651571941607"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p436267711607"><a name="p436267711607"></a><a name="p436267711607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p666684981607"><a name="p666684981607"></a><a name="p666684981607"></a>和remote_ip_prefix参数二选一</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p141218971607"><a name="p141218971607"></a><a name="p141218971607"></a>所属安全组的对端id</p>
<p id="p522705591607"><a name="p522705591607"></a><a name="p522705591607"></a></p>
</td>
</tr>
<tr id="row9932071607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p657989401607"><a name="p657989401607"></a><a name="p657989401607"></a>direction</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p19741111723910"><a name="p19741111723910"></a><a name="p19741111723910"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p507988391607"><a name="p507988391607"></a><a name="p507988391607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p432170021607"><a name="p432170021607"></a><a name="p432170021607"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p17194441607"><a name="p17194441607"></a><a name="p17194441607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p109886931607"><a name="p109886931607"></a><a name="p109886931607"></a>ingress/egress</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p570991491607"><a name="p570991491607"></a><a name="p570991491607"></a>规则方向</p>
</td>
</tr>
<tr id="row97529031607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p478834691607"><a name="p478834691607"></a><a name="p478834691607"></a>remote_ip_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p1574110175393"><a name="p1574110175393"></a><a name="p1574110175393"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p622759951607"><a name="p622759951607"></a><a name="p622759951607"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p292528151607"><a name="p292528151607"></a><a name="p292528151607"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p12634981607"><a name="p12634981607"></a><a name="p12634981607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p274879811607"><a name="p274879811607"></a><a name="p274879811607"></a>cidr格式。和remote_group_id参数二选一</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p146708701607"><a name="p146708701607"></a><a name="p146708701607"></a>对端ip网段</p>
<p id="p471956071607"><a name="p471956071607"></a><a name="p471956071607"></a></p>
</td>
</tr>
<tr id="row315033981607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p163656291607"><a name="p163656291607"></a><a name="p163656291607"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p07411217183920"><a name="p07411217183920"></a><a name="p07411217183920"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p628340441607"><a name="p628340441607"></a><a name="p628340441607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p414405131607"><a name="p414405131607"></a><a name="p414405131607"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p5232451607"><a name="p5232451607"></a><a name="p5232451607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p375468481607"><a name="p375468481607"></a><a name="p375468481607"></a>tcp/udp/icmp或IP协议号</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p99902671607"><a name="p99902671607"></a><a name="p99902671607"></a>协议类型或直接指定IP协议号</p>
</td>
</tr>
<tr id="row551583771607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p97886331607"><a name="p97886331607"></a><a name="p97886331607"></a>port_range_max</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p8741717103914"><a name="p8741717103914"></a><a name="p8741717103914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p343603851607"><a name="p343603851607"></a><a name="p343603851607"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p571196801607"><a name="p571196801607"></a><a name="p571196801607"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p220647581607"><a name="p220647581607"></a><a name="p220647581607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p218858261607"><a name="p218858261607"></a><a name="p218858261607"></a>范围：1-65535（当表示code时是0-255）</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p188144701607"><a name="p188144701607"></a><a name="p188144701607"></a>最大端口，当协议类型为ICMP时，该值表示ICMP的code</p>
</td>
</tr>
<tr id="row456604071607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p630384091607"><a name="p630384091607"></a><a name="p630384091607"></a>port_range_min</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p137411517143913"><a name="p137411517143913"></a><a name="p137411517143913"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p337362901607"><a name="p337362901607"></a><a name="p337362901607"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p68991711607"><a name="p68991711607"></a><a name="p68991711607"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p486859301607"><a name="p486859301607"></a><a name="p486859301607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p412375281607"><a name="p412375281607"></a><a name="p412375281607"></a>范围：1-65535（当表示type时是0-255)</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p258562691607"><a name="p258562691607"></a><a name="p258562691607"></a>最小端口，当协议类型为ICMP时，该值表示ICMP的type。</p>
<p id="p5690808615417"><a name="p5690808615417"></a><a name="p5690808615417"></a>protocol为tcp和udp时，port_range_max和port_range_min必须同时输入，且port_range_max应大于等于port_range_min。</p>
<p id="p4241072615417"><a name="p4241072615417"></a><a name="p4241072615417"></a>protocol为icmp时，指定ICMP code（port_range_max）时，必须同时指定ICMP type（port_range_min）。</p>
</td>
</tr>
<tr id="row360773491607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p364292801607"><a name="p364292801607"></a><a name="p364292801607"></a>ethertype</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p15741131719393"><a name="p15741131719393"></a><a name="p15741131719393"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p339523071607"><a name="p339523071607"></a><a name="p339523071607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p137562211607"><a name="p137562211607"></a><a name="p137562211607"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p292956461607"><a name="p292956461607"></a><a name="p292956461607"></a>IPv4</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p112998301607"><a name="p112998301607"></a><a name="p112998301607"></a>IPv4/IPv6</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p34728681607"><a name="p34728681607"></a><a name="p34728681607"></a>网络类型</p>
<p id="p568898621607"><a name="p568898621607"></a><a name="p568898621607"></a>仅支持IPv4</p>
</td>
</tr>
<tr id="row532124261607"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p593368391607"><a name="p593368391607"></a><a name="p593368391607"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p27416179397"><a name="p27416179397"></a><a name="p27416179397"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p130282191607"><a name="p130282191607"></a><a name="p130282191607"></a>String(255)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p615662141607"><a name="p615662141607"></a><a name="p615662141607"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p257536711607"><a name="p257536711607"></a><a name="p257536711607"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p152013761607"><a name="p152013761607"></a><a name="p152013761607"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p275426401607"><a name="p275426401607"></a><a name="p275426401607"></a>项目ID。</p>
</td>
</tr>
<tr id="row11992111863317"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p169261732143314"><a name="p169261732143314"></a><a name="p169261732143314"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p129291132143318"><a name="p129291132143318"></a><a name="p129291132143318"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p69311132153317"><a name="p69311132153317"></a><a name="p69311132153317"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p159341332163311"><a name="p159341332163311"></a><a name="p159341332163311"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p59361732163314"><a name="p59361732163314"></a><a name="p59361732163314"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p1993923215336"><a name="p1993923215336"></a><a name="p1993923215336"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p994112324333"><a name="p994112324333"></a><a name="p994112324333"></a>资源project_id</p>
</td>
</tr>
<tr id="row10903153923318"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p6634195714335"><a name="p6634195714335"></a><a name="p6634195714335"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p196371257193310"><a name="p196371257193310"></a><a name="p196371257193310"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p12638157153319"><a name="p12638157153319"></a><a name="p12638157153319"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p1264010571332"><a name="p1264010571332"></a><a name="p1264010571332"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p16641205710337"><a name="p16641205710337"></a><a name="p16641205710337"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p2064315783319"><a name="p2064315783319"></a><a name="p2064315783319"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p1364635713332"><a name="p1364635713332"></a><a name="p1364635713332"></a>资源创建时间</p>
</td>
</tr>
<tr id="row1797311427338"><td class="cellrowborder" valign="top" width="15.101510151015102%" headers="mcps1.2.8.1.1 "><p id="p1725445103416"><a name="p1725445103416"></a><a name="p1725445103416"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="7.520752075207521%" headers="mcps1.2.8.1.2 "><p id="p12257052343"><a name="p12257052343"></a><a name="p12257052343"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.3 "><p id="p192601514345"><a name="p192601514345"></a><a name="p192601514345"></a>String(64)</p>
</td>
<td class="cellrowborder" valign="top" width="9.43094309430943%" headers="mcps1.2.8.1.4 "><p id="p112625511347"><a name="p112625511347"></a><a name="p112625511347"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.5 "><p id="p192653512342"><a name="p192653512342"></a><a name="p192653512342"></a>自动生成</p>
</td>
<td class="cellrowborder" valign="top" width="13.211321132113211%" headers="mcps1.2.8.1.6 "><p id="p1126755123418"><a name="p1126755123418"></a><a name="p1126755123418"></a>N/A</p>
</td>
<td class="cellrowborder" valign="top" width="28.312831283128315%" headers="mcps1.2.8.1.7 "><p id="p1127018513343"><a name="p1127018513343"></a><a name="p1127018513343"></a>资源更新时间</p>
</td>
</tr>
</tbody>
</table>

