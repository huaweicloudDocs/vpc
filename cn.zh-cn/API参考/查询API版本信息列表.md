# 查询API版本信息列表<a name="ZH-CN_TOPIC_0100582600"></a>

## 功能介绍<a name="section47928120"></a>

返回当前API所有可用的版本（仅针对OpenStack原生接口）。

## URI<a name="section28699899"></a>

GET

## 请求消息<a name="section42990474"></a>

请求参数

无

请求样例

```
GET /
```

## 响应消息<a name="section51369953"></a>

响应参数

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
<tbody><tr id="row46706151"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p25101909"><a name="p25101909"></a><a name="p25101909"></a>versions</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p19988723"><a name="p19988723"></a><a name="p19988723"></a>List</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p15291872"><a name="p15291872"></a><a name="p15291872"></a>API版本列表</p>
</td>
</tr>
<tr id="row152771610135510"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p3277310205517"><a name="p3277310205517"></a><a name="p3277310205517"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p9277101075514"><a name="p9277101075514"></a><a name="p9277101075514"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p20277121025515"><a name="p20277121025515"></a><a name="p20277121025515"></a>API版本的状态，值可为CURRENT，STABLE，DEPRECATED</p>
</td>
</tr>
<tr id="row95031021115715"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p15503122135718"><a name="p15503122135718"></a><a name="p15503122135718"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p850322175720"><a name="p850322175720"></a><a name="p850322175720"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p75032217576"><a name="p75032217576"></a><a name="p75032217576"></a>API版本</p>
</td>
</tr>
<tr id="row87148285575"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p471522845712"><a name="p471522845712"></a><a name="p471522845712"></a>links</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p18715192814578"><a name="p18715192814578"></a><a name="p18715192814578"></a>List</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p14715728195710"><a name="p14715728195710"></a><a name="p14715728195710"></a>链接列表</p>
</td>
</tr>
<tr id="row6401103475719"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p340123410573"><a name="p340123410573"></a><a name="p340123410573"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p840113418575"><a name="p840113418575"></a><a name="p840113418575"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p184011834135714"><a name="p184011834135714"></a><a name="p184011834135714"></a>API链接</p>
</td>
</tr>
<tr id="row064116391574"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p1164173965718"><a name="p1164173965718"></a><a name="p1164173965718"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p06411739165717"><a name="p06411739165717"></a><a name="p06411739165717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p46416393575"><a name="p46416393575"></a><a name="p46416393575"></a>API链接与该API版本的关系</p>
</td>
</tr>
</tbody>
</table>

响应样例

```
{
    "versions": [
        {
            "status": "CURRENT", 
            "id": "v2.0", 
            "links": [
                {
                    "href": "https://None/v2.0", 
                    "rel": "self"
                }
            ]
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

