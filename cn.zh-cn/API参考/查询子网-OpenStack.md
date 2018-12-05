# 查询子网<a name="ZH-CN_TOPIC_0062160179"></a>

## 功能介绍<a name="section17487184"></a>

查询子网详情

## URI<a name="section23166934"></a>

GET /v2.0/subnets/\{subnet\_id\}

## 请求消息<a name="section64582388"></a>

无。

## 响应消息<a name="section44370581"></a>

**表 1**  响应参数

<a name="table14681450"></a>
<table><thead align="left"><tr id="row21069217"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p28885026"><a name="p28885026"></a><a name="p28885026"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p57985771"><a name="p57985771"></a><a name="p57985771"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p4499576"><a name="p4499576"></a><a name="p4499576"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row28921355"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p60928390"><a name="p60928390"></a><a name="p60928390"></a>subnet</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p36252562"><a name="p36252562"></a><a name="p36252562"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p19248251"><a name="p19248251"></a><a name="p19248251"></a>subnet对象列表，参见<a href="子网API简介-OpenStack.md#table12211980105515">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section63790914"></a>

请求样例

```
GET /v2.0/subnets/011fc878-5521-4654-a1ad-f5b0b5820302
```

响应样例

```
{
    "subnet": {
        "name": "kesmdemeet",
        "cidr": "172.16.236.0/24",
        "id": "011fc878-5521-4654-a1ad-f5b0b5820302",
        "enable_dhcp": true,
        "network_id": "48efad0c-079d-4cc8-ace0-dce35d584124",
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "dns_nameservers": [],
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
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

