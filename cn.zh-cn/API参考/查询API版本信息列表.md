# 查询API版本信息列表<a name="vpc_version_0001"></a>

## 功能介绍<a name="section47928120"></a>

返回当前API所有可用的版本（仅针对OpenStack原生接口）。

## URI<a name="section28699899"></a>

GET

## 请求消息<a name="section42990474"></a>

请求参数

无

请求样例

```
GET https://{Endpoint}/
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
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p1668082023018"><a name="p1668082023018"></a><a name="p1668082023018"></a>Array of <a href="#table7472653181512">version</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p15291872"><a name="p15291872"></a><a name="p15291872"></a>API版本列表，请参见<a href="#table7472653181512">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  version对象

<a name="table7472653181512"></a>
<table><thead align="left"><tr id="row24721153191511"><th class="cellrowborder" valign="top" width="23.122312231223123%" id="mcps1.2.4.1.1"><p id="p7472853151518"><a name="p7472853151518"></a><a name="p7472853151518"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.552555255525554%" id="mcps1.2.4.1.2"><p id="p1647210534155"><a name="p1647210534155"></a><a name="p1647210534155"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.325132513251326%" id="mcps1.2.4.1.3"><p id="p11472185317150"><a name="p11472185317150"></a><a name="p11472185317150"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18472155310158"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p147217533154"><a name="p147217533154"></a><a name="p147217533154"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p947255320159"><a name="p947255320159"></a><a name="p947255320159"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p47752014191"><a name="p47752014191"></a><a name="p47752014191"></a>API版本的状态：</p>
<a name="ul1053872581218"></a><a name="ul1053872581218"></a><ul id="ul1053872581218"><li>CURRENT（当前版本）</li><li>STABLE（稳定版本）</li><li>DEPRECATED（废弃版本）</li></ul>
</td>
</tr>
<tr id="row747215312152"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p10472115381512"><a name="p10472115381512"></a><a name="p10472115381512"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p9472115313158"><a name="p9472115313158"></a><a name="p9472115313158"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p647375331518"><a name="p647375331518"></a><a name="p647375331518"></a>API版本</p>
</td>
</tr>
<tr id="row174734534159"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p18473105321516"><a name="p18473105321516"></a><a name="p18473105321516"></a>links</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p984011365304"><a name="p984011365304"></a><a name="p984011365304"></a>Array of <a href="#table62331111162">link</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p164731253181513"><a name="p164731253181513"></a><a name="p164731253181513"></a>链接列表，请参见<a href="#table62331111162">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  link对象

<a name="table62331111162"></a>
<table><thead align="left"><tr id="row1823611191619"><th class="cellrowborder" valign="top" width="23.122312231223123%" id="mcps1.2.4.1.1"><p id="p19231111161619"><a name="p19231111161619"></a><a name="p19231111161619"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.552555255525554%" id="mcps1.2.4.1.2"><p id="p112301121618"><a name="p112301121618"></a><a name="p112301121618"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.325132513251326%" id="mcps1.2.4.1.3"><p id="p1323611171617"><a name="p1323611171617"></a><a name="p1323611171617"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row15260111169"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p192851171616"><a name="p192851171616"></a><a name="p192851171616"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p122815111167"><a name="p122815111167"></a><a name="p122815111167"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p12813117167"><a name="p12813117167"></a><a name="p12813117167"></a>API链接</p>
</td>
</tr>
<tr id="row132891118162"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="p1728171118161"><a name="p1728171118161"></a><a name="p1728171118161"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="p42820114167"><a name="p42820114167"></a><a name="p42820114167"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="p5289119162"><a name="p5289119162"></a><a name="p5289119162"></a>API链接与该API版本的关系</p>
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

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

