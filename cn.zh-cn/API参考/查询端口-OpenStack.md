# 查询端口<a name="ZH-CN_TOPIC_0062207807"></a>

## 功能介绍<a name="zh-cn_topic_0062207351_section48492792"></a>

查询端口详情。

## URI<a name="zh-cn_topic_0062207351_section33781949"></a>

GET /v2.0/ports/\{port\_id\}

## 请求消息<a name="zh-cn_topic_0062207351_section65197270"></a>

无

## 响应消息<a name="zh-cn_topic_0062207351_section49904522"></a>

**表 1**  响应参数

<a name="zh-cn_topic_0062207351_table21718662"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207351_row2001795"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207351_p27927672"><a name="zh-cn_topic_0062207351_p27927672"></a><a name="zh-cn_topic_0062207351_p27927672"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207351_p47548937"><a name="zh-cn_topic_0062207351_p47548937"></a><a name="zh-cn_topic_0062207351_p47548937"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207351_p46581538"><a name="zh-cn_topic_0062207351_p46581538"></a><a name="zh-cn_topic_0062207351_p46581538"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207351_row15008249"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207351_p7708685"><a name="zh-cn_topic_0062207351_p7708685"></a><a name="zh-cn_topic_0062207351_p7708685"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207351_p20423749"><a name="zh-cn_topic_0062207351_p20423749"></a><a name="zh-cn_topic_0062207351_p20423749"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207351_p50928963"><a name="zh-cn_topic_0062207351_p50928963"></a><a name="zh-cn_topic_0062207351_p50928963"></a>port对象列表，参见<a href="端口API简介-OpenStack.md#table15919752145624">表1</a></p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0062207351_section46487516"></a>

请求样例

```
GET /v2.0/ports/791870bd-36a7-4d9b-b015-a78e9b06af08
```

响应样例

```
{
    "port": {
        "id": "791870bd-36a7-4d9b-b015-a78e9b06af08",
        "name": "port-test",
        "status": "DOWN",
        "admin_state_up": true,
        "fixed_ips": [],
        "mac_address": "fa:16:3e:01:e0:b2",
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
        "created_at": "2018-09-13T01:43:41",
        "updated_at": "2018-09-13T01:43:41"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

