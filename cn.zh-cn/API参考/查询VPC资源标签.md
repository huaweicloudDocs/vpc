# 查询VPC资源标签<a name="vpc_tag_0002"></a>

## 功能介绍<a name="section5346624101819"></a>

查询指定VPC实例的标签信息。

该类型接口目前仅在“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”区域开放。

## URI<a name="section7346122401818"></a>

GET /v2.0/\{project\_id\}/vpcs/\{vpc\_id\}/tags

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

## 请求消息<a name="section13185925275"></a>

-   请求参数

    无

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/{project_id}/vpcs/{vpc_id}/tags
    ```


## 响应消息<a name="section1635502415182"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table1135702419184"></a>
    <table><thead align="left"><tr id="row7424152414187"><th class="cellrowborder" valign="top" width="12.4%" id="mcps1.2.4.1.1"><p id="p14424202481810"><a name="p14424202481810"></a><a name="p14424202481810"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.47%" id="mcps1.2.4.1.2"><p id="p1442492451817"><a name="p1442492451817"></a><a name="p1442492451817"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="64.13%" id="mcps1.2.4.1.3"><p id="p18424202481819"><a name="p18424202481819"></a><a name="p18424202481819"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row14424192461816"><td class="cellrowborder" valign="top" width="12.4%" headers="mcps1.2.4.1.1 "><p id="p1942472411816"><a name="p1942472411816"></a><a name="p1942472411816"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.47%" headers="mcps1.2.4.1.2 "><p id="p10424324181820"><a name="p10424324181820"></a><a name="p10424324181820"></a>Array of <a href="#table13242848193719">tag</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.13%" headers="mcps1.2.4.1.3 "><p id="p742482418183"><a name="p742482418183"></a><a name="p742482418183"></a>tag对象列表，请参见<a href="#table13242848193719">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tag对象

    <a name="table13242848193719"></a>
    <table><thead align="left"><tr id="row13343144812379"><th class="cellrowborder" valign="top" width="21.33%" id="mcps1.2.4.1.1"><p id="p15343174853715"><a name="p15343174853715"></a><a name="p15343174853715"></a>属性</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p13431648163716"><a name="p13431648163716"></a><a name="p13431648163716"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.67%" id="mcps1.2.4.1.3"><p id="p11344748183719"><a name="p11344748183719"></a><a name="p11344748183719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row103449487379"><td class="cellrowborder" valign="top" width="21.33%" headers="mcps1.2.4.1.1 "><p id="p183469482373"><a name="p183469482373"></a><a name="p183469482373"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1434684863710"><a name="p1434684863710"></a><a name="p1434684863710"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.67%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><ul id="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"><li>标签名称</li><li>不能为空。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li><li>同一资源的key值不能重复。</li></ul>
    </td>
    </tr>
    <tr id="row2346548163714"><td class="cellrowborder" valign="top" width="21.33%" headers="mcps1.2.4.1.1 "><p id="p1134624816377"><a name="p1134624816377"></a><a name="p1134624816377"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p234619483371"><a name="p234619483371"></a><a name="p234619483371"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.67%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><a name="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><ul id="zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"><li>标签值</li><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
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


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

