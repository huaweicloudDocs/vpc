# 创建安全组规则<a name="ZH-CN_TOPIC_0060595558"></a>

## 功能介绍<a name="section5958580616319"></a>

创建安全组规则。

## URI<a name="section6291358016319"></a>

POST /v2.0/security-group-rules

## 请求消息<a name="section3953869316319"></a>

**表 1**  请求参数

<a name="table981991416319"></a>
<table><thead align="left"><tr id="row191482716319"><th class="cellrowborder" valign="top" width="26.52734726527347%" id="mcps1.2.5.1.1"><p id="p2280026616319"><a name="p2280026616319"></a><a name="p2280026616319"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.5.1.2"><p id="p1835529716319"><a name="p1835529716319"></a><a name="p1835529716319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p3464228716319"><a name="p3464228716319"></a><a name="p3464228716319"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p3284526816319"><a name="p3284526816319"></a><a name="p3284526816319"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3793835116319"><td class="cellrowborder" valign="top" width="26.52734726527347%" headers="mcps1.2.5.1.1 "><p id="p4303593816319"><a name="p4303593816319"></a><a name="p4303593816319"></a>security_group_rule</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p3852346816319"><a name="p3852346816319"></a><a name="p3852346816319"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p6530542116319"><a name="p6530542116319"></a><a name="p6530542116319"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p732393116218"><a name="p732393116218"></a><a name="p732393116218"></a>security_group_rule对象列表，参见<a href="安全组API简介-OpenStack.md#table655457801607">表2</a>。</p>
<p id="p3126719916319"><a name="p3126719916319"></a><a name="p3126719916319"></a>必选参数：direction，security_group_id</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section2023987716319"></a>

**表 2**  响应参数

<a name="table676552316319"></a>
<table><thead align="left"><tr id="row5032047016319"><th class="cellrowborder" valign="top" width="31.7%" id="mcps1.2.4.1.1"><p id="p4182747116319"><a name="p4182747116319"></a><a name="p4182747116319"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.080000000000002%" id="mcps1.2.4.1.2"><p id="p4264467116319"><a name="p4264467116319"></a><a name="p4264467116319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p4267558716319"><a name="p4267558716319"></a><a name="p4267558716319"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row60629616319"><td class="cellrowborder" valign="top" width="31.7%" headers="mcps1.2.4.1.1 "><p id="p2428304416319"><a name="p2428304416319"></a><a name="p2428304416319"></a>security_group_rule</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.4.1.2 "><p id="p2724314316319"><a name="p2724314316319"></a><a name="p2724314316319"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p5745755316319"><a name="p5745755316319"></a><a name="p5745755316319"></a>security_group_rule对象列表，参见<a href="安全组API简介-OpenStack.md#table655457801607">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section5025263616319"></a>

请求样例

```
POST /v2.0/security-group-rules
{
    "security_group_rule": {
        "security_group_id": "5cb9c1ee-00e0-4d0f-9623-55463cd26ff8", 
        "direction": "egress", 
        "protocol": "tcp", 
        "remote_ip_prefix": "10.10.0.0/24"
    }
}
```

响应样例

```
{
    "security_group_rule": {
        "remote_group_id": null, 
        "direction": "egress", 
        "remote_ip_prefix": "10.10.0.0/24", 
        "protocol": "tcp", 
        "tenant_id": "6fbe9263116a4b68818cf1edce16bc4f", 
        "port_range_max": null, 
        "security_group_id": "5cb9c1ee-00e0-4d0f-9623-55463cd26ff8", 
        "port_range_min": null, 
        "ethertype": "IPv4", 
        "description": null, 
        "id": "7c336b04-1603-4911-a6f4-f2af1d9a0488",
        "project_id": "6fbe9263116a4b68818cf1edce16bc4f", 
        "created_at": "2018-09-20T02:15:34",
        "updated_at": "2018-09-20T02:15:34"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

