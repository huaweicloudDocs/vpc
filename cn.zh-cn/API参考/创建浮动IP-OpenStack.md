# 创建浮动IP<a name="ZH-CN_TOPIC_0060333022"></a>

## 功能介绍<a name="section3174871621549"></a>

创建浮动IP。

创建浮动IP的外部网络UUID，请使用GET /v2.0/networks?router:external=True或neutron net-external-list方式获取。

## URI<a name="section5936537521549"></a>

POST /v2.0/floatingips

## 请求消息<a name="section5012846321549"></a>

**表 1**  请求参数

<a name="table3387369821549"></a>
<table><thead align="left"><tr id="row1358409521549"><th class="cellrowborder" valign="top" width="19.59%" id="mcps1.2.5.1.1"><p id="p2656991721549"><a name="p2656991721549"></a><a name="p2656991721549"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.2.5.1.2"><p id="p467970821549"><a name="p467970821549"></a><a name="p467970821549"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.3"><p id="p4351210021549"><a name="p4351210021549"></a><a name="p4351210021549"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="54.63%" id="mcps1.2.5.1.4"><p id="p3481919621549"><a name="p3481919621549"></a><a name="p3481919621549"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row178260421549"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.1 "><p id="p1017324521549"><a name="p1017324521549"></a><a name="p1017324521549"></a>floatingip</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.2 "><p id="p1872651821549"><a name="p1872651821549"></a><a name="p1872651821549"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.3 "><p id="p4045302421549"><a name="p4045302421549"></a><a name="p4045302421549"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="54.63%" headers="mcps1.2.5.1.4 "><p id="p499181352148"><a name="p499181352148"></a><a name="p499181352148"></a>floatingip对象列表，参见<a href="浮动IP-API简介-OpenStack.md#table5388109319164">表1</a>。</p>
<p id="p2946380521549"><a name="p2946380521549"></a><a name="p2946380521549"></a>必选字段：floating_network_id</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section6384765421549"></a>

**表 2**  响应参数

<a name="table427745721549"></a>
<table><thead align="left"><tr id="row435809221549"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p1746120521549"><a name="p1746120521549"></a><a name="p1746120521549"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.11%" id="mcps1.2.4.1.2"><p id="p507150621549"><a name="p507150621549"></a><a name="p507150621549"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.540000000000006%" id="mcps1.2.4.1.3"><p id="p5526791421549"><a name="p5526791421549"></a><a name="p5526791421549"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4751605321549"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p2359506021549"><a name="p2359506021549"></a><a name="p2359506021549"></a>floatingip</p>
</td>
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p3215169621549"><a name="p3215169621549"></a><a name="p3215169621549"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p2411791621549"><a name="p2411791621549"></a><a name="p2411791621549"></a>floatingip对象列表，参见<a href="浮动IP-API简介-OpenStack.md#table5388109319164">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section1573465921549"></a>

请求样例

```
POST /v2.0/floatingips 
{
    "floatingip": {
           "floating_network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975"
    }
}
```

响应样例

```
{
    "floatingip": {
        "id": "b997e0d4-3359-4c74-8f88-bc0af81cd5a2",
        "status": "DOWN",
        "router_id": null,
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "floating_network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
        "fixed_ip_address": null,
        "floating_ip_address": "88.88.215.205",
        "port_id": null,
        "created_at": "2018-09-20T02:10:02",
        "updated_at": "2018-09-20T02:10:02"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

