# 查询安全组规则<a name="ZH-CN_TOPIC_0060595556"></a>

## 功能介绍<a name="section6306987516218"></a>

查询提交请求的租户有权限操作的所有安全组规则。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section2319473516218"></a>

GET /v2.0/security-group-rules

样例：

```
/v2.0/security-group-rules?security_group_id={security_group_id}&remote_group_id={remote_group_id}&direction={direction}&remote_ip_prefix={remote_ip_prefix}&protocol={protocol}&port_range_max={port_range_max}&port_range_min={port_range_min}&ethertype={ethertype}&tenant_id ={tenant_id}
```

## 请求消息<a name="section4004032316218"></a>

无。

## 响应消息<a name="section4154959916218"></a>

**表 1**  响应参数

<a name="table5126909016218"></a>
<table><thead align="left"><tr id="row4406312316218"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p130340816218"><a name="p130340816218"></a><a name="p130340816218"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p23005316218"><a name="p23005316218"></a><a name="p23005316218"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p1954037216218"><a name="p1954037216218"></a><a name="p1954037216218"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row25691016218"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p5925871816218"><a name="p5925871816218"></a><a name="p5925871816218"></a>security_group_rules</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p2213891816218"><a name="p2213891816218"></a><a name="p2213891816218"></a>List(security_group_rule)</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p732393116218"><a name="p732393116218"></a><a name="p732393116218"></a>security_group_rule对象列表，参见<a href="安全组API简介-OpenStack.md#table655457801607">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section2229785216218"></a>

请求样例

```
GET /v2.0/security-group-rules
```

响应样例

```
{
    "security_group_rules": [
        {
            "remote_group_id": "1d8b19c7-7c56-48f7-a99b-4b40eb390967", 
            "direction": "ingress", 
            "remote_ip_prefix": null, 
            "protocol": null, 
            "tenant_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "port_range_max": null, 
            "security_group_id": "1d8b19c7-7c56-48f7-a99b-4b40eb390967", 
            "port_range_min": null, 
            "ethertype": "IPv6", 
            "description": null, 
            "id": "07adc044-3f21-4eeb-bd57-5e5eb6024b7f",
            "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "created_at": "2018-09-20T02:15:34",
            "updated_at": "2018-09-20T02:15:34"
        }, 
        {
            "remote_group_id": null, 
            "direction": "egress", 
            "remote_ip_prefix": null, 
            "protocol": null, 
            "tenant_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "port_range_max": null, 
            "security_group_id": "328fb454-a2ee-4a11-bdb1-ee19bbdfde43", 
            "port_range_min": null, 
            "ethertype": "IPv6", 
            "description": null, 
            "id": "09358f83-f4a5-4386-9563-a1e3c373d655",
            "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "created_at": "2018-09-20T02:15:34",
            "updated_at": "2018-09-20T02:15:34"
        }, 
        {
            "remote_group_id": "4c763030-366e-428c-be2b-d48f6baf5297", 
            "direction": "ingress", 
            "remote_ip_prefix": null, 
            "protocol": null, 
            "tenant_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "port_range_max": null, 
            "security_group_id": "4c763030-366e-428c-be2b-d48f6baf5297", 
            "port_range_min": null, 
            "ethertype": "IPv6", 
            "description": null, 
            "id": "219a6f56-1069-458b-bec0-df9270e7a074",
            "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "created_at": "2018-09-20T02:15:34",
            "updated_at": "2018-09-20T02:15:34"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

