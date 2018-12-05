# 创建网络<a name="ZH-CN_TOPIC_0060495803"></a>

## 功能介绍<a name="section6414416120507"></a>

创建网络。

## URI<a name="section5332460720507"></a>

POST /v2.0/networks

## 请求消息<a name="section4437514120507"></a>

**表 1**  请求参数

<a name="table3761670020507"></a>
<table><thead align="left"><tr id="row4177733320507"><th class="cellrowborder" valign="top" width="14.430000000000001%" id="mcps1.2.5.1.1"><p id="p2852081420507"><a name="p2852081420507"></a><a name="p2852081420507"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.2"><p id="p2848463220507"><a name="p2848463220507"></a><a name="p2848463220507"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.3"><p id="p2555388320507"><a name="p2555388320507"></a><a name="p2555388320507"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="69.07%" id="mcps1.2.5.1.4"><p id="p5659862220507"><a name="p5659862220507"></a><a name="p5659862220507"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2108564120507"><td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.1 "><p id="p3021536520507"><a name="p3021536520507"></a><a name="p3021536520507"></a>network</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.2 "><p id="p3152549720507"><a name="p3152549720507"></a><a name="p3152549720507"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.3 "><p id="p342849420507"><a name="p342849420507"></a><a name="p342849420507"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="69.07%" headers="mcps1.2.5.1.4 "><p id="p3740541204921"><a name="p3740541204921"></a><a name="p3740541204921"></a>network对象列表，参见<a href="网络API简介-OpenStack.md#table49902238182444">表1</a>。</p>
<p id="p927262020507"><a name="p927262020507"></a><a name="p927262020507"></a>必选字段：无</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section1288473020507"></a>

**表 2**  响应参数

<a name="table3703017620507"></a>
<table><thead align="left"><tr id="row256778820507"><th class="cellrowborder" valign="top" width="21.59%" id="mcps1.2.4.1.1"><p id="p666426420507"><a name="p666426420507"></a><a name="p666426420507"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.63%" id="mcps1.2.4.1.2"><p id="p293447220507"><a name="p293447220507"></a><a name="p293447220507"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="64.78%" id="mcps1.2.4.1.3"><p id="p5993672520507"><a name="p5993672520507"></a><a name="p5993672520507"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2303659520507"><td class="cellrowborder" valign="top" width="21.59%" headers="mcps1.2.4.1.1 "><p id="p5402491720507"><a name="p5402491720507"></a><a name="p5402491720507"></a>network</p>
</td>
<td class="cellrowborder" valign="top" width="13.63%" headers="mcps1.2.4.1.2 "><p id="p1394218020507"><a name="p1394218020507"></a><a name="p1394218020507"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="64.78%" headers="mcps1.2.4.1.3 "><p id="p526423120507"><a name="p526423120507"></a><a name="p526423120507"></a>network对象列表，参见<a href="网络API简介-OpenStack.md#table49902238182444">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section4737808120507"></a>

请求样例

```
POST /v2.0/networks 
{
    "network": {
           "name": "network-test",
           "shared": false,
           "admin_state_up": true
    }
}
```

响应样例

```
{
    "network": {
        "id": "c360322d-5315-45d7-b7d2-481f98c56edb",
        "name": "network-test",
        "status": "ACTIVE",
        "shared": false,
        "subnets": [],
        "availability_zone_hints": [],
        "availability_zones": [
            "az2.dc2",
            "az5.dc5"
        ],
        "admin_state_up": true,
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "provider:network_type": "vxlan",
        "router:external": false,
        "port_security_enabled": true,
        "created_at": "2018-09-20T01:53:18",
        "updated_at": "2018-09-20T01:53:20"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

