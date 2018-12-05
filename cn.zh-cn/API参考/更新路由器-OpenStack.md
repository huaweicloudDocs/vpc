# 更新路由器<a name="ZH-CN_TOPIC_0060495816"></a>

## 功能介绍<a name="section2668865720589"></a>

更新路由器。

## URI<a name="section6156926920589"></a>

PUT /v2.0/routers/\{router\_id\}

## 请求消息<a name="section3272152320589"></a>

**表 1**  请求参数

<a name="table3319773520589"></a>
<table><thead align="left"><tr id="row680247320589"><th class="cellrowborder" valign="top" width="14.430000000000001%" id="mcps1.2.5.1.1"><p id="p1412942020589"><a name="p1412942020589"></a><a name="p1412942020589"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.2"><p id="p363234320589"><a name="p363234320589"></a><a name="p363234320589"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.3"><p id="p2578437120589"><a name="p2578437120589"></a><a name="p2578437120589"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="69.07%" id="mcps1.2.5.1.4"><p id="p815930320589"><a name="p815930320589"></a><a name="p815930320589"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5692383620589"><td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.1 "><p id="p4742802620589"><a name="p4742802620589"></a><a name="p4742802620589"></a>router</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.2 "><p id="p1646487220589"><a name="p1646487220589"></a><a name="p1646487220589"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.3 "><p id="p5858622220589"><a name="p5858622220589"></a><a name="p5858622220589"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="69.07%" headers="mcps1.2.5.1.4 "><p id="p63022381205744"><a name="p63022381205744"></a><a name="p63022381205744"></a>router对象列表，参见<a href="路由器API简介-OpenStack.md#table24153696181443">表1</a>。</p>
<p id="p2811868820589"><a name="p2811868820589"></a><a name="p2811868820589"></a>必选参数：无，更新操作时至少指定一项属性</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section6302125920589"></a>

**表 2**  响应参数

<a name="table444833020589"></a>
<table><thead align="left"><tr id="row3190269720589"><th class="cellrowborder" valign="top" width="15.73%" id="mcps1.2.4.1.1"><p id="p3398165120589"><a name="p3398165120589"></a><a name="p3398165120589"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.99%" id="mcps1.2.4.1.2"><p id="p105036620589"><a name="p105036620589"></a><a name="p105036620589"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="75.28%" id="mcps1.2.4.1.3"><p id="p4635141320589"><a name="p4635141320589"></a><a name="p4635141320589"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row6347701020589"><td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.2.4.1.1 "><p id="p4136417520589"><a name="p4136417520589"></a><a name="p4136417520589"></a>router</p>
</td>
<td class="cellrowborder" valign="top" width="8.99%" headers="mcps1.2.4.1.2 "><p id="p6216386020589"><a name="p6216386020589"></a><a name="p6216386020589"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="75.28%" headers="mcps1.2.4.1.3 "><p id="p3652335220589"><a name="p3652335220589"></a><a name="p3652335220589"></a>router对象列表，参见<a href="路由器API简介-OpenStack.md#table24153696181443">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section6027472020589"></a>

请求样例

```
PUT /v2.0/routers/f5dbdfe0-86f9-4b0a-9a32-6be143f0a076  
{
    "router": {
           "name": "router-220"
    }
}
```

响应样例

```
{
    "router": {
        "id": "f5dbdfe0-86f9-4b0a-9a32-6be143f0a076",
        "name": "router-220",
        "status": "ACTIVE",
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "admin_state_up": true,
        "external_gateway_info": {
            "network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
            "enable_snat": false
        },
        "routes": [],
        "created_at": "2018-09-20T02:06:07",
        "updated_at": "2018-09-20T02:06:09"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

