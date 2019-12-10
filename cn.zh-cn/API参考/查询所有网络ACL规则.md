# 查询所有网络ACL规则<a name="ZH-CN_TOPIC_0201534200"></a>

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

## 请求消息<a name="section16626865122541"></a>

无。

## 响应消息<a name="section39494421122541"></a>

**表 1**  响应参数

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
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p24293772122541"><a name="p24293772122541"></a><a name="p24293772122541"></a>firewall rule对象列表，参见<a href="#table38646929121127">表2</a>。单次查询最多返回2000条数据，超过2000后会返回分页标记，分页查询请参见<a href="分页查询.md">分页查询</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Firewall Rule对象

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
<td class="cellrowborder" valign="top" width="46.550000000000004%" headers="mcps1.2.4.1.3 "><p id="p187677200286"><a name="p187677200286"></a><a name="p187677200286"></a>项目ID</p>
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

