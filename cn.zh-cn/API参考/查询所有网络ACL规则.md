# 查询所有网络ACL规则<a name="vpc_firewall_0001"></a>

## 功能介绍<a name="section32978392122541"></a>

查询提交请求的租户有权限操作的所有网络ACL规则信息。单次查询最多返回2000条数据，超过2000后会返回分页标记，分页查询请参见[分页查询](分页查询.md)

## URI<a name="section11642292122541"></a>

GET /v2.0/fwaas/firewall\_rules

样例：

```
GET https://{Endpoint}/v2.0/fwaas/firewall_rules?name={firewall_rule_name}&tenant_id={tenant_id}&public={is_public}&protocol={protocol}&ip_version={ip_version}&action={action}&enabled={is_enabled}
```

分页查询样例：

```
GET https://{Endpoint}/v2.0/fwaas/firewall_rules?limit=2&marker=2a193015-4a88-4aa1-84ad-d4955adae707&page_reverse=False
```

参数说明请参见[表1](#table997509428)。

**表 1**  参数说明

<a name="table997509428"></a>
<table><thead align="left"><tr id="row11137135094218"><th class="cellrowborder" valign="top" width="14.72147214721472%" id="mcps1.2.5.1.1"><p id="p91372500429"><a name="p91372500429"></a><a name="p91372500429"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.64216421642164%" id="mcps1.2.5.1.2"><p id="p20137350164218"><a name="p20137350164218"></a><a name="p20137350164218"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.8017801780178%" id="mcps1.2.5.1.3"><p id="p1913719500427"><a name="p1913719500427"></a><a name="p1913719500427"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="45.83458345834583%" id="mcps1.2.5.1.4"><p id="p2137125013423"><a name="p2137125013423"></a><a name="p2137125013423"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row10137165064216"><td class="cellrowborder" valign="top" width="14.72147214721472%" headers="mcps1.2.5.1.1 "><p id="p171379507423"><a name="p171379507423"></a><a name="p171379507423"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="21.64216421642164%" headers="mcps1.2.5.1.2 "><p id="p141378503428"><a name="p141378503428"></a><a name="p141378503428"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.8017801780178%" headers="mcps1.2.5.1.3 "><p id="p5137450184219"><a name="p5137450184219"></a><a name="p5137450184219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.83458345834583%" headers="mcps1.2.5.1.4 "><p id="p1013785017424"><a name="p1013785017424"></a><a name="p1013785017424"></a>按照网络ACL规则对应的ID过滤查询</p>
</td>
</tr>
<tr id="row313725054217"><td class="cellrowborder" valign="top" width="14.72147214721472%" headers="mcps1.2.5.1.1 "><p id="p8137135074211"><a name="p8137135074211"></a><a name="p8137135074211"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="21.64216421642164%" headers="mcps1.2.5.1.2 "><p id="p14137175064212"><a name="p14137175064212"></a><a name="p14137175064212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.8017801780178%" headers="mcps1.2.5.1.3 "><p id="p171372050114214"><a name="p171372050114214"></a><a name="p171372050114214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.83458345834583%" headers="mcps1.2.5.1.4 "><p id="p141374506425"><a name="p141374506425"></a><a name="p141374506425"></a>按照网络ACL规则的名称过滤查询</p>
</td>
</tr>
<tr id="row1813745044211"><td class="cellrowborder" valign="top" width="14.72147214721472%" headers="mcps1.2.5.1.1 "><p id="p9137175094217"><a name="p9137175094217"></a><a name="p9137175094217"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="21.64216421642164%" headers="mcps1.2.5.1.2 "><p id="p18137175015420"><a name="p18137175015420"></a><a name="p18137175015420"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.8017801780178%" headers="mcps1.2.5.1.3 "><p id="p213715024219"><a name="p213715024219"></a><a name="p213715024219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.83458345834583%" headers="mcps1.2.5.1.4 "><p id="p1913775016422"><a name="p1913775016422"></a><a name="p1913775016422"></a>按照网络ACL规则的描述过滤查询</p>
</td>
</tr>
<tr id="row61371650194212"><td class="cellrowborder" valign="top" width="14.72147214721472%" headers="mcps1.2.5.1.1 "><p id="p1213825054216"><a name="p1213825054216"></a><a name="p1213825054216"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="21.64216421642164%" headers="mcps1.2.5.1.2 "><p id="p313815504428"><a name="p313815504428"></a><a name="p313815504428"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.8017801780178%" headers="mcps1.2.5.1.3 "><p id="p7138165014214"><a name="p7138165014214"></a><a name="p7138165014214"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="45.83458345834583%" headers="mcps1.2.5.1.4 "><p id="p5526124316"><a name="p5526124316"></a><a name="p5526124316"></a>按照网络ACL规则的IP协议版本过滤查询</p>
<p id="p121381950174212"><a name="p121381950174212"></a><a name="p121381950174212"></a>取值范围：4</p>
</td>
</tr>
<tr id="row12138195084219"><td class="cellrowborder" valign="top" width="14.72147214721472%" headers="mcps1.2.5.1.1 "><p id="p161385503424"><a name="p161385503424"></a><a name="p161385503424"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="21.64216421642164%" headers="mcps1.2.5.1.2 "><p id="p313855094219"><a name="p313855094219"></a><a name="p313855094219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.8017801780178%" headers="mcps1.2.5.1.3 "><p id="p13138145015423"><a name="p13138145015423"></a><a name="p13138145015423"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.83458345834583%" headers="mcps1.2.5.1.4 "><p id="p167111932438"><a name="p167111932438"></a><a name="p167111932438"></a>按照网络ACL规则的行为过滤查询</p>
<p id="p13138135016424"><a name="p13138135016424"></a><a name="p13138135016424"></a>取值范围：allow or deny</p>
</td>
</tr>
<tr id="row131381450164218"><td class="cellrowborder" valign="top" width="14.72147214721472%" headers="mcps1.2.5.1.1 "><p id="p1713811507429"><a name="p1713811507429"></a><a name="p1713811507429"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="21.64216421642164%" headers="mcps1.2.5.1.2 "><p id="p13138145094212"><a name="p13138145094212"></a><a name="p13138145094212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.8017801780178%" headers="mcps1.2.5.1.3 "><p id="p17138350194215"><a name="p17138350194215"></a><a name="p17138350194215"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="45.83458345834583%" headers="mcps1.2.5.1.4 "><p id="p1564520515432"><a name="p1564520515432"></a><a name="p1564520515432"></a>按照网络ACL规则是否使能过滤查询</p>
<p id="p513820509425"><a name="p513820509425"></a><a name="p513820509425"></a>取值范围：true or false</p>
</td>
</tr>
<tr id="row9138450124210"><td class="cellrowborder" valign="top" width="14.72147214721472%" headers="mcps1.2.5.1.1 "><p id="p1138145015421"><a name="p1138145015421"></a><a name="p1138145015421"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.64216421642164%" headers="mcps1.2.5.1.2 "><p id="p713855094216"><a name="p713855094216"></a><a name="p713855094216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.8017801780178%" headers="mcps1.2.5.1.3 "><p id="p2138155019429"><a name="p2138155019429"></a><a name="p2138155019429"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.83458345834583%" headers="mcps1.2.5.1.4 "><p id="p61381650184213"><a name="p61381650184213"></a><a name="p61381650184213"></a>按照安全组所属的项目ID过滤查询</p>
</td>
</tr>
<tr id="row013818506422"><td class="cellrowborder" valign="top" width="14.72147214721472%" headers="mcps1.2.5.1.1 "><p id="p613817506423"><a name="p613817506423"></a><a name="p613817506423"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="21.64216421642164%" headers="mcps1.2.5.1.2 "><p id="p1513817501420"><a name="p1513817501420"></a><a name="p1513817501420"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.8017801780178%" headers="mcps1.2.5.1.3 "><p id="p14138450134211"><a name="p14138450134211"></a><a name="p14138450134211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.83458345834583%" headers="mcps1.2.5.1.4 "><p id="p15138165064212"><a name="p15138165064212"></a><a name="p15138165064212"></a>分页查询起始的资源ID，为空时为查询第一页</p>
</td>
</tr>
<tr id="row813815500428"><td class="cellrowborder" valign="top" width="14.72147214721472%" headers="mcps1.2.5.1.1 "><p id="p813825014428"><a name="p813825014428"></a><a name="p813825014428"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="21.64216421642164%" headers="mcps1.2.5.1.2 "><p id="p5138155015425"><a name="p5138155015425"></a><a name="p5138155015425"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.8017801780178%" headers="mcps1.2.5.1.3 "><p id="p41381750124216"><a name="p41381750124216"></a><a name="p41381750124216"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="45.83458345834583%" headers="mcps1.2.5.1.4 "><p id="p491518711431"><a name="p491518711431"></a><a name="p491518711431"></a>每页返回的个数</p>
<p id="p161381350114216"><a name="p161381350114216"></a><a name="p161381350114216"></a>取值范围：0~intmax</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section16626865122541"></a>

无。

## 响应消息<a name="section39494421122541"></a>

**表 2**  响应参数

<a name="table48261844122541"></a>
<table><thead align="left"><tr id="row41263599122541"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p23207162122541"><a name="p23207162122541"></a><a name="p23207162122541"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.11%" id="mcps1.2.4.1.2"><p id="p46617019122541"><a name="p46617019122541"></a><a name="p46617019122541"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.540000000000006%" id="mcps1.2.4.1.3"><p id="p38363364122541"><a name="p38363364122541"></a><a name="p38363364122541"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row34200971122541"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p34822248122541"><a name="p34822248122541"></a><a name="p34822248122541"></a>firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p125656569422"><a name="p125656569422"></a><a name="p125656569422"></a>Array of <a href="#table38646929121127">Firewall Rule</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p24293772122541"><a name="p24293772122541"></a><a name="p24293772122541"></a>firewall rule对象列表，参见<a href="#table38646929121127">表4</a>。单次查询最多返回2000条数据，超过2000后会返回分页标记，分页查询请参见<a href="分页查询.md">分页查询</a>。</p>
</td>
</tr>
<tr id="row431543194812"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p121201423154911"><a name="p121201423154911"></a><a name="p121201423154911"></a>firewall_rules_links</p>
</td>
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p1412092384917"><a name="p1412092384917"></a><a name="p1412092384917"></a>Array of <a href="#table2049004519490">firewall_rules_link</a> Object</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p16120623194914"><a name="p16120623194914"></a><a name="p16120623194914"></a>分页信息，参见<a href="#table2049004519490">表3</a> 。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  firewall\_rules\_link对象

<a name="table2049004519490"></a>
<table><thead align="left"><tr id="row13534124514917"><th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.1"><p id="p753404514915"><a name="p753404514915"></a><a name="p753404514915"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.2"><p id="p25341945124920"><a name="p25341945124920"></a><a name="p25341945124920"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="71.72%" id="mcps1.2.4.1.3"><p id="p7534194512494"><a name="p7534194512494"></a><a name="p7534194512494"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13534164554911"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p1534184524920"><a name="p1534184524920"></a><a name="p1534184524920"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p753415454494"><a name="p753415454494"></a><a name="p753415454494"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p125340459499"><a name="p125340459499"></a><a name="p125340459499"></a>API链接</p>
</td>
</tr>
<tr id="row8534104512493"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p10534745114919"><a name="p10534745114919"></a><a name="p10534745114919"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p13534164534911"><a name="p13534164534911"></a><a name="p13534164534911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p16534164584910"><a name="p16534164584910"></a><a name="p16534164584910"></a>API链接与该API版本的关系</p>
</td>
</tr>
</tbody>
</table>

**表 4**  Firewall Rule对象

<a name="table38646929121127"></a>
<table><thead align="left"><tr id="row18263398121127"><th class="cellrowborder" valign="top" width="32.76%" id="mcps1.2.4.1.1"><p id="p2027461121127"><a name="p2027461121127"></a><a name="p2027461121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="20.69%" id="mcps1.2.4.1.2"><p id="p51747644121127"><a name="p51747644121127"></a><a name="p51747644121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="46.550000000000004%" id="mcps1.2.4.1.3"><p id="p12805757121127"><a name="p12805757121127"></a><a name="p12805757121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row39528007121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p7362024121127"><a name="p7362024121127"></a><a name="p7362024121127"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p53278848121127"><a name="p53278848121127"></a><a name="p53278848121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p13095685121127"><a name="p13095685121127"></a><a name="p13095685121127"></a>网络ACL规则的uuid标识。</p>
</td>
</tr>
<tr id="row3417421121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p16296528121127"><a name="p16296528121127"></a><a name="p16296528121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p52887833121127"><a name="p52887833121127"></a><a name="p52887833121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p29399172121127"><a name="p29399172121127"></a><a name="p29399172121127"></a>网络ACL规则名称。</p>
</td>
</tr>
<tr id="row33772147121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p62102623121127"><a name="p62102623121127"></a><a name="p62102623121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p30062050121127"><a name="p30062050121127"></a><a name="p30062050121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p64485971121127"><a name="p64485971121127"></a><a name="p64485971121127"></a>网络ACL规则描述。</p>
</td>
</tr>
<tr id="row39157453121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p40485546121127"><a name="p40485546121127"></a><a name="p40485546121127"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p20366062121127"><a name="p20366062121127"></a><a name="p20366062121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row13612334121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p3945861121127"><a name="p3945861121127"></a><a name="p3945861121127"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p53059091121127"><a name="p53059091121127"></a><a name="p53059091121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p46007536121127"><a name="p46007536121127"></a><a name="p46007536121127"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row66347377121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p7361769121127"><a name="p7361769121127"></a><a name="p7361769121127"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p50019959121127"><a name="p50019959121127"></a><a name="p50019959121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p36897817121127"><a name="p36897817121127"></a><a name="p36897817121127"></a>IP协议。</p>
</td>
</tr>
<tr id="row8703753121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p5943474121127"><a name="p5943474121127"></a><a name="p5943474121127"></a>source_port</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p59206978121127"><a name="p59206978121127"></a><a name="p59206978121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p62826249121127"><a name="p62826249121127"></a><a name="p62826249121127"></a>源端口号或者一段端口范围。</p>
</td>
</tr>
<tr id="row52935496121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p12876203121127"><a name="p12876203121127"></a><a name="p12876203121127"></a>destination_port</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p66631365121127"><a name="p66631365121127"></a><a name="p66631365121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p66851026121127"><a name="p66851026121127"></a><a name="p66851026121127"></a>目的端口号或者一段端口范围。</p>
</td>
</tr>
<tr id="row37973187121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p18090983121127"><a name="p18090983121127"></a><a name="p18090983121127"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p15064211121127"><a name="p15064211121127"></a><a name="p15064211121127"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p10402054121127"><a name="p10402054121127"></a><a name="p10402054121127"></a>IP协议版本。</p>
</td>
</tr>
<tr id="row34581454121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p61377852121127"><a name="p61377852121127"></a><a name="p61377852121127"></a>source_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p36483585121127"><a name="p36483585121127"></a><a name="p36483585121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p31475962121127"><a name="p31475962121127"></a><a name="p31475962121127"></a>源地址或者CIDR。</p>
</td>
</tr>
<tr id="row13949121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p43901244121127"><a name="p43901244121127"></a><a name="p43901244121127"></a>destination_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p14651426121127"><a name="p14651426121127"></a><a name="p14651426121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p53743554121127"><a name="p53743554121127"></a><a name="p53743554121127"></a>目的地址或者CIDR。</p>
</td>
</tr>
<tr id="row33223843121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p40131900121127"><a name="p40131900121127"></a><a name="p40131900121127"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p952780121127"><a name="p952780121127"></a><a name="p952780121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p16135729121127"><a name="p16135729121127"></a><a name="p16135729121127"></a>对通过网络ACL的流量执行的操作。</p>
</td>
</tr>
<tr id="row11398101121127"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p50347088121127"><a name="p50347088121127"></a><a name="p50347088121127"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p46161809121127"><a name="p46161809121127"></a><a name="p46161809121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p57324252121127"><a name="p57324252121127"></a><a name="p57324252121127"></a>是否使能网络ACL规则。</p>
</td>
</tr>
<tr id="row1574912215580"><td class="cellrowborder" valign="top" width="32.76%" headers="mcps1.2.4.1.1 "><p id="p1312116475819"><a name="p1312116475819"></a><a name="p1312116475819"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.69%" headers="mcps1.2.4.1.2 "><p id="p5125543583"><a name="p5125543583"></a><a name="p5125543583"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p187677200286"><a name="p187677200286"></a><a name="p187677200286"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section60841704122541"></a>

请求样例

```
GET https://{Endpoint}/v2.0/fwaas/firewall_rules
```

响应样例

```
{
    "firewall_rules": [
        {
            "protocol": "tcp", 
            "name": "crhfwruleupdate", 
            "mode": "normal", 
            "tenant_id": "f480f5d250824e5fafedcf05acf1419c", 
            "rule_profile": "", 
            "enabled": true, 
            "source_port": null, 
            "source_ip_address": null, 
            "destination_ip_address": null, 
            "firewall_policy_id": "b4f81251-c47a-4fe1-8579-6f9271d015d1", 
            "action": "deny", 
            "position": 1, 
            "ip_version": 4, 
            "shared": false, 
            "destination_port": null, 
            "id": "2a193015-4a88-4aa1-84ad-d4955adae707", 
            "description": "",
            "project_id": "f480f5d250824e5fafedcf05acf1419c"
        }, 
        {
            "protocol": "tcp", 
            "name": "update_firewall-role-tommy", 
            "mode": "mix", 
            "tenant_id": "a1c6f90c94334bd2953d9a61b8031a68", 
            "rule_profile": "", 
            "enabled": false, 
            "source_port": "20:50", 
            "source_ip_address": null, 
            "destination_ip_address": null, 
            "firewall_policy_id": null, 
            "action": "deny", 
            "position": null, 
            "ip_version": 4, 
            "shared": true, 
            "destination_port": "40:60", 
            "id": "db7a204c-9eb1-40a2-9bd6-ed5cfd3cff32", 
            "description": "update check parameter",
            "project_id": "a1c6f90c94334bd2953d9a61b8031a68"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

