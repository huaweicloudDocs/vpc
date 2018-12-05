# 查询特定网络ACL规则<a name="ZH-CN_TOPIC_0060574378"></a>

## 功能介绍<a name="section65879037122957"></a>

查询特定网络ACL规则详情。

## URI<a name="section46813763122957"></a>

GET /v2.0/fwaas/firewall\_rules/\{firewall\_rule\_id\}

**表 1**  参数说明

<a name="table18880184689"></a>
<table><thead align="left"><tr id="row13968641385"><th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.2.5.1.1"><p id="p209684410817"><a name="p209684410817"></a><a name="p209684410817"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.2"><p id="p69681441386"><a name="p69681441386"></a><a name="p69681441386"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="27.27272727272727%" id="mcps1.2.5.1.3"><p id="p1096813412811"><a name="p1096813412811"></a><a name="p1096813412811"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.36363636363636%" id="mcps1.2.5.1.4"><p id="p139686416813"><a name="p139686416813"></a><a name="p139686416813"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19681041189"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1682422682817"><a name="p1682422682817"></a><a name="p1682422682817"></a>firewall_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p1797015416817"><a name="p1797015416817"></a><a name="p1797015416817"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p19701411813"><a name="p19701411813"></a><a name="p19701411813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p158091718125714"><a name="p158091718125714"></a><a name="p158091718125714"></a>网络ACL规则唯一标识，按照firewall_rule_id查询</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section25083919122957"></a>

无。

## 响应消息<a name="section24140738122957"></a>

**表 2**  响应参数

<a name="table22071969122957"></a>
<table><thead align="left"><tr id="row27211568122957"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p41925459122957"><a name="p41925459122957"></a><a name="p41925459122957"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.11%" id="mcps1.2.4.1.2"><p id="p18784029122957"><a name="p18784029122957"></a><a name="p18784029122957"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.540000000000006%" id="mcps1.2.4.1.3"><p id="p64308775122957"><a name="p64308775122957"></a><a name="p64308775122957"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row14692262122957"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p36226380122957"><a name="p36226380122957"></a><a name="p36226380122957"></a>firewall_rule</p>
</td>
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p60366906122957"><a name="p60366906122957"></a><a name="p60366906122957"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p61314665122957"><a name="p61314665122957"></a><a name="p61314665122957"></a>firewall rule对象，参见<a href="网络ACL简介-OpenStack.md#table38646929121127">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section16344236122957"></a>

请求样例

```
GET /v2.0/fwaas/firewall_rules/514e6776-162a-4b5d-ab8b-aa36b86655ef
```

响应样例

```
{
    "firewall_rule": {
        "protocol": "tcp", 
        "name": "bobby_rule", 
        "mode": "normal", 
        "tenant_id": "4490a89232ce46d4ae4bfb227ef1a40a", 
        "rule_profile": "", 
        "enabled": true, 
        "source_port": null, 
        "source_ip_address": null, 
        "destination_ip_address": null, 
        "firewall_policy_id": null, 
        "action": "allow", 
        "position": null, 
        "ip_version": 4, 
        "shared": false, 
        "destination_port": null, 
        "id": "514e6776-162a-4b5d-ab8b-aa36b86655ef", 
        "description": "",
        "project_id": "4490a89232ce46d4ae4bfb227ef1a40a"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

