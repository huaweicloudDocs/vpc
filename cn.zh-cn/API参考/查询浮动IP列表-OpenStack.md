# 查询浮动IP列表<a name="ZH-CN_TOPIC_0060333020"></a>

## 功能介绍<a name="section310981132148"></a>

查询提交请求的租户有权限操作的所有浮动IP地址。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section548377002148"></a>

GET /v2.0/floatingips

样例：

```
/v2.0/floatingips?id={fip_id}&router_id={router_id}&floating_network_id={net_id}&floating_ip_address={floating_ip}&port_id={port_id}&fixed_ip_address={fixed_ip}&tenant_id={tenant_id}
```

## 请求消息<a name="section656683442148"></a>

无。

## 响应消息<a name="section236032922148"></a>

**表 1**  响应参数

<a name="table328184742148"></a>
<table><thead align="left"><tr id="row308815332148"><th class="cellrowborder" valign="top" width="15.559999999999999%" id="mcps1.2.4.1.1"><p id="p183762202148"><a name="p183762202148"></a><a name="p183762202148"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.2"><p id="p120788402148"><a name="p120788402148"></a><a name="p120788402148"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.11%" id="mcps1.2.4.1.3"><p id="p608097322148"><a name="p608097322148"></a><a name="p608097322148"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row266412852148"><td class="cellrowborder" valign="top" width="15.559999999999999%" headers="mcps1.2.4.1.1 "><p id="p104605152148"><a name="p104605152148"></a><a name="p104605152148"></a>floatingips</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p419953972148"><a name="p419953972148"></a><a name="p419953972148"></a>List(floatingip)</p>
</td>
<td class="cellrowborder" valign="top" width="61.11%" headers="mcps1.2.4.1.3 "><p id="p499181352148"><a name="p499181352148"></a><a name="p499181352148"></a>floatingip对象列表，参见<a href="浮动IP-API简介-OpenStack.md#table5388109319164">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section466100362148"></a>

请求样例

```
GET /v2.0/floatingips?limit=1
```

响应样例

```
{
    "floatingips": [
        {
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
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

