# 查询子网列表<a name="ZH-CN_TOPIC_0062160178"></a>

## 功能介绍<a name="section47928120"></a>

查询提交请求的租户的所有子网，单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section28699899"></a>

GET /v2.0/subnets

样例：

```
/v2.0/subnets?name={subnet_name}&ip_version={ip_version}&network_id={network_id}&cidr={subnet_cidr_address}&gateway_ip={subnet_gateway}&tenant_id={tenant_id}&enable_dhcp={is_enable_dhcp}
```

## 请求消息<a name="section42990474"></a>

无。

## 响应消息<a name="section51369953"></a>

**表 1**  响应参数

<a name="table51277242"></a>
<table><thead align="left"><tr id="row64740644"><th class="cellrowborder" valign="top" width="23.122312231223123%" id="mcps1.2.4.1.1"><p id="p9500791"><a name="p9500791"></a><a name="p9500791"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.552555255525554%" id="mcps1.2.4.1.2"><p id="p31366578"><a name="p31366578"></a><a name="p31366578"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.325132513251326%" id="mcps1.2.4.1.3"><p id="p40344834"><a name="p40344834"></a><a name="p40344834"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46706151"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p25101909"><a name="p25101909"></a><a name="p25101909"></a>subnets</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p19988723"><a name="p19988723"></a><a name="p19988723"></a>List(subnet)</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p15291872"><a name="p15291872"></a><a name="p15291872"></a>subnet对象列表，参见<a href="子网API简介-OpenStack.md#table12211980105515">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section64320104111236"></a>

请求样例

```
GET /v2.0/subnets?limit=1
```

响应样例

```
{
    "subnets": [
        {
            "name": "kesmdemeet",
            "cidr": "172.16.236.0/24",
            "id": "011fc878-5521-4654-a1ad-f5b0b5820302",
            "enable_dhcp": true,
            "network_id": "48efad0c-079d-4cc8-ace0-dce35d584124",
            "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",            "dns_nameservers": [],
            "allocation_pools": [
                {
                    "start": "172.16.236.2",
                    "end": "172.16.236.251"
                }
            ],
            "host_routes": [],
            "ip_version": 4,
            "gateway_ip": "172.16.236.1",
            "created_at": "2018-03-26T08:23:43",
            "updated_at": "2018-03-26T08:23:44"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

