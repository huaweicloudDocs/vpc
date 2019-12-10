# 删除私有IP<a name="ZH-CN_TOPIC_0201534084"></a>

## 功能介绍<a name="section1933992"></a>

删除私有IP。

## URI<a name="section17405935"></a>

DELETE /v1/\{project\_id\}/privateips/\{privateip\_id\}

参数说明请参见[表1](#table24633528)。

**表 1**  参数说明

<a name="table24633528"></a>
<table><thead align="left"><tr id="row5608311"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p51620080"><a name="p51620080"></a><a name="p51620080"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p20476957"><a name="p20476957"></a><a name="p20476957"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p48020839"><a name="p48020839"></a><a name="p48020839"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row64482741"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p55719536"><a name="p55719536"></a><a name="p55719536"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p16988543"><a name="p16988543"></a><a name="p16988543"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row36617123"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p13196948"><a name="p13196948"></a><a name="p13196948"></a>privateip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p62319862"><a name="p62319862"></a><a name="p62319862"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p14744048"><a name="p14744048"></a><a name="p14744048"></a>私有IP唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section22435692"></a>

-   请求参数

    无

-   请求样例

    ```
    DELETE https://{Endpoint}/v1/{project_id}/privateips/4779ab1c-7c1a-44b1-a02e-93dfc361b32d
    ```


## 响应消息<a name="section594640"></a>

-   请求参数

    无

-   响应样例

    ```
    无
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

