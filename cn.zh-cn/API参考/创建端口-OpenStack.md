# 创建端口<a name="ZH-CN_TOPIC_0062207808"></a>

## 功能介绍<a name="zh-cn_topic_0062207340_section45663083"></a>

创建端口。

## URI<a name="zh-cn_topic_0062207340_section8314568"></a>

POST /v2.0/ports

## 请求消息<a name="zh-cn_topic_0062207340_section21522370"></a>

**表 1**  请求参数

<a name="zh-cn_topic_0062207340_table29618759"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207340_row3151905"><th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0062207340_p53977738"><a name="zh-cn_topic_0062207340_p53977738"></a><a name="zh-cn_topic_0062207340_p53977738"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="10.2%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0062207340_p10120656"><a name="zh-cn_topic_0062207340_p10120656"></a><a name="zh-cn_topic_0062207340_p10120656"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.16%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0062207340_p14466778"><a name="zh-cn_topic_0062207340_p14466778"></a><a name="zh-cn_topic_0062207340_p14466778"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="67.35%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0062207340_p30958352"><a name="zh-cn_topic_0062207340_p30958352"></a><a name="zh-cn_topic_0062207340_p30958352"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207340_row24598620"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0062207340_p46331171"><a name="zh-cn_topic_0062207340_p46331171"></a><a name="zh-cn_topic_0062207340_p46331171"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="10.2%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0062207340_p61837391"><a name="zh-cn_topic_0062207340_p61837391"></a><a name="zh-cn_topic_0062207340_p61837391"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="8.16%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0062207340_p42772808"><a name="zh-cn_topic_0062207340_p42772808"></a><a name="zh-cn_topic_0062207340_p42772808"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="67.35%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0062207340_p42045429"><a name="zh-cn_topic_0062207340_p42045429"></a><a name="zh-cn_topic_0062207340_p42045429"></a>port对象列表，参见<a href="端口API简介-OpenStack.md#table15919752145624">表1</a></p>
<p id="zh-cn_topic_0062207340_p42864547"><a name="zh-cn_topic_0062207340_p42864547"></a><a name="zh-cn_topic_0062207340_p42864547"></a>必选字段：network_id</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0062207340_section59483605"></a>

**表 2**  响应参数

<a name="zh-cn_topic_0062207340_table42633357"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207340_row53195707"><th class="cellrowborder" valign="top" width="15.559999999999999%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207340_p13884972"><a name="zh-cn_topic_0062207340_p13884972"></a><a name="zh-cn_topic_0062207340_p13884972"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.110000000000001%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207340_p50940942"><a name="zh-cn_topic_0062207340_p50940942"></a><a name="zh-cn_topic_0062207340_p50940942"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="73.33%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207340_p21379907"><a name="zh-cn_topic_0062207340_p21379907"></a><a name="zh-cn_topic_0062207340_p21379907"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207340_row54050919"><td class="cellrowborder" valign="top" width="15.559999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207340_p16048282"><a name="zh-cn_topic_0062207340_p16048282"></a><a name="zh-cn_topic_0062207340_p16048282"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207340_p24842503"><a name="zh-cn_topic_0062207340_p24842503"></a><a name="zh-cn_topic_0062207340_p24842503"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="73.33%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207340_p51342761"><a name="zh-cn_topic_0062207340_p51342761"></a><a name="zh-cn_topic_0062207340_p51342761"></a>ports信息，参见<a href="端口API简介-OpenStack.md#table15919752145624">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0062207340_section65590400"></a>

请求样例

```
POST /v2.0/ports 
{
    "port": {
       "admin_state_up": true,
        "network_id": "00ae08c5-f727-49ab-ad4b-b069398aa171",
        "name": "port-test"
    }
}
```

响应样例

```
{
    "port": {
        "id": "a7d98f3c-b42f-460b-96a1-07601e145961",
        "name": "port-test",
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
        "updated_at": "2018-09-20T01:45:26"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

