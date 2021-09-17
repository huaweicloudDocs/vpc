# 创建VPC路由<a name="vpc_route_0003"></a>

## 功能介绍<a name="section47901846151217"></a>

创建路由。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=CreateVpcRoute)中直接运行调试该接口。

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
    <td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.2 "><p id="p179478465125"><a name="p179478465125"></a><a name="p179478465125"></a><a href="创建VPC路由.md">route</a> object</p>
    </td>
    <td class="cellrowborder" valign="top" width="8.08%" headers="mcps1.2.5.1.3 "><p id="p094714468129"><a name="p094714468129"></a><a name="p094714468129"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="69.69999999999999%" headers="mcps1.2.5.1.4 "><p id="p16438204318114"><a name="p16438204318114"></a><a name="p16438204318114"></a>route对象列表，参见<a href="#table05001250111">表2</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  route对象

    <a name="table05001250111"></a>
    <table><thead align="left"><tr id="row1604152531116"><th class="cellrowborder" valign="top" width="21.26%" id="mcps1.2.5.1.1"><p id="p19605525151115"><a name="p19605525151115"></a><a name="p19605525151115"></a>属性</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.66%" id="mcps1.2.5.1.2"><p id="p2060572511111"><a name="p2060572511111"></a><a name="p2060572511111"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.580000000000002%" id="mcps1.2.5.1.3"><p id="p91930461309"><a name="p91930461309"></a><a name="p91930461309"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="37.5%" id="mcps1.2.5.1.4"><p id="p11605425111120"><a name="p11605425111120"></a><a name="p11605425111120"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row19605192511115"><td class="cellrowborder" valign="top" width="21.26%" headers="mcps1.2.5.1.1 "><p id="p1160582510117"><a name="p1160582510117"></a><a name="p1160582510117"></a>destination</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.5.1.2 "><p id="p186051725131113"><a name="p186051725131113"></a><a name="p186051725131113"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.580000000000002%" headers="mcps1.2.5.1.3 "><p id="p1819354623012"><a name="p1819354623012"></a><a name="p1819354623012"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.5%" headers="mcps1.2.5.1.4 "><p id="p20605425121118"><a name="p20605425121118"></a><a name="p20605425121118"></a>路由目的地址CIDR，如192.168.200.0/24。</p>
    </td>
    </tr>
    <tr id="row160513252111"><td class="cellrowborder" valign="top" width="21.26%" headers="mcps1.2.5.1.1 "><p id="p76051225121114"><a name="p76051225121114"></a><a name="p76051225121114"></a>nexthop</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.5.1.2 "><p id="p1460592591111"><a name="p1460592591111"></a><a name="p1460592591111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.580000000000002%" headers="mcps1.2.5.1.3 "><p id="p0193184613307"><a name="p0193184613307"></a><a name="p0193184613307"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.5%" headers="mcps1.2.5.1.4 "><p id="p487414894012"><a name="p487414894012"></a><a name="p487414894012"></a>路由下一跳，如果路由是“peering”类型，填写vpc peering id。</p>
    </td>
    </tr>
    <tr id="row26061325191110"><td class="cellrowborder" valign="top" width="21.26%" headers="mcps1.2.5.1.1 "><p id="p86067257112"><a name="p86067257112"></a><a name="p86067257112"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.5.1.2 "><p id="p260619251118"><a name="p260619251118"></a><a name="p260619251118"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.580000000000002%" headers="mcps1.2.5.1.3 "><p id="p319310462306"><a name="p319310462306"></a><a name="p319310462306"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.5%" headers="mcps1.2.5.1.4 "><p id="p9916134014397"><a name="p9916134014397"></a><a name="p9916134014397"></a>路由类型。目前只支持“peering”。</p>
    </td>
    </tr>
    <tr id="row11606125111110"><td class="cellrowborder" valign="top" width="21.26%" headers="mcps1.2.5.1.1 "><p id="p12606162501119"><a name="p12606162501119"></a><a name="p12606162501119"></a>vpc_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.66%" headers="mcps1.2.5.1.2 "><p id="p06061925181119"><a name="p06061925181119"></a><a name="p06061925181119"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.580000000000002%" headers="mcps1.2.5.1.3 "><p id="p819334617303"><a name="p819334617303"></a><a name="p819334617303"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.5%" headers="mcps1.2.5.1.4 "><p id="p9606112519111"><a name="p9606112519111"></a><a name="p9606112519111"></a>请求创建路由的VPC ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    POST https://{Endpoint}/v2.0/vpc/routes 
    
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

    **表 3**  响应参数

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
    <td class="cellrowborder" valign="top" width="13.48%" headers="mcps1.2.4.1.2 "><p id="p19471546151212"><a name="p19471546151212"></a><a name="p19471546151212"></a><a href="创建VPC路由.md">route</a> object</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.16999999999999%" headers="mcps1.2.4.1.3 "><p id="p16548142183616"><a name="p16548142183616"></a><a name="p16548142183616"></a>route对象列表，参见<a href="#table1163544010410">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  route对象

    <a name="table1163544010410"></a>
    <table><thead align="left"><tr id="row863564014119"><th class="cellrowborder" valign="top" width="19.321932193219325%" id="mcps1.2.4.1.1"><p id="p1463514017412"><a name="p1463514017412"></a><a name="p1463514017412"></a>属性</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.172417241724172%" id="mcps1.2.4.1.2"><p id="p5635240154118"><a name="p5635240154118"></a><a name="p5635240154118"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.5056505650565%" id="mcps1.2.4.1.3"><p id="p563554018417"><a name="p563554018417"></a><a name="p563554018417"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row19605172516117"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p4605625141117"><a name="p4605625141117"></a><a name="p4605625141117"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p4605425191116"><a name="p4605425191116"></a><a name="p4605425191116"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p136051025171110"><a name="p136051025171110"></a><a name="p136051025171110"></a>路由id</p>
    </td>
    </tr>
    <tr id="row9635134015418"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p16354403419"><a name="p16354403419"></a><a name="p16354403419"></a>destination</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p9635164004115"><a name="p9635164004115"></a><a name="p9635164004115"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p1863514018419"><a name="p1863514018419"></a><a name="p1863514018419"></a>路由目的地址CIDR，如192.168.200.0/24。</p>
    </td>
    </tr>
    <tr id="row7635840174120"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p166351040174117"><a name="p166351040174117"></a><a name="p166351040174117"></a>nexthop</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p18635740104120"><a name="p18635740104120"></a><a name="p18635740104120"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p16361640134116"><a name="p16361640134116"></a><a name="p16361640134116"></a>路由下一跳，如果路由是“peering”类型，填写vpc peering id。</p>
    </td>
    </tr>
    <tr id="row1563604034114"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p56361240184111"><a name="p56361240184111"></a><a name="p56361240184111"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p11636174019411"><a name="p11636174019411"></a><a name="p11636174019411"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p14636134094111"><a name="p14636134094111"></a><a name="p14636134094111"></a>路由类型。目前只支持“peering”。</p>
    </td>
    </tr>
    <tr id="row563614017419"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p3636240124118"><a name="p3636240124118"></a><a name="p3636240124118"></a>vpc_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p06361940114114"><a name="p06361940114114"></a><a name="p06361940114114"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p166361940154117"><a name="p166361940154117"></a><a name="p166361940154117"></a>路由的vpc，需要填写存在的vpc_id。</p>
    </td>
    </tr>
    <tr id="row56067256117"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p196065257115"><a name="p196065257115"></a><a name="p196065257115"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p10606182591115"><a name="p10606182591115"></a><a name="p10606182591115"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
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

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

