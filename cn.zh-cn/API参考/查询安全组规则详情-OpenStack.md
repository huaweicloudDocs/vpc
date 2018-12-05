# 查询安全组规则详情<a name="ZH-CN_TOPIC_0060595557"></a>

## 功能介绍<a name="section241393816235"></a>

查询安全组规则详情。

## URI<a name="section4708630216235"></a>

GET /v2.0/security-group-rules/\{security\_groups\_rules\_id\}

## 请求消息<a name="section1121883416235"></a>

无。

## 响应消息<a name="section2503267016235"></a>

**表 1**  响应参数

<a name="table265337716235"></a>
<table><thead align="left"><tr id="row4122992216235"><th class="cellrowborder" valign="top" width="34.14658534146586%" id="mcps1.2.4.1.1"><p id="p6294639916235"><a name="p6294639916235"></a><a name="p6294639916235"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.628537146285373%" id="mcps1.2.4.1.2"><p id="p6682514016235"><a name="p6682514016235"></a><a name="p6682514016235"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22487751224878%" id="mcps1.2.4.1.3"><p id="p1721315516235"><a name="p1721315516235"></a><a name="p1721315516235"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1324978916235"><td class="cellrowborder" valign="top" width="34.14658534146586%" headers="mcps1.2.4.1.1 "><p id="p510999716235"><a name="p510999716235"></a><a name="p510999716235"></a>security_group_rule</p>
</td>
<td class="cellrowborder" valign="top" width="14.628537146285373%" headers="mcps1.2.4.1.2 "><p id="p1974626116235"><a name="p1974626116235"></a><a name="p1974626116235"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22487751224878%" headers="mcps1.2.4.1.3 "><p id="p4059418616235"><a name="p4059418616235"></a><a name="p4059418616235"></a>security_group_rule对象列表，参见<a href="安全组API简介-OpenStack.md#table655457801607">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section2374028316235"></a>

请求样例

```
GET /v2.0/security-group-rules/1755bc80-cf3a-4f57-8ae9-d9796482ddc0
```

响应样例

```
{
    "security_group_rule": {
        "remote_group_id": null, 
        "direction": "egress", 
        "remote_ip_prefix": null, 
        "protocol": null, 
        "tenant_id": "6fbe9263116a4b68818cf1edce16bc4f", 
        "port_range_max": null, 
        "security_group_id": "723bc02c-d7f7-49b5-b6ff-d08320f315e2", 
        "port_range_min": null, 
        "ethertype": "IPv4", 
        "description": null, 
        "id": "1755bc80-cf3a-4f57-8ae9-d9796482ddc0",
        "project_id": "6fbe9263116a4b68818cf1edce16bc4f", 
        "created_at": "2018-09-20T02:15:34",
        "updated_at": "2018-09-20T02:15:34"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

