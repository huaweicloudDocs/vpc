# 查询所有网络ACL规则<a name="ZH-CN_TOPIC_0060574377"></a>

## 功能介绍<a name="section32978392122541"></a>

查询提交请求的租户有权限操作的所有网络ACL规则信息。单次查询最多返回2000条数据，超过2000后会返回分页标记，分页查询请参见[分页查询](分页查询.md)

## URI<a name="section11642292122541"></a>

GET /v2.0/fwaas/firewall\_rules

样例：

```
/v2.0/fwaas/firewall_rules?name={firewall_rule_name}&tenant_id={tenant_id}&public={is_public}&protocol={protocol}&ip_version={ip_version}&action={action}&enabled={is_enabled}
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
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p49072285122541"><a name="p49072285122541"></a><a name="p49072285122541"></a>List(firewall rule)</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p24293772122541"><a name="p24293772122541"></a><a name="p24293772122541"></a>firewall rule对象列表，参见<a href="网络ACL简介-OpenStack.md#table38646929121127">表1</a>。单次查询最多返回2000条数据，超过2000后会返回分页标记，分页查询请参见<a href="分页查询.md">分页查询</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section60841704122541"></a>

请求样例

```
GET /v2.0/fwaas/firewall_rules
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

