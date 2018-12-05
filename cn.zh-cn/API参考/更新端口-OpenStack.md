# 更新端口<a name="ZH-CN_TOPIC_0062207809"></a>

## 功能介绍<a name="zh-cn_topic_0062207392_section23646388"></a>

更新端口。

## URI<a name="zh-cn_topic_0062207392_section11490904"></a>

PUT /v2.0/ports/\{port\_id\}

## 请求消息<a name="zh-cn_topic_0062207392_section55370462"></a>

**表 1**  请求参数

<a name="zh-cn_topic_0062207392_table10296933"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207392_row62640398"><th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0062207392_p40707460"><a name="zh-cn_topic_0062207392_p40707460"></a><a name="zh-cn_topic_0062207392_p40707460"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.16%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0062207392_p8970000"><a name="zh-cn_topic_0062207392_p8970000"></a><a name="zh-cn_topic_0062207392_p8970000"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0062207392_p55481367"><a name="zh-cn_topic_0062207392_p55481367"></a><a name="zh-cn_topic_0062207392_p55481367"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="65.31%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0062207392_p64805763"><a name="zh-cn_topic_0062207392_p64805763"></a><a name="zh-cn_topic_0062207392_p64805763"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207392_row14775484"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0062207392_p55963561"><a name="zh-cn_topic_0062207392_p55963561"></a><a name="zh-cn_topic_0062207392_p55963561"></a>ports</p>
</td>
<td class="cellrowborder" valign="top" width="8.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0062207392_p36754611"><a name="zh-cn_topic_0062207392_p36754611"></a><a name="zh-cn_topic_0062207392_p36754611"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0062207392_p24333505"><a name="zh-cn_topic_0062207392_p24333505"></a><a name="zh-cn_topic_0062207392_p24333505"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="65.31%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0062207386_p50516929"><a name="zh-cn_topic_0062207386_p50516929"></a><a name="zh-cn_topic_0062207386_p50516929"></a>port对象列表，参见<a href="端口API简介-OpenStack.md#table15919752145624">表1</a></p>
<p id="zh-cn_topic_0062207392_p22385437"><a name="zh-cn_topic_0062207392_p22385437"></a><a name="zh-cn_topic_0062207392_p22385437"></a>必选字段：无，更新操作时至少指定一项属性</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0062207392_section28572113"></a>

**表 2**  响应参数

<a name="zh-cn_topic_0062207392_table1281126"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207392_row10321460"><th class="cellrowborder" valign="top" width="15.559999999999999%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207392_p30731970"><a name="zh-cn_topic_0062207392_p30731970"></a><a name="zh-cn_topic_0062207392_p30731970"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.33%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207392_p6261652"><a name="zh-cn_topic_0062207392_p6261652"></a><a name="zh-cn_topic_0062207392_p6261652"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="71.11%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207392_p12079142"><a name="zh-cn_topic_0062207392_p12079142"></a><a name="zh-cn_topic_0062207392_p12079142"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207392_row38886454"><td class="cellrowborder" valign="top" width="15.559999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207392_p62795050"><a name="zh-cn_topic_0062207392_p62795050"></a><a name="zh-cn_topic_0062207392_p62795050"></a>ports</p>
</td>
<td class="cellrowborder" valign="top" width="13.33%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207392_p53234283"><a name="zh-cn_topic_0062207392_p53234283"></a><a name="zh-cn_topic_0062207392_p53234283"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="71.11%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207392_p35602929"><a name="zh-cn_topic_0062207392_p35602929"></a><a name="zh-cn_topic_0062207392_p35602929"></a>port对象列表，参见<a href="端口API简介-OpenStack.md#table15919752145624">表1</a></p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0062207392_section55822426"></a>

请求样例

```
PUT /v2.0/ports/7a9a954a-eb41-4954-a300-11ab17a361a2  
{
    "port": {
           "name": "port-test02"
    }
}
```

响应样例

```
{
    "port": {
        "id": "a7d98f3c-b42f-460b-96a1-07601e145961",
        "name": "port-test02",
        "status": "DOWN",
        "admin_state_up": true,
        "fixed_ips": [],
        "mac_address": "fa:16:3e:01:f7:90",
        "network_id": "00ae08c5-f727-49ab-ad4b-b069398aa171",
        "tenant_id": "db82c9e1415a464ea68048baa8acc6b8",
        "project_id": "db82c9e1415a464ea68048baa8acc6b8",
        "device_id": "",
        "device_owner": "",
        "security_groups": [
            "d0d58aa9-cda9-414c-9c52-6c3daf8534e6"
        ],
        "extra_dhcp_opts": [],
        "allowed_address_pairs": [],
        "binding:vnic_type": "normal",
        "binding:vif_details": {},
        "binding:profile": {},
        "port_security_enabled": true,
        "created_at": "2018-09-20T01:45:26",
        "updated_at": "2018-09-20T01:48:56"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

