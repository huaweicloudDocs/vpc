# 删除网络ACL组<a name="ZH-CN_TOPIC_0060574393"></a>

## 功能介绍<a name="section12785655132831"></a>

删除网络ACL组。

## URI<a name="section23213218132831"></a>

DELETE /v2.0/fwaas/firewall\_groups/\{firewall\_group\_id\}

**表 1**  参数说明

<a name="table18880184689"></a>
<table><thead align="left"><tr id="row13968641385"><th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.2.5.1.1"><p id="p209684410817"><a name="p209684410817"></a><a name="p209684410817"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.2"><p id="p69681441386"><a name="p69681441386"></a><a name="p69681441386"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="27.27272727272727%" id="mcps1.2.5.1.3"><p id="p1096813412811"><a name="p1096813412811"></a><a name="p1096813412811"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.36363636363636%" id="mcps1.2.5.1.4"><p id="p139686416813"><a name="p139686416813"></a><a name="p139686416813"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19681041189"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1682422682817"><a name="p1682422682817"></a><a name="p1682422682817"></a>firewall_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p1797015416817"><a name="p1797015416817"></a><a name="p1797015416817"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p19701411813"><a name="p19701411813"></a><a name="p19701411813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p109701641488"><a name="p109701641488"></a><a name="p109701641488"></a>网络ACL组唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section32219668132831"></a>

无。

## 响应消息<a name="section64705436132831"></a>

无。

## 样例<a name="section18785711132831"></a>

请求样例

```
DELETE /v2.0/fwaas/firewall_groups/0415f554-26ed-44e7-a881-bdf4e6216e38
```

响应样例

无。

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

