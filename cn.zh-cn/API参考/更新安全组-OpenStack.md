# 更新安全组<a name="ZH-CN_TOPIC_0060595534"></a>

## 功能介绍<a name="section3331610616137"></a>

更新安全组。

## URI<a name="section1957098316137"></a>

PUT /v2.0/security-groups/\{security\_group\_id\}

## 请求消息<a name="section1781687316137"></a>

**表 1**  请求参数

<a name="table460557116137"></a>
<table><thead align="left"><tr id="row1322435616137"><th class="cellrowborder" valign="top" width="14.430000000000001%" id="mcps1.2.5.1.1"><p id="p1590492916137"><a name="p1590492916137"></a><a name="p1590492916137"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.2"><p id="p1862451716137"><a name="p1862451716137"></a><a name="p1862451716137"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.3"><p id="p4976459316137"><a name="p4976459316137"></a><a name="p4976459316137"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="69.07%" id="mcps1.2.5.1.4"><p id="p5736665916137"><a name="p5736665916137"></a><a name="p5736665916137"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2162479616137"><td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.1 "><p id="p4116380516137"><a name="p4116380516137"></a><a name="p4116380516137"></a>security_group</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.2 "><p id="p2400419616137"><a name="p2400419616137"></a><a name="p2400419616137"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.3 "><p id="p2340142616137"><a name="p2340142616137"></a><a name="p2340142616137"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="69.07%" headers="mcps1.2.5.1.4 "><p id="p4415424716137"><a name="p4415424716137"></a><a name="p4415424716137"></a>security_group对象列表，参见<a href="安全组API简介-OpenStack.md#table513726041607">表1</a>。</p>
<p id="p2337407916137"><a name="p2337407916137"></a><a name="p2337407916137"></a>必选字段：无，更新操作时至少指定一项属性</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section3049893816137"></a>

**表 2**  响应参数

<a name="table821390116137"></a>
<table><thead align="left"><tr id="row2831580216137"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p4903315216137"><a name="p4903315216137"></a><a name="p4903315216137"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p4573700616137"><a name="p4573700616137"></a><a name="p4573700616137"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p6032521316137"><a name="p6032521316137"></a><a name="p6032521316137"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1711318416137"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p1178551316137"><a name="p1178551316137"></a><a name="p1178551316137"></a>security_group</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p3114620116137"><a name="p3114620116137"></a><a name="p3114620116137"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p5959614316137"><a name="p5959614316137"></a><a name="p5959614316137"></a>security_group对象，参见<a href="安全组API简介-OpenStack.md#table513726041607">表1</a></p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section2347777416137"></a>

请求样例

```
PUT /v2.0/security-groups/d29ae17d-f355-4992-8747-1fb66cc9afd2  
{
    "security_group": {
           "name": "sg-test02"
    }
}
```

响应样例

```
{
    "security_group": {
        "id": "d29ae17d-f355-4992-8747-1fb66cc9afd2",
        "name": "sg-test02",
        "description": "",
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "security_group_rules": [
            {
                "id": "6332de3e-98fb-4f8c-b44a-fcb8ff09881e",
                "direction": "egress",
                "protocol": null,
                "ethertype": "IPv6",
                "description": null,
                "remote_group_id": null,
                "remote_ip_prefix": null,
                "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
                "port_range_max": null,
                "port_range_min": null,
                "security_group_id": "d29ae17d-f355-4992-8747-1fb66cc9afd2"
            },
            {
                "id": "3f51e52c-0e85-40f7-a137-85927392e436",
                "direction": "egress",
                "protocol": null,
                "ethertype": "IPv4",
                "description": null,
                "remote_group_id": null,
                "remote_ip_prefix": null,
                "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
                "port_range_max": null,
                "port_range_min": null,
                "security_group_id": "d29ae17d-f355-4992-8747-1fb66cc9afd2"
            }
        ],
        "created_at": "2018-09-20T02:15:34",
        "updated_at": "2018-09-20T02:16:31"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

