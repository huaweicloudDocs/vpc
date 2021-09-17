# 批量创建和删除VPC资源标签<a name="vpc_tag_0004"></a>

## 功能介绍<a name="section9716105931810"></a>

为指定的VPC资源实例批量添加或删除标签。

此接口为幂等接口：

创建时如果请求体中存在重复key则报错。

创建时，不允许设置重复key数据，如果数据库已存在该key，就覆盖value的值。

删除时，如果删除的标签不存在，默认处理成功，删除时不对标签字符集范围做校验。删除时tags结构体不能缺失，key不能为空，或者空字符串。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=BatchCreateVpcTags)中直接运行调试该接口。

## URI<a name="section14718205991814"></a>

POST /v2.0/\{project\_id\}/vpcs/\{vpc\_id\}/tags/action

参数说明请参见[表1](#table27380479)。

**表 1**  参数说明

<a name="table27380479"></a>
<table><thead align="left"><tr id="row28751554"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p47174532"><a name="p47174532"></a><a name="p47174532"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p63040734"><a name="p63040734"></a><a name="p63040734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p6025849"><a name="p6025849"></a><a name="p6025849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18331773"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p8478608"><a name="p8478608"></a><a name="p8478608"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p15678685"><a name="p15678685"></a><a name="p15678685"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row21254748"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p43913021"><a name="p43913021"></a><a name="p43913021"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p184914"><a name="p184914"></a><a name="p184914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p14978051"><a name="p14978051"></a><a name="p14978051"></a>虚拟私有云唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section972418597185"></a>

请求参数

**表 2**  请求参数

<a name="table2726185911818"></a>
<table><thead align="left"><tr id="row1080816597184"><th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.1"><p id="p208081359151817"><a name="p208081359151817"></a><a name="p208081359151817"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.2.5.1.2"><p id="p9808135941814"><a name="p9808135941814"></a><a name="p9808135941814"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="9.900990099009901%" id="mcps1.2.5.1.3"><p id="p080805991816"><a name="p080805991816"></a><a name="p080805991816"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.5.1.4"><p id="p680845913189"><a name="p680845913189"></a><a name="p680845913189"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row180885915182"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p148081759191815"><a name="p148081759191815"></a><a name="p148081759191815"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.2 "><p id="p10424324181820"><a name="p10424324181820"></a><a name="p10424324181820"></a>Array of <a href="#table244913515593">tag</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="9.900990099009901%" headers="mcps1.2.5.1.3 "><p id="p6808115981818"><a name="p6808115981818"></a><a name="p6808115981818"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.5.1.4 "><p id="p180814592186"><a name="p180814592186"></a><a name="p180814592186"></a>tag对象，请参见<a href="#table244913515593">表3</a>。</p>
</td>
</tr>
<tr id="row58082596188"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p128082059141814"><a name="p128082059141814"></a><a name="p128082059141814"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.2 "><p id="p480816591183"><a name="p480816591183"></a><a name="p480816591183"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="9.900990099009901%" headers="mcps1.2.5.1.3 "><p id="p1380825915181"><a name="p1380825915181"></a><a name="p1380825915181"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.5.1.4 "><p id="p1562014114112"><a name="p1562014114112"></a><a name="p1562014114112"></a>操作标识：</p>
<a name="ul2205152413110"></a><a name="ul2205152413110"></a><ul id="ul2205152413110"><li>create：创建</li><li>delete：删除</li></ul>
</td>
</tr>
</tbody>
</table>

**表 3**  tag对象

<a name="table244913515593"></a>
<table><thead align="left"><tr id="row345095195914"><th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.1"><p id="p1045012512597"><a name="p1045012512597"></a><a name="p1045012512597"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="18.060000000000002%" id="mcps1.2.5.1.2"><p id="p124502516594"><a name="p124502516594"></a><a name="p124502516594"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.3"><p id="p169809965412"><a name="p169809965412"></a><a name="p169809965412"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.699999999999996%" id="mcps1.2.5.1.4"><p id="p1545075105910"><a name="p1545075105910"></a><a name="p1545075105910"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row84502515598"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.1 "><p id="p154506595915"><a name="p154506595915"></a><a name="p154506595915"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.5.1.2 "><p id="p14501518591"><a name="p14501518591"></a><a name="p14501518591"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="p298018911544"><a name="p298018911544"></a><a name="p298018911544"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.699999999999996%" headers="mcps1.2.5.1.4 "><a name="ul9450135125915"></a><a name="ul9450135125915"></a><ul id="ul9450135125915"><li>标签名称</li><li>不能为空。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li><li>同一资源的key值不能重复。</li></ul>
</td>
</tr>
<tr id="row845145185917"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.1 "><p id="p12451185185910"><a name="p12451185185910"></a><a name="p12451185185910"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.5.1.2 "><p id="p104515514598"><a name="p104515514598"></a><a name="p104515514598"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="p209805915417"><a name="p209805915417"></a><a name="p209805915417"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.699999999999996%" headers="mcps1.2.5.1.4 "><a name="ul0451105165914"></a><a name="ul0451105165914"></a><ul id="ul0451105165914"><li>标签值</li><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
</td>
</tr>
</tbody>
</table>

请求样例1：批量创建标签

```
POST https://{Endpoint}/v2.0/{project_id}/vpcs/{vpc_id}/tags/action

{
    "action": "create",
    "tags": [
        {
            "key": "key1",
            "value": "value1"
        },
        {
            "key": "key2",
            "value": "value3"
        }
    ]
}
```

请求样例2：批量删除标签

```
POST https://{Endpoint}/v2.0/{project_id}/vpcs/{vpc_id}/tags/action

{
    "action": "delete",
    "tags": [
        {
            "key": "key1",
            "value": "value1"
        },
        {
            "key": "key2",
            "value": "value3"
        }
    ]
}
```

## 响应消息<a name="section973755901815"></a>

响应参数

无

响应样例

无

## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

