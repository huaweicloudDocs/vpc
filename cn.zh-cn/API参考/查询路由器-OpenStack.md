# 查询路由器<a name="ZH-CN_TOPIC_0060495814"></a>

## 功能介绍<a name="section64937351205744"></a>

查询路由器详情。

## URI<a name="section27580478205744"></a>

GET /v2.0/routers/\{router\_id\}

## 请求消息<a name="section60819119205744"></a>

无。

## 响应消息<a name="section45287922205744"></a>

**表 1**  响应参数

<a name="table44443065205744"></a>
<table><thead align="left"><tr id="row61398570205744"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p7228234205744"><a name="p7228234205744"></a><a name="p7228234205744"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p48616054205744"><a name="p48616054205744"></a><a name="p48616054205744"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p1505045205744"><a name="p1505045205744"></a><a name="p1505045205744"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row54799831205744"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p9601350205744"><a name="p9601350205744"></a><a name="p9601350205744"></a>router</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p39511881205744"><a name="p39511881205744"></a><a name="p39511881205744"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p63022381205744"><a name="p63022381205744"></a><a name="p63022381205744"></a>router对象列表，参见<a href="路由器API简介-OpenStack.md#table24153696181443">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section4539230205744"></a>

请求样例

```
GET /v2.0/routers/01ab4be1-4447-45fb-94be-3ee787ed4ebe
```

响应样例

```
{
    "router": {
        "id": "01ab4be1-4447-45fb-94be-3ee787ed4ebe",
        "name": "xiaoleizi-tag",
        "status": "ACTIVE",
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "admin_state_up": true,
        "external_gateway_info": {
            "network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
            "enable_snat": false
        },
        "routes": [
            {
                "destination": "0.0.0.0/0",
                "nexthop": "172.16.0.124"
            }
        ],
        "created_at": "2018-03-23T09:26:08",
        "updated_at": "2018-08-24T08:49:53"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

