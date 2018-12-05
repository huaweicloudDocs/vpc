# 更新网络ACL规则<a name="ZH-CN_TOPIC_0060574380"></a>

## 功能介绍<a name="section48881744123249"></a>

更新网络ACL规则。

## URI<a name="section40985924123249"></a>

PUT /v2.0/fwaas/firewall\_rules/\{firewall\_rule\_id\}

## 请求消息<a name="section49242216123249"></a>

**表 1**  请求参数

<a name="table30921260123249"></a>
<table><thead align="left"><tr id="row39375977123249"><th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.1"><p id="p12242224123249"><a name="p12242224123249"></a><a name="p12242224123249"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p24418590123249"><a name="p24418590123249"></a><a name="p24418590123249"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p13201747123249"><a name="p13201747123249"></a><a name="p13201747123249"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p62761712123249"><a name="p62761712123249"></a><a name="p62761712123249"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row57358099123249"><td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.1 "><p id="p46539485123249"><a name="p46539485123249"></a><a name="p46539485123249"></a>firewall_rule</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p13703023123249"><a name="p13703023123249"></a><a name="p13703023123249"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p21092839123249"><a name="p21092839123249"></a><a name="p21092839123249"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p3044429312329"><a name="p3044429312329"></a><a name="p3044429312329"></a>firewall rule对象，参见<a href="网络ACL简介-OpenStack.md#table38646929121127">表1</a>。</p>
<p id="p52349002123249"><a name="p52349002123249"></a><a name="p52349002123249"></a>必选字段：无</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section9857292123249"></a>

**表 2**  响应参数

<a name="table38652922123249"></a>
<table><thead align="left"><tr id="row54513389123249"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p28336710123249"><a name="p28336710123249"></a><a name="p28336710123249"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p47571350123249"><a name="p47571350123249"></a><a name="p47571350123249"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p23002266123249"><a name="p23002266123249"></a><a name="p23002266123249"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row47557263123249"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p57698555123249"><a name="p57698555123249"></a><a name="p57698555123249"></a>firewall_rule</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p31745790123249"><a name="p31745790123249"></a><a name="p31745790123249"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p35727944123249"><a name="p35727944123249"></a><a name="p35727944123249"></a>firewall rule对象，参见<a href="网络ACL简介-OpenStack.md#table38646929121127">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section10725923123249"></a>

请求样例

```
PUT /v2.0/fwaas/firewall_rules/b94acf06-efc2-485d-ba67-a61acf2a7e28
{
    "firewall_rule": {
        "action": "deny"
    }
}
```

响应样例

```
{
    "firewall_rule": {
        "protocol": "tcp", 
        "description": "", 
        "source_ip_address": null, 
        "destination_ip_address": null, 
        "source_port": null, 
        "destination_port": "80", 
        "id": "b94acf06-efc2-485d-ba67-a61acf2a7e28", 
        "name": "ALLOW_HTTP", 
        "tenant_id": "23c8a121505047b6869edf39f3062712", 
        "enabled": true, 
        "action": "deny", 
        "ip_version": 4, 
        "public": false,
        "project_id": "23c8a121505047b6869edf39f3062712"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

