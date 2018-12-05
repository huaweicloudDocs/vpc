# 查询浮动IP<a name="ZH-CN_TOPIC_0060333021"></a>

## 功能介绍<a name="section433032482159"></a>

查询浮动IP详情。

## URI<a name="section269019862159"></a>

GET /v2.0/floatingips/\{floatingip\_id\}

## 请求消息<a name="section513321362159"></a>

无。

## 响应消息<a name="section414903182159"></a>

**表 1**  响应参数

<a name="table52726292159"></a>
<table><thead align="left"><tr id="row483206142159"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p216556632159"><a name="p216556632159"></a><a name="p216556632159"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.99%" id="mcps1.2.4.1.2"><p id="p92783132159"><a name="p92783132159"></a><a name="p92783132159"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="69.66%" id="mcps1.2.4.1.3"><p id="p72773912159"><a name="p72773912159"></a><a name="p72773912159"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row525977702159"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p325609822159"><a name="p325609822159"></a><a name="p325609822159"></a>floatingip</p>
</td>
<td class="cellrowborder" valign="top" width="8.99%" headers="mcps1.2.4.1.2 "><p id="p201938822159"><a name="p201938822159"></a><a name="p201938822159"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.4.1.3 "><p id="p191679172159"><a name="p191679172159"></a><a name="p191679172159"></a>floatingip对象列表，参见<a href="浮动IP-API简介-OpenStack.md#table5388109319164">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section382935262159"></a>

请求样例

```
GET /v2.0/floatingips/1a3a2818-d9b4-4a9c-8a19-5252c499d1cd
```

响应样例

```
{
    "floatingip": {
        "id": "1a3a2818-d9b4-4a9c-8a19-5252c499d1cd",
        "status": "DOWN",
        "router_id": null,
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "floating_network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
        "fixed_ip_address": null,
        "floating_ip_address": "99.99.99.84",
        "port_id": null,
        "created_at": "2017-10-19T12:21:28",
        "updated_at": "2018-07-30T12:52:13"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

