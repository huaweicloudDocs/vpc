# 删除端口<a name="zh-cn_topic_0062207810"></a>

## 功能介绍<a name="zh-cn_topic_0062207359_section45238241"></a>

删除端口。

接口约束：

-   不允许删除device\_owner为非空且不为neutron:VIP\_PORT的端口。
-   不允许删除device\_id为非空的端口。

## URI<a name="zh-cn_topic_0062207359_section4490990"></a>

DELETE /v2.0/ports/\{port\_id\}

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

