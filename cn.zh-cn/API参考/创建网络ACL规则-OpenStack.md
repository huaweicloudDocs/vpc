# 创建网络ACL规则<a name="ZH-CN_TOPIC_0060574379"></a>

## 功能介绍<a name="section3826619212329"></a>

创建网络ACL规则。

## URI<a name="section2109482512329"></a>

POST /v2.0/fwaas/firewall\_rules

## 请求消息<a name="section2533876012329"></a>

**表 1**  请求参数

<a name="table1879369612329"></a>
<table><thead align="left"><tr id="row34303012329"><th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.1"><p id="p1807949812329"><a name="p1807949812329"></a><a name="p1807949812329"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p262059712329"><a name="p262059712329"></a><a name="p262059712329"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p4218882212329"><a name="p4218882212329"></a><a name="p4218882212329"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p2622676712329"><a name="p2622676712329"></a><a name="p2622676712329"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1636364712329"><td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.1 "><p id="p3751930212329"><a name="p3751930212329"></a><a name="p3751930212329"></a>firewall_rule</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p6089760312329"><a name="p6089760312329"></a><a name="p6089760312329"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p1109711212329"><a name="p1109711212329"></a><a name="p1109711212329"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p61314665122957"><a name="p61314665122957"></a><a name="p61314665122957"></a>firewall rule对象，参见<a href="网络ACL简介-OpenStack.md#table38646929121127">表1</a>。</p>
<p id="p1698184812329"><a name="p1698184812329"></a><a name="p1698184812329"></a>必选字段：无</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section3990074312329"></a>

**表 2**  响应参数

<a name="table209507312329"></a>
<table><thead align="left"><tr id="row5536995412329"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p2706537512329"><a name="p2706537512329"></a><a name="p2706537512329"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p5424121912329"><a name="p5424121912329"></a><a name="p5424121912329"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p1697811312329"><a name="p1697811312329"></a><a name="p1697811312329"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3190076212329"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p5714453912329"><a name="p5714453912329"></a><a name="p5714453912329"></a>firewall_rule</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p394121812329"><a name="p394121812329"></a><a name="p394121812329"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p3044429312329"><a name="p3044429312329"></a><a name="p3044429312329"></a>firewall rule对象，参见<a href="网络ACL简介-OpenStack.md#table38646929121127">表1</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section1765314912329"></a>

请求样例

```
POST /v2.0/fwaas/firewall_rules
{
    "firewall_rule": {
        "action": "allow", 
        "enabled": true, 
        "destination_port": "80", 
        "protocol": "tcp", 
        "name": "ALLOW_HTTP"
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
        "action": "allow", 
        "ip_version": 4, 
        "public": false,
        "project_id": "23c8a121505047b6869edf39f3062712"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

