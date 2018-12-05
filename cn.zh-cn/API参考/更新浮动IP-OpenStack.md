# 更新浮动IP<a name="ZH-CN_TOPIC_0060333023"></a>

## 功能介绍<a name="section6285365021641"></a>

更新浮动IP。

接口约束：

绑定浮动IP过程中，如果浮动IP处于“error”状态，请先尝试执行浮动IP解绑定动作。

不支持直接把已经绑定端口的浮动ip重新绑定到另外一个端口上，必须先解绑定再绑定。

## URI<a name="section5206576221641"></a>

PUT /v2.0/floatingips/\{floatingip\_id\}

## 请求消息<a name="section2938074421641"></a>

**表 1**  请求参数

<a name="table3103003021641"></a>
<table><thead align="left"><tr id="row5907300221641"><th class="cellrowborder" valign="top" width="19.59%" id="mcps1.2.5.1.1"><p id="p2018384621641"><a name="p2018384621641"></a><a name="p2018384621641"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.2.5.1.2"><p id="p2427879021641"><a name="p2427879021641"></a><a name="p2427879021641"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.3"><p id="p2042494621641"><a name="p2042494621641"></a><a name="p2042494621641"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="54.63%" id="mcps1.2.5.1.4"><p id="p4380795521641"><a name="p4380795521641"></a><a name="p4380795521641"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5878350521641"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.1 "><p id="p6384347521641"><a name="p6384347521641"></a><a name="p6384347521641"></a>floatingip</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.2 "><p id="p393901021641"><a name="p393901021641"></a><a name="p393901021641"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.3 "><p id="p5062438921641"><a name="p5062438921641"></a><a name="p5062438921641"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="54.63%" headers="mcps1.2.5.1.4 "><p id="p557124874610"><a name="p557124874610"></a><a name="p557124874610"></a>floatingip对象列表，参见<a href="浮动IP-API简介-OpenStack.md#table5388109319164">表1</a>。</p>
<p id="p693485321641"><a name="p693485321641"></a><a name="p693485321641"></a>必选字段：无</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section2485220121641"></a>

**表 2**  响应参数

<a name="table6687125821641"></a>
<table><thead align="left"><tr id="row2678790321641"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p2233651921641"><a name="p2233651921641"></a><a name="p2233651921641"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.11%" id="mcps1.2.4.1.2"><p id="p6442759121641"><a name="p6442759121641"></a><a name="p6442759121641"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.540000000000006%" id="mcps1.2.4.1.3"><p id="p5780308921641"><a name="p5780308921641"></a><a name="p5780308921641"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5153866721641"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p1388252621641"><a name="p1388252621641"></a><a name="p1388252621641"></a>floatingip</p>
</td>
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p5074280121641"><a name="p5074280121641"></a><a name="p5074280121641"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p6355285621641"><a name="p6355285621641"></a><a name="p6355285621641"></a>floatingip对象列表，参见<a href="浮动IP-API简介-OpenStack.md#table5388109319164">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section3510479621641"></a>

请求样例1

```
PUT /v2.0/floatingips/b997e0d4-3359-4c74-8f88-bc0af81cd5a2  
{
    "floatingip": {
           "port_id": "f91f5763-c5a2-4458-979d-61e48b3c3fac"
    }
}
```

响应样例1

```
{
    "floatingip": {
        "id": "b997e0d4-3359-4c74-8f88-bc0af81cd5a2",
        "status": "DOWN",
        "router_id": null,
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "floating_network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
        "fixed_ip_address": "192.168.10.3",
        "floating_ip_address": "88.88.215.205",
        "port_id": 00587256-27e3-489b-96bf-ea80c1da4aeb,
        "created_at": "2018-09-20T02:10:02",
        "updated_at": "2018-09-20T02:10:07"
    }
}
```

请求样例2

```
PUT /v2.0/floatingips/b997e0d4-3359-4c74-8f88-bc0af81cd5a2
{
    "floatingip": {
        "port_id": null
    }
}
```

响应样例2

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
        "updated_at": "2018-09-20T02:10:07"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

