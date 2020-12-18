# 删除端口<a name="vpc_port02_0005"></a>

## 功能介绍<a name="zh-cn_topic_0062207359_section45238241"></a>

删除端口。

接口约束：

-   不允许删除device\_owner为非空且不为neutron:VIP\_PORT的端口。
-   不允许删除device\_id为非空的端口。

## URI<a name="zh-cn_topic_0062207359_section4490990"></a>

DELETE /v2.0/ports/\{port\_id\}

参数说明请参见[表1](#table1855162528)。

**表 1**  参数说明

<a name="table1855162528"></a>
<table><thead align="left"><tr id="vpc_port02_0002_row1394617591304"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="vpc_port02_0002_p159467591307"><a name="vpc_port02_0002_p159467591307"></a><a name="vpc_port02_0002_p159467591307"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="vpc_port02_0002_p1094612597019"><a name="vpc_port02_0002_p1094612597019"></a><a name="vpc_port02_0002_p1094612597019"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="vpc_port02_0002_p29466591203"><a name="vpc_port02_0002_p29466591203"></a><a name="vpc_port02_0002_p29466591203"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_port02_0002_row1494695918012"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="vpc_port02_0002_p9946159600"><a name="vpc_port02_0002_p9946159600"></a><a name="vpc_port02_0002_p9946159600"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="vpc_port02_0002_p09465594017"><a name="vpc_port02_0002_p09465594017"></a><a name="vpc_port02_0002_p09465594017"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="vpc_port02_0002_p394618591401"><a name="vpc_port02_0002_p394618591401"></a><a name="vpc_port02_0002_p394618591401"></a>端口唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0062207359_section52706911"></a>

无。

## 响应消息<a name="zh-cn_topic_0062207359_section4600155"></a>

无。

## 样例<a name="zh-cn_topic_0062207359_section41401397"></a>

请求样例

```
DELETE https://{Endpoint}/v2.0/ports/2b098395-046a-4071-b009-312bcee665cb 
```

响应样例

无

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

