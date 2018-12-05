# 查询路由器列表<a name="ZH-CN_TOPIC_0062224579"></a>

## 功能介绍<a name="section55573059205730"></a>

查询提交请求的租户有权限操作的所有路由器信息，单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section46115681205730"></a>

GET /v2.0/routers

样例：

```
/v2.0/routers?id={id}&name={name}&admin_state_up={admin_state_up}&tenant_id={tenant_id}&status={status}
```

## 请求消息<a name="section22539803205730"></a>

无。

## 响应消息<a name="section56953834205730"></a>

**表 1**  响应参数

<a name="table49857835205730"></a>
<table><thead align="left"><tr id="row16977544205730"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p33003808205730"><a name="p33003808205730"></a><a name="p33003808205730"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.11%" id="mcps1.2.4.1.2"><p id="p56062768205730"><a name="p56062768205730"></a><a name="p56062768205730"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.540000000000006%" id="mcps1.2.4.1.3"><p id="p4141274205730"><a name="p4141274205730"></a><a name="p4141274205730"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row67007812205730"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p58923719205730"><a name="p58923719205730"></a><a name="p58923719205730"></a>routers</p>
</td>
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p8091914205730"><a name="p8091914205730"></a><a name="p8091914205730"></a>List(router)</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p7937265205730"><a name="p7937265205730"></a><a name="p7937265205730"></a>router对象列表，参见<a href="路由器API简介-OpenStack.md#table24153696181443">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section4326525205730"></a>

请求样例

```
GET /v2.0/routers?limit=1
```

响应样例

```
{
    "routers": [
        {
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
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

