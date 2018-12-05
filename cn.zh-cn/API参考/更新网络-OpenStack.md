# 更新网络<a name="ZH-CN_TOPIC_0060495804"></a>

## 功能介绍<a name="section33818323205249"></a>

更新网络。

## URI<a name="section24604448205249"></a>

PUT /v2.0/networks/\{network\_id\}

## 请求消息<a name="section59272937205249"></a>

**表 1**  请求参数

<a name="table36378601205249"></a>
<table><thead align="left"><tr id="row6955900205249"><th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1"><p id="p26557067205249"><a name="p26557067205249"></a><a name="p26557067205249"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.16%" id="mcps1.2.5.1.2"><p id="p3638851205249"><a name="p3638851205249"></a><a name="p3638851205249"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.3"><p id="p26311499205249"><a name="p26311499205249"></a><a name="p26311499205249"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="65.31%" id="mcps1.2.5.1.4"><p id="p50856651205249"><a name="p50856651205249"></a><a name="p50856651205249"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row25748076205249"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="p5219413205249"><a name="p5219413205249"></a><a name="p5219413205249"></a>networks</p>
</td>
<td class="cellrowborder" valign="top" width="8.16%" headers="mcps1.2.5.1.2 "><p id="p20119343205249"><a name="p20119343205249"></a><a name="p20119343205249"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="p19054114205249"><a name="p19054114205249"></a><a name="p19054114205249"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="65.31%" headers="mcps1.2.5.1.4 "><p id="p3740541204921"><a name="p3740541204921"></a><a name="p3740541204921"></a>network对象列表，参见<a href="网络API简介-OpenStack.md#table49902238182444">表1</a>。</p>
<p id="p66023294205249"><a name="p66023294205249"></a><a name="p66023294205249"></a>必选字段：无，更新操作时至少指定一项属性</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section57338736205249"></a>

**表 2**  响应参数

<a name="table13926044205249"></a>
<table><thead align="left"><tr id="row9699884205249"><th class="cellrowborder" valign="top" width="15.559999999999999%" id="mcps1.2.4.1.1"><p id="p47493145205249"><a name="p47493145205249"></a><a name="p47493145205249"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.33%" id="mcps1.2.4.1.2"><p id="p21739555205249"><a name="p21739555205249"></a><a name="p21739555205249"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="71.11%" id="mcps1.2.4.1.3"><p id="p26886828205249"><a name="p26886828205249"></a><a name="p26886828205249"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row30349435205249"><td class="cellrowborder" valign="top" width="15.559999999999999%" headers="mcps1.2.4.1.1 "><p id="p42385159205249"><a name="p42385159205249"></a><a name="p42385159205249"></a>networks</p>
</td>
<td class="cellrowborder" valign="top" width="13.33%" headers="mcps1.2.4.1.2 "><p id="p10645815205249"><a name="p10645815205249"></a><a name="p10645815205249"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="71.11%" headers="mcps1.2.4.1.3 "><p id="p53974692205249"><a name="p53974692205249"></a><a name="p53974692205249"></a>网络元数据，参见<a href="网络API简介-OpenStack.md#table49902238182444">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section9873970205249"></a>

请求样例

```
PUT /v2.0/networks/c360322d-5315-45d7-b7d2-481f98c56edb  
{
  "network": {
    "name": "network-test02"
  }
}
```

响应样例

```
{
    "network": {
        "id": "c360322d-5315-45d7-b7d2-481f98c56edb",
        "name": "network-test02",
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
        "updated_at": "2018-09-20T01:55:47"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

