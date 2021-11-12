# 查询VPC项目标签<a name="vpc_tag_0006"></a>

## 功能介绍<a name="section159501022015"></a>

查询租户在指定区域和实例类型的所有标签集合。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=ListVpcTags)中直接运行调试该接口。

## URI<a name="section13950150202019"></a>

GET /v2.0/\{project\_id\}/vpcs/tags

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
</tbody>
</table>

## 请求消息<a name="section159561804206"></a>

请求参数

无

请求样例

```
GET https://{Endpoint}/v2.0/{project_id}/vpcs/tags
```

## 响应消息<a name="section4956302200"></a>

响应参数

**表 2**  响应参数

<a name="table18958160152014"></a>
<table><thead align="left"><tr id="row106121102012"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p14611716203"><a name="p14611716203"></a><a name="p14611716203"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.48%" id="mcps1.2.4.1.2"><p id="p8613112202"><a name="p8613112202"></a><a name="p8613112202"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.16999999999999%" id="mcps1.2.4.1.3"><p id="p062121192014"><a name="p062121192014"></a><a name="p062121192014"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row96219162018"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p16624112203"><a name="p16624112203"></a><a name="p16624112203"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="13.48%" headers="mcps1.2.4.1.2 "><p id="p146212172016"><a name="p146212172016"></a><a name="p146212172016"></a>Array of <a href="#table1696410062019">tag</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="65.16999999999999%" headers="mcps1.2.4.1.3 "><p id="p46214112203"><a name="p46214112203"></a><a name="p46214112203"></a>标签列表</p>
</td>
</tr>
</tbody>
</table>

**表 3**  tag字段数据结构说明

<a name="table1696410062019"></a>
<table><thead align="left"><tr id="row16625112015"><th class="cellrowborder" valign="top" width="25.332533253325334%" id="mcps1.2.4.1.1"><p id="p156216117208"><a name="p156216117208"></a><a name="p156216117208"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.332533253325334%" id="mcps1.2.4.1.2"><p id="p8622172014"><a name="p8622172014"></a><a name="p8622172014"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="49.33493349334934%" id="mcps1.2.4.1.3"><p id="p1262101182018"><a name="p1262101182018"></a><a name="p1262101182018"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row166216192017"><td class="cellrowborder" valign="top" width="25.332533253325334%" headers="mcps1.2.4.1.1 "><p id="p562013203"><a name="p562013203"></a><a name="p562013203"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="25.332533253325334%" headers="mcps1.2.4.1.2 "><p id="p4621132014"><a name="p4621132014"></a><a name="p4621132014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="49.33493349334934%" headers="mcps1.2.4.1.3 "><p id="p3622162019"><a name="p3622162019"></a><a name="p3622162019"></a>键。</p>
<a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><ul id="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"><li>不能为空。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li></ul>
</td>
</tr>
<tr id="row862171152012"><td class="cellrowborder" valign="top" width="25.332533253325334%" headers="mcps1.2.4.1.1 "><p id="p2062312201"><a name="p2062312201"></a><a name="p2062312201"></a>values</p>
</td>
<td class="cellrowborder" valign="top" width="25.332533253325334%" headers="mcps1.2.4.1.2 "><p id="p7282112319144"><a name="p7282112319144"></a><a name="p7282112319144"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="49.33493349334934%" headers="mcps1.2.4.1.3 "><p id="p166210162014"><a name="p166210162014"></a><a name="p166210162014"></a>值列表。</p>
<a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><ul id="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
</td>
</tr>
</tbody>
</table>

响应样例

```
{
    "tags": [
        {
            "key": "key1",
            "values": [
                "value1",
                "value2"
            ]
        },
        {
            "key": "key2",
            "values": [
                "value1",
                "value2"
            ]
        }
    ]
}
```

## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

