# 创建VPC路由<a name="ZH-CN_TOPIC_0075677494"></a>

## 功能介绍<a name="section47901846151217"></a>

创建路由。

## URI<a name="section13791164631218"></a>

POST /v2.0/vpc/routes

## 请求消息<a name="section3797746131211"></a>

-   请求参数

    **表 1**  请求参数

    <a name="table1798124601216"></a>
    <table><thead align="left"><tr id="row9947104641211"><th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.1"><p id="p15947546131217"><a name="p15947546131217"></a><a name="p15947546131217"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="8.08%" id="mcps1.2.5.1.2"><p id="p1094744610126"><a name="p1094744610126"></a><a name="p1094744610126"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="8.08%" id="mcps1.2.5.1.3"><p id="p3947104631217"><a name="p3947104631217"></a><a name="p3947104631217"></a>必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="69.69999999999999%" id="mcps1.2.5.1.4"><p id="p17947154661210"><a name="p17947154661210"></a><a name="p17947154661210"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row20947134611120"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.1 "><p id="p1947194618124"><a name="p1947194618124"></a><a name="p1947194618124"></a>route</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="p179478465125"><a name="p179478465125"></a><a name="p179478465125"></a>Dict</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.3 "><p id="p094714468129"><a name="p094714468129"></a><a name="p094714468129"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.5.1.4 "><p id="p16438204318114"><a name="p16438204318114"></a><a name="p16438204318114"></a>route对象列表，参见<a href="VPC路由API简介.md#table05001250111">表1</a>。</p>
    <p id="p189472465121"><a name="p189472465121"></a><a name="p189472465121"></a>必选字段：destination、nexthop、type、vpc_id。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    POST /v2.0/vpc/routes 
    { 
        "route": { 
            "type": "peering",  
            "nexthop": "60c809cb-6731-45d0-ace8-3bf5626421a9",  
            "destination": "192.168.200.0/24",  
            "vpc_id": "ab78be2d-782f-42a5-aa72-35879f6890ff"
        }
    }
    ```


## 响应消息<a name="section1680694610122"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table158077469123"></a>
    <table><thead align="left"><tr id="row994734618124"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p159471246131219"><a name="p159471246131219"></a><a name="p159471246131219"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.48%" id="mcps1.2.4.1.2"><p id="p59471646191212"><a name="p59471646191212"></a><a name="p59471646191212"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="65.16999999999999%" id="mcps1.2.4.1.3"><p id="p12947114615129"><a name="p12947114615129"></a><a name="p12947114615129"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row18947144601211"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p1794734651219"><a name="p1794734651219"></a><a name="p1794734651219"></a>route</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.48%" headers="mcps1.2.4.1.2 "><p id="p19471546151212"><a name="p19471546151212"></a><a name="p19471546151212"></a>Dict</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.16999999999999%" headers="mcps1.2.4.1.3 "><p id="p16548142183616"><a name="p16548142183616"></a><a name="p16548142183616"></a>route对象列表，参见<a href="VPC路由API简介.md#table05001250111">表1</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    { 
        "route": { 
            "type": "peering",  
            "nexthop": "60c809cb-6731-45d0-ace8-3bf5626421a9",  
            "destination": "192.168.200.0/24",  
            "vpc_id": "ab78be2d-782f-42a5-aa72-35879f6890ff",  
            "tenant_id": "6fbe9263116a4b68818cf1edce16bc4f",
            "id": "3d42a0d4-a980-4613-ae76-a2cddecff054" 
        }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

