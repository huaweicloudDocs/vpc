# 查询安全组<a name="ZH-CN_TOPIC_0060595064"></a>

## 功能介绍<a name="section1170323616037"></a>

查询提交请求的租户有权限操作的所有安全组。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section2797834416037"></a>

GET /v2.0/security-groups

## 请求消息<a name="section3834086716037"></a>

无。

## 响应消息<a name="section6006230416037"></a>

**表 1**  响应参数

<a name="table1547016516037"></a>
<table><thead align="left"><tr id="row2546099716037"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p3614026216037"><a name="p3614026216037"></a><a name="p3614026216037"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p3446060616037"><a name="p3446060616037"></a><a name="p3446060616037"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p3726817816037"><a name="p3726817816037"></a><a name="p3726817816037"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row841863916037"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p5631571516037"><a name="p5631571516037"></a><a name="p5631571516037"></a>security_groups</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p2388987016037"><a name="p2388987016037"></a><a name="p2388987016037"></a>List(security_group)</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p6079210416037"><a name="p6079210416037"></a><a name="p6079210416037"></a>security_group对象列表，参见<a href="安全组API简介-OpenStack.md#table513726041607">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section2440368716037"></a>

请求样例

```
GET /v2.0/security-groups?limit=1
```

响应样例

```
{
    "security_groups": [
        {
            "id": "0431c9c5-1660-42e0-8a00-134bec7f03e2",
            "name": "sg-ad3f",
            "description": "",
            "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
            "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
            "security_group_rules": [
                {
                    "id": "d90e55ba-23bd-4d97-b722-8cb6fb485d69",
                    "direction": "ingress",
                    "protocol": null,
                    "ethertype": "IPv4",
                    "description": null,
                    "remote_group_id": "0431c9c5-1660-42e0-8a00-134bec7f03e2",
                    "remote_ip_prefix": null,
                    "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
                    "port_range_max": null,
                    "port_range_min": null,
                    "security_group_id": "0431c9c5-1660-42e0-8a00-134bec7f03e2"
                },
                {
                    "id": "aecff4d4-9ce9-489c-86a3-803aedec65f7",
                    "direction": "egress",
                    "protocol": null,
                    "ethertype": "IPv4",
                    "description": null,
                    "remote_group_id": null,
                    "remote_ip_prefix": null,
                    "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
                    "port_range_max": null,
                    "port_range_min": null,
                    "security_group_id": "0431c9c5-1660-42e0-8a00-134bec7f03e2"
                }
            ],
            "created_at": "2018-09-12T08:24:14",
            "updated_at": "2018-09-12T08:24:14"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

