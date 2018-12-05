# 更新子网<a name="ZH-CN_TOPIC_0062160181"></a>

## 功能介绍<a name="section10267951"></a>

更新子网。

接口约束：

更新allocation\_pools字段时范围不能包含网关和广播地址的所有IP。

## URI<a name="section25302698"></a>

PUT /v2.0/subnets/\{subnet\_id\}

## 请求消息<a name="section36252627"></a>

**表 1**  请求参数

<a name="table40701910"></a>
<table><thead align="left"><tr id="row5914937"><th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1"><p id="p9347893"><a name="p9347893"></a><a name="p9347893"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.16%" id="mcps1.2.5.1.2"><p id="p18981865"><a name="p18981865"></a><a name="p18981865"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10.2%" id="mcps1.2.5.1.3"><p id="p61136126"><a name="p61136126"></a><a name="p61136126"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="67.35%" id="mcps1.2.5.1.4"><p id="p53079196"><a name="p53079196"></a><a name="p53079196"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4447594"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="p24710800"><a name="p24710800"></a><a name="p24710800"></a>subnet</p>
</td>
<td class="cellrowborder" valign="top" width="8.16%" headers="mcps1.2.5.1.2 "><p id="p55417783"><a name="p55417783"></a><a name="p55417783"></a>dict</p>
</td>
<td class="cellrowborder" valign="top" width="10.2%" headers="mcps1.2.5.1.3 "><p id="p59655430"><a name="p59655430"></a><a name="p59655430"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.35%" headers="mcps1.2.5.1.4 "><p id="p37955333"><a name="p37955333"></a><a name="p37955333"></a>subnet对象列表，参见<a href="子网API简介-OpenStack.md#table12211980105515">表1</a>。</p>
<p id="p2265180"><a name="p2265180"></a><a name="p2265180"></a>必选字段：无，更新操作时至少指定一项属性</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section57838187"></a>

**表 2**  响应参数

<a name="table49261880"></a>
<table><thead align="left"><tr id="row31386613"><th class="cellrowborder" valign="top" width="31.7%" id="mcps1.2.4.1.1"><p id="p59287744"><a name="p59287744"></a><a name="p59287744"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.080000000000002%" id="mcps1.2.4.1.2"><p id="p37577972"><a name="p37577972"></a><a name="p37577972"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p58217140"><a name="p58217140"></a><a name="p58217140"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17967889"><td class="cellrowborder" valign="top" width="31.7%" headers="mcps1.2.4.1.1 "><p id="p46112886"><a name="p46112886"></a><a name="p46112886"></a>subnet</p>
</td>
<td class="cellrowborder" valign="top" width="17.080000000000002%" headers="mcps1.2.4.1.2 "><p id="p44156300"><a name="p44156300"></a><a name="p44156300"></a>dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p522217"><a name="p522217"></a><a name="p522217"></a>subnet对象列表，参见<a href="子网API简介-OpenStack.md#table12211980105515">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section5055526711495"></a>

请求样例

```
PUT /v2.0/subnets/98bac90c-0ba7-4a63-8995-097da9bead1c  
{
  "subnet": {
    "name": "subnet-test"
  }
}
```

响应样例

```
{
    "subnet": {
        "name": "subnet-test",
        "cidr": "172.16.2.0/24",
        "id": "98bac90c-0ba7-4a63-8995-097da9bead1c",
        "enable_dhcp": true,
        "network_id": "0133cd73-34d4-4d4c-bf1f-e65b24603206",
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "dns_nameservers": [],
        "allocation_pools": [
            {
                "start": "172.16.2.2",
                "end": "172.16.2.251"
            }
        ],
        "host_routes": [],
        "ip_version": 4,
        "gateway_ip": "172.16.2.1",
        "created_at": "2018-09-20T02:02:16",
        "updated_at": "2018-09-20T02:03:03"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

