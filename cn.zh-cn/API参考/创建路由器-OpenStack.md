# 创建路由器<a name="ZH-CN_TOPIC_0060495815"></a>

## 功能介绍<a name="section54866008205757"></a>

创建路由器。

## URI<a name="section437105205757"></a>

POST /v2.0/routers

## 请求消息<a name="section56558784205757"></a>

**表 1**  请求参数

<a name="table17858782205757"></a>
<table><thead align="left"><tr id="row29195524205757"><th class="cellrowborder" valign="top" width="19.388061193880613%" id="mcps1.2.5.1.1"><p id="p16027205205757"><a name="p16027205205757"></a><a name="p16027205205757"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.2"><p id="p23135223205757"><a name="p23135223205757"></a><a name="p23135223205757"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p62013761205757"><a name="p62013761205757"></a><a name="p62013761205757"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p57058764205757"><a name="p57058764205757"></a><a name="p57058764205757"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row58357184205757"><td class="cellrowborder" valign="top" width="19.388061193880613%" headers="mcps1.2.5.1.1 "><p id="p29311427205757"><a name="p29311427205757"></a><a name="p29311427205757"></a>router</p>
</td>
<td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.2 "><p id="p25415424205757"><a name="p25415424205757"></a><a name="p25415424205757"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p45383453205757"><a name="p45383453205757"></a><a name="p45383453205757"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p52181058205757"><a name="p52181058205757"></a><a name="p52181058205757"></a>router对象列表，参见<a href="路由器API简介-OpenStack.md#table24153696181443">表1</a>。必选字段：无</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section56374749205757"></a>

**表 2**  响应参数

<a name="table2951934205757"></a>
<table><thead align="left"><tr id="row46218389205757"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p52702038205757"><a name="p52702038205757"></a><a name="p52702038205757"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p41006687205757"><a name="p41006687205757"></a><a name="p41006687205757"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p5443692205757"><a name="p5443692205757"></a><a name="p5443692205757"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row38285887205757"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p14149114205757"><a name="p14149114205757"></a><a name="p14149114205757"></a>router</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p5227590205757"><a name="p5227590205757"></a><a name="p5227590205757"></a>Dict</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p5591471205757"><a name="p5591471205757"></a><a name="p5591471205757"></a>router对象，参见<a href="路由器API简介-OpenStack.md#table24153696181443">表1</a></p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section50323245205757"></a>

请求样例

```
POST /v2.0/routers 
{
    "router": {
           "name": "router-test2",
           "admin_state_up": true
    }
}
```

响应样例

```
{
    "router": {
        "id": "f5dbdfe0-86f9-4b0a-9a32-6be143f0a076",
        "name": "router-test2",
        "status": "ACTIVE",
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "admin_state_up": true,
        "external_gateway_info": {
            "network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
            "enable_snat": false
        },
        "routes": [],
        "created_at": "2018-09-20T02:06:07",
        "updated_at": "2018-09-20T02:06:09"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

