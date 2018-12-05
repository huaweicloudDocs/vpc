# 创建子网<a name="ZH-CN_TOPIC_0062160180"></a>

## 功能介绍<a name="section54540374"></a>

创建子网

## URI<a name="section21101319"></a>

POST /v2.0/subnets

## 请求消息<a name="section31485239"></a>

**表 1**  请求参数

<a name="table26517876"></a>
<table><thead align="left"><tr id="row40476817"><th class="cellrowborder" valign="top" width="14.430000000000001%" id="mcps1.2.5.1.1"><p id="p57396781"><a name="p57396781"></a><a name="p57396781"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.2"><p id="p18627652"><a name="p18627652"></a><a name="p18627652"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.3"><p id="p32444864"><a name="p32444864"></a><a name="p32444864"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="69.07%" id="mcps1.2.5.1.4"><p id="p10788361"><a name="p10788361"></a><a name="p10788361"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1442054"><td class="cellrowborder" valign="top" width="14.430000000000001%" headers="mcps1.2.5.1.1 "><p id="p49697568"><a name="p49697568"></a><a name="p49697568"></a>subnet</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.2 "><p id="p66080062"><a name="p66080062"></a><a name="p66080062"></a>dict</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.3 "><p id="p50884809"><a name="p50884809"></a><a name="p50884809"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="69.07%" headers="mcps1.2.5.1.4 "><p id="p19248251"><a name="p19248251"></a><a name="p19248251"></a>subnet对象列表，参见<a href="子网API简介-OpenStack.md#table12211980105515">表1</a>。</p>
<p id="p50932971"><a name="p50932971"></a><a name="p50932971"></a>必选字段：network_id，cidr</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section14931696"></a>

**表 2**  响应参数

<a name="table31929956"></a>
<table><thead align="left"><tr id="row12454319"><th class="cellrowborder" valign="top" width="15.73%" id="mcps1.2.4.1.1"><p id="p2166929"><a name="p2166929"></a><a name="p2166929"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.99%" id="mcps1.2.4.1.2"><p id="p41303584"><a name="p41303584"></a><a name="p41303584"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="75.28%" id="mcps1.2.4.1.3"><p id="p7224675"><a name="p7224675"></a><a name="p7224675"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row48327783"><td class="cellrowborder" valign="top" width="15.73%" headers="mcps1.2.4.1.1 "><p id="p22236344"><a name="p22236344"></a><a name="p22236344"></a>subnet</p>
</td>
<td class="cellrowborder" valign="top" width="8.99%" headers="mcps1.2.4.1.2 "><p id="p56313405"><a name="p56313405"></a><a name="p56313405"></a>dict</p>
</td>
<td class="cellrowborder" valign="top" width="75.28%" headers="mcps1.2.4.1.3 "><p id="p37955333"><a name="p37955333"></a><a name="p37955333"></a>subnet对象列表，参见<a href="子网API简介-OpenStack.md#table12211980105515">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section38241653113834"></a>

请求样例

```
POST /v2.0/subnets 
{
    "subnet": {
           "name": "subnet-test",
           "network_id": "0133cd73-34d4-4d4c-bf1f-e65b24603206",
           "cidr": "172.16.2.0/24",
           "enable_dhcp": true
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
        "updated_at": "2018-09-20T02:02:16"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

