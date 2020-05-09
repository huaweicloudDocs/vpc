# 删除VPC<a name="vpc_api01_0005"></a>

## 功能介绍<a name="section15422169"></a>

删除虚拟私有云。

## URI<a name="section4581796"></a>

DELETE /v1/\{project\_id\}/vpcs/\{vpc\_id\}

参数说明请参见[表1](#table47834478)。

**表 1**  参数说明

<a name="table47834478"></a>
<table><thead align="left"><tr id="row29612923"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p49836563"><a name="p49836563"></a><a name="p49836563"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p10229816"><a name="p10229816"></a><a name="p10229816"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p23308753"><a name="p23308753"></a><a name="p23308753"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8960839"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p54739329"><a name="p54739329"></a><a name="p54739329"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p4700647"><a name="p4700647"></a><a name="p4700647"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row4220283"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p6298672"><a name="p6298672"></a><a name="p6298672"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p40430446"><a name="p40430446"></a><a name="p40430446"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p53640668"><a name="p53640668"></a><a name="p53640668"></a>虚拟私有云唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section41236172"></a>

-   请求参数

    无

-   请求样例

    ```
    DELETE https://{Endpoint}/v1/{project_id}/vpcs/13551d6b-755d-4757-b956-536f674975c0
    ```


## 响应消息<a name="section35581233"></a>

-   响应参数

    无


-   响应样例

    无


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

