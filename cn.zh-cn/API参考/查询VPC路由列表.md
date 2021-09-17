# 查询VPC路由列表<a name="vpc_route_0001"></a>

## 功能介绍<a name="section162841743131116"></a>

查询提交请求的租户的所有路由列表，并根据过滤条件进行过滤。分页查询响应格式请参考[分页查询](分页查询.md)。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=ListVpcRoutes)中直接运行调试该接口。

## URI<a name="section1828464319118"></a>

GET /v2.0/vpc/routes

样例：

```
样例：
GET https://{Endpoint}/v2.0/vpc/routes?id={id}&vpc_id={vpc_id}&tenant_id={tenant_id}&destination={destination}&type={type}&limit={limit}&marker={marker}
```

参数说明请参见[表1](#table1256815152114)。

**表 1**  参数说明

<a name="table1256815152114"></a>
<table><thead align="left"><tr id="row2066671591116"><th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.2.5.1.1"><p id="p1466620159113"><a name="p1466620159113"></a><a name="p1466620159113"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.2"><p id="p0666015121119"><a name="p0666015121119"></a><a name="p0666015121119"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="27.27272727272727%" id="mcps1.2.5.1.3"><p id="p966631501115"><a name="p966631501115"></a><a name="p966631501115"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.36363636363636%" id="mcps1.2.5.1.4"><p id="p14666615171112"><a name="p14666615171112"></a><a name="p14666615171112"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row06661515151115"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1666681551120"><a name="p1666681551120"></a><a name="p1666681551120"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p12666151515113"><a name="p12666151515113"></a><a name="p12666151515113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p66664158117"><a name="p66664158117"></a><a name="p66664158117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p16661715101119"><a name="p16661715101119"></a><a name="p16661715101119"></a>按照routes_id过滤查询</p>
</td>
</tr>
<tr id="row10666515101113"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p5482113610377"><a name="p5482113610377"></a><a name="p5482113610377"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p11666815111120"><a name="p11666815111120"></a><a name="p11666815111120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p146661615161112"><a name="p146661615161112"></a><a name="p146661615161112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p1066641513118"><a name="p1066641513118"></a><a name="p1066641513118"></a>按照tenant_id过滤查询</p>
</td>
</tr>
<tr id="row19666101515116"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p866631561113"><a name="p866631561113"></a><a name="p866631561113"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p1666616153117"><a name="p1666616153117"></a><a name="p1666616153117"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p18666215201119"><a name="p18666215201119"></a><a name="p18666215201119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p466651510117"><a name="p466651510117"></a><a name="p466651510117"></a>按照vpc_id过滤查询</p>
</td>
</tr>
<tr id="row14666415101111"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1066681561114"><a name="p1066681561114"></a><a name="p1066681561114"></a>destination</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p166671571112"><a name="p166671571112"></a><a name="p166671571112"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p1266681521114"><a name="p1266681521114"></a><a name="p1266681521114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p466671561110"><a name="p466671561110"></a><a name="p466671561110"></a>按照路由目的地址CIDR过滤查询</p>
</td>
</tr>
<tr id="row186663151117"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p56661015111110"><a name="p56661015111110"></a><a name="p56661015111110"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p17666151515114"><a name="p17666151515114"></a><a name="p17666151515114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p1566641571117"><a name="p1566641571117"></a><a name="p1566641571117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p1666610159113"><a name="p1666610159113"></a><a name="p1666610159113"></a>按照type进行过滤查询，目前只支持peering</p>
</td>
</tr>
<tr id="row12666615181111"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p17666191551117"><a name="p17666191551117"></a><a name="p17666191551117"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p2666131513115"><a name="p2666131513115"></a><a name="p2666131513115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p15666715171118"><a name="p15666715171118"></a><a name="p15666715171118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p28526205175853"><a name="p28526205175853"></a><a name="p28526205175853"></a>分页查询的起始资源ID，表示从指定资源的下一条记录开始查询。</p>
<p id="p538818488578"><a name="p538818488578"></a><a name="p538818488578"></a>marker需要和limit配合使用：</p>
<a name="ul12704811125810"></a><a name="ul12704811125810"></a><ul id="ul12704811125810"><li>若不传入marker和limit参数，查询结果返回全部资源记录。</li><li>若不传入marker参数，limit为10，查询结果返回第1~10条资源记录。</li><li>若marker为第10条记录的资源ID，limit为10，查询结果返回第11~20条资源记录。</li><li>若marker为第10条记录的资源ID，不传入limit参数，查询结果返回第11条及之后的所有资源记录。</li></ul>
</td>
</tr>
<tr id="row1666661561117"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1666121531117"><a name="p1666121531117"></a><a name="p1666121531117"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p66667156117"><a name="p66667156117"></a><a name="p66667156117"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p12666111514118"><a name="p12666111514118"></a><a name="p12666111514118"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p2017153116589"><a name="p2017153116589"></a><a name="p2017153116589"></a>分页查询每页返回的记录个数，取值范围为0~intmax。</p>
<p id="p125192338584"><a name="p125192338584"></a><a name="p125192338584"></a>limit需要和marker配合使用，详细规则请见marker的参数说明。</p>
<p id="p11472454669"><a name="p11472454669"></a><a name="p11472454669"></a>默认值为2000。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section229194351110"></a>

-   请求参数

    无


-   请求样例

    ```
    GET https://{Endpoint}/v2.0/vpc/routes?vpc_id=ab78be2d-782f-42a5-aa72-35879f6890ff
    ```


## 响应消息<a name="section12916437119"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table10292143181119"></a>
    <table><thead align="left"><tr id="row5437104312112"><th class="cellrowborder" valign="top" width="18.82%" id="mcps1.2.4.1.1"><p id="p19437124311115"><a name="p19437124311115"></a><a name="p19437124311115"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.709999999999997%" id="mcps1.2.4.1.2"><p id="p3437243191113"><a name="p3437243191113"></a><a name="p3437243191113"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.2.4.1.3"><p id="p8437174311112"><a name="p8437174311112"></a><a name="p8437174311112"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1443754317116"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.2.4.1.1 "><p id="p8437643101115"><a name="p8437643101115"></a><a name="p8437643101115"></a>routes</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.709999999999997%" headers="mcps1.2.4.1.2 "><p id="p20437343121112"><a name="p20437343121112"></a><a name="p20437343121112"></a>Array of <a href="#table05001250111">route</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.2.4.1.3 "><p id="p16438204318114"><a name="p16438204318114"></a><a name="p16438204318114"></a>route对象列表，参见<a href="#table05001250111">表3</a>。</p>
    </td>
    </tr>
    <tr id="row61512449419"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.2.4.1.1 "><p id="p7152194417414"><a name="p7152194417414"></a><a name="p7152194417414"></a>routes_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.709999999999997%" headers="mcps1.2.4.1.2 "><p id="p14152154444113"><a name="p14152154444113"></a><a name="p14152154444113"></a>Array of <a href="#table25150247450">routes_link</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.2.4.1.3 "><p id="p44238379436"><a name="p44238379436"></a><a name="p44238379436"></a>routes_link对象列表，参见<a href="#table25150247450">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  route对象

    <a name="table05001250111"></a>
    <table><thead align="left"><tr id="row1604152531116"><th class="cellrowborder" valign="top" width="19.321932193219325%" id="mcps1.2.4.1.1"><p id="p19605525151115"><a name="p19605525151115"></a><a name="p19605525151115"></a>属性</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.172417241724172%" id="mcps1.2.4.1.2"><p id="p2060572511111"><a name="p2060572511111"></a><a name="p2060572511111"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.5056505650565%" id="mcps1.2.4.1.3"><p id="p11605425111120"><a name="p11605425111120"></a><a name="p11605425111120"></a>说明</p>
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
    <tr id="row19605192511115"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p1160582510117"><a name="p1160582510117"></a><a name="p1160582510117"></a>destination</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p186051725131113"><a name="p186051725131113"></a><a name="p186051725131113"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p20605425121118"><a name="p20605425121118"></a><a name="p20605425121118"></a>路由目的地址CIDR，如192.168.200.0/24。</p>
    </td>
    </tr>
    <tr id="row160513252111"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p76051225121114"><a name="p76051225121114"></a><a name="p76051225121114"></a>nexthop</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p1460592591111"><a name="p1460592591111"></a><a name="p1460592591111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p487414894012"><a name="p487414894012"></a><a name="p487414894012"></a>路由下一跳，如果路由是“peering”类型，填写vpc peering id。</p>
    </td>
    </tr>
    <tr id="row26061325191110"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p86067257112"><a name="p86067257112"></a><a name="p86067257112"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p260619251118"><a name="p260619251118"></a><a name="p260619251118"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p9916134014397"><a name="p9916134014397"></a><a name="p9916134014397"></a>路由类型。目前只支持“peering”。</p>
    </td>
    </tr>
    <tr id="row11606125111110"><td class="cellrowborder" valign="top" width="19.321932193219325%" headers="mcps1.2.4.1.1 "><p id="p12606162501119"><a name="p12606162501119"></a><a name="p12606162501119"></a>vpc_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.172417241724172%" headers="mcps1.2.4.1.2 "><p id="p06061925181119"><a name="p06061925181119"></a><a name="p06061925181119"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.5056505650565%" headers="mcps1.2.4.1.3 "><p id="p9606112519111"><a name="p9606112519111"></a><a name="p9606112519111"></a>路由的vpc，需要填写存在的vpc_id。</p>
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

    **表 4**  routes\_link对象

    <a name="table25150247450"></a>
    <table><thead align="left"><tr id="row10561424184513"><th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.1"><p id="p15562102474514"><a name="p15562102474514"></a><a name="p15562102474514"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.2"><p id="p656212464511"><a name="p656212464511"></a><a name="p656212464511"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="71.72%" id="mcps1.2.4.1.3"><p id="p856220242456"><a name="p856220242456"></a><a name="p856220242456"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3562132464511"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p13562224194510"><a name="p13562224194510"></a><a name="p13562224194510"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p556214245453"><a name="p556214245453"></a><a name="p556214245453"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p145623247454"><a name="p145623247454"></a><a name="p145623247454"></a>API链接</p>
    </td>
    </tr>
    <tr id="row656292454519"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p1756252484511"><a name="p1756252484511"></a><a name="p1756252484511"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p056210247459"><a name="p056210247459"></a><a name="p056210247459"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p75621724194516"><a name="p75621724194516"></a><a name="p75621724194516"></a>API链接与该API版本的关系</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    { 
      "routes": [ 
        { 
          "type": "peering",  
          "nexthop": "60c809cb-6731-45d0-ace8-3bf5626421a9",  
          "destination": "192.168.200.0/24",  
          "vpc_id": "ab78be2d-782f-42a5-aa72-35879f6890ff",  
          "tenant_id": "6fbe9263116a4b68818cf1edce16bc4f",
          "id": "3d42a0d4-a980-4613-ae76-a2cddecff054" 
        }
      ] 
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

