# 批量创建和删除弹性IP资源标签<a name="eip_tag_0004"></a>

## 功能介绍<a name="section16984350162413"></a>

为指定的弹性IP资源实例批量添加或删除标签。

此接口为幂等接口：

创建时如果请求体中存在重复key则报错。

创建时，不允许设置重复key数据,如果数据库已存在该key，就覆盖value的值。

删除时，如果删除的标签不存在，默认处理成功,删除时不对标签字符集范围做校验。删除时tags结构体不能缺失，key不能为空，或者空字符串。

## URI<a name="section49844500244"></a>

POST /v2.0/\{project\_id\}/publicips/\{publicip\_id\}/tags/action

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
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row21254748"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p43913021"><a name="p43913021"></a><a name="p43913021"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p184914"><a name="p184914"></a><a name="p184914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p14978051"><a name="p14978051"></a><a name="p14978051"></a>EIP唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section1799117501243"></a>

请求参数

**表 2**  请求参数

<a name="table8992250172415"></a>
<table><thead align="left"><tr id="row3711351132413"><th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.1"><p id="p471145111242"><a name="p471145111242"></a><a name="p471145111242"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="18%" id="mcps1.2.5.1.2"><p id="p47115515247"><a name="p47115515247"></a><a name="p47115515247"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="18.509999999999998%" id="mcps1.2.5.1.3"><p id="p10711051202417"><a name="p10711051202417"></a><a name="p10711051202417"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="49.49%" id="mcps1.2.5.1.4"><p id="p117218511241"><a name="p117218511241"></a><a name="p117218511241"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row572951152420"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="p17721851132411"><a name="p17721851132411"></a><a name="p17721851132411"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="p072551172414"><a name="p072551172414"></a><a name="p072551172414"></a>Array of <a href="#table13242848193719">tag</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.5.1.3 "><p id="p7721851162410"><a name="p7721851162410"></a><a name="p7721851162410"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="49.49%" headers="mcps1.2.5.1.4 "><p id="p67265110244"><a name="p67265110244"></a><a name="p67265110244"></a>tag对象列表，请参见<a href="#table13242848193719">表3</a>。</p>
</td>
</tr>
<tr id="row57295120245"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="p572115152417"><a name="p572115152417"></a><a name="p572115152417"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="p12724511244"><a name="p12724511244"></a><a name="p12724511244"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.5.1.3 "><p id="p3721951162417"><a name="p3721951162417"></a><a name="p3721951162417"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="49.49%" headers="mcps1.2.5.1.4 "><p id="p1562014114112"><a name="p1562014114112"></a><a name="p1562014114112"></a>操作标识：</p>
<a name="ul2205152413110"></a><a name="ul2205152413110"></a><ul id="ul2205152413110"><li>create：创建</li><li>delete：删除</li></ul>
</td>
</tr>
</tbody>
</table>

**表 3**  tag对象

<a name="table13242848193719"></a>
<table><thead align="left"><tr id="row13343144812379"><th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.1"><p id="p15343174853715"><a name="p15343174853715"></a><a name="p15343174853715"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="18.060000000000002%" id="mcps1.2.5.1.2"><p id="p13431648163716"><a name="p13431648163716"></a><a name="p13431648163716"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.3"><p id="p169809965412"><a name="p169809965412"></a><a name="p169809965412"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="56.699999999999996%" id="mcps1.2.5.1.4"><p id="p11344748183719"><a name="p11344748183719"></a><a name="p11344748183719"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row103449487379"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.1 "><p id="p183469482373"><a name="p183469482373"></a><a name="p183469482373"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.5.1.2 "><p id="p1434684863710"><a name="p1434684863710"></a><a name="p1434684863710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="p298018911544"><a name="p298018911544"></a><a name="p298018911544"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="56.699999999999996%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><ul id="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"><li>标签名称</li><li>不能为空。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li><li>同一资源的key值不能重复。</li></ul>
</td>
</tr>
<tr id="row2346548163714"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.1 "><p id="p1134624816377"><a name="p1134624816377"></a><a name="p1134624816377"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.5.1.2 "><p id="p234619483371"><a name="p234619483371"></a><a name="p234619483371"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="p209805915417"><a name="p209805915417"></a><a name="p209805915417"></a>action为create时：是；action为delete时：否</p>
</td>
<td class="cellrowborder" valign="top" width="56.699999999999996%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><ul id="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"><li>标签值</li><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
</td>
</tr>
</tbody>
</table>

请求样例1：批量创建标签

```
POST https://{Endpoint}/v2.0/{project_id}/publicips/{publicip_id}/tags/action

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
POST https://{Endpoint}/v2.0/{project_id}/publicips/{publicip_id}/tags/action

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

## 响应消息<a name="section173510241"></a>

响应参数

无

响应样例

无

## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

