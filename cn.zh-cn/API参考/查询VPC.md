# 查询VPC<a name="ZH-CN_TOPIC_0020090618"></a>

## 功能介绍<a name="section48604061"></a>

查询虚拟私有云。

## URI<a name="section34783366"></a>

GET /v1/\{project\_id\}/vpcs/\{vpc\_id\}

**表 1**  参数说明

<a name="table26431778"></a>
<table><thead align="left"><tr id="row38955607"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p1287621"><a name="p1287621"></a><a name="p1287621"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p37188451"><a name="p37188451"></a><a name="p37188451"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p59474521"><a name="p59474521"></a><a name="p59474521"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row52706896"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p41400175"><a name="p41400175"></a><a name="p41400175"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p65079903"><a name="p65079903"></a><a name="p65079903"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p36980808"><a name="p36980808"></a><a name="p36980808"></a>项目ID</p>
</td>
</tr>
<tr id="row64391817"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p48354649"><a name="p48354649"></a><a name="p48354649"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p24412469"><a name="p24412469"></a><a name="p24412469"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p31252998"><a name="p31252998"></a><a name="p31252998"></a>虚拟私有云唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section44614845"></a>

-   请求参数

    无

-   请求样例

    无


## 响应消息<a name="section65989290"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table574587231556"></a>
    <table><thead align="left"><tr id="row118397001556"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p194916751556"><a name="p194916751556"></a><a name="p194916751556"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.16%" id="mcps1.2.4.1.2"><p id="p424939721556"><a name="p424939721556"></a><a name="p424939721556"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.49999999999999%" id="mcps1.2.4.1.3"><p id="p194597361556"><a name="p194597361556"></a><a name="p194597361556"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row327347841556"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p342718611556"><a name="p342718611556"></a><a name="p342718611556"></a>vpc</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.16%" headers="mcps1.2.4.1.2 "><p id="p429876841556"><a name="p429876841556"></a><a name="p429876841556"></a>字典数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.49999999999999%" headers="mcps1.2.4.1.3 "><p id="p652911041556"><a name="p652911041556"></a><a name="p652911041556"></a>vpc对象</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  vpc字段说明

    <a name="table53205180"></a>
    <table><thead align="left"><tr id="row33959011"><th class="cellrowborder" valign="top" width="21.66%" id="mcps1.2.4.1.1"><p id="p66325402"><a name="p66325402"></a><a name="p66325402"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.32%" id="mcps1.2.4.1.2"><p id="p13682832174258"><a name="p13682832174258"></a><a name="p13682832174258"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.02%" id="mcps1.2.4.1.3"><p id="p27088563"><a name="p27088563"></a><a name="p27088563"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row46690023"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p23795519"><a name="p23795519"></a><a name="p23795519"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p34567587174258"><a name="p34567587174258"></a><a name="p34567587174258"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><p id="p27186813"><a name="p27186813"></a><a name="p27186813"></a>uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row43354729"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p22072140"><a name="p22072140"></a><a name="p22072140"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p48511134174258"><a name="p48511134174258"></a><a name="p48511134174258"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><p id="p61491827"><a name="p61491827"></a><a name="p61491827"></a>虚拟私有云名称。</p>
    </td>
    </tr>
    <tr id="row16555535"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p65929926"><a name="p65929926"></a><a name="p65929926"></a>cidr</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p37087786174258"><a name="p37087786174258"></a><a name="p37087786174258"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><p id="p49620939"><a name="p49620939"></a><a name="p49620939"></a>虚拟私有云下可用子网的范围。</p>
    </td>
    </tr>
    <tr id="row43935272"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p1987246"><a name="p1987246"></a><a name="p1987246"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p51320686174258"><a name="p51320686174258"></a><a name="p51320686174258"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><a name="ul16729126124815"></a><a name="ul16729126124815"></a><ul id="ul16729126124815"><li>功能说明：虚拟私有云的状态。</li><li>取值范围：创建中CREATING，创建成功OK</li></ul>
    </td>
    </tr>
    <tr id="row11226980135054"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p36970168135054"><a name="p36970168135054"></a><a name="p36970168135054"></a>routes</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p29840430135054"><a name="p29840430135054"></a><a name="p29840430135054"></a>List</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><a name="ul491764954811"></a><a name="ul491764954811"></a><ul id="ul491764954811"><li>功能说明：路由信息列表。</li><li>约束：详情参见route对象。</li></ul>
    </td>
    </tr>
    <tr id="row440413369017"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p9278134112013"><a name="p9278134112013"></a><a name="p9278134112013"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p1027811411302"><a name="p1027811411302"></a><a name="p1027811411302"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><a name="ul10977141512493"></a><a name="ul10977141512493"></a><ul id="ul10977141512493"><li>功能说明：企业项目ID。</li><li>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。</li></ul>
    <div class="note" id="note1823412419013"><a name="note1823412419013"></a><a name="note1823412419013"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1727974116010"><a name="p1727974116010"></a><a name="p1727974116010"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见《企业资源服务用户指南》。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  route字段说明

    <a name="table3576833291556"></a>
    <table><thead align="left"><tr id="row921218691556"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p798956991556"><a name="p798956991556"></a><a name="p798956991556"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.38%" id="mcps1.2.4.1.2"><p id="p754435891556"><a name="p754435891556"></a><a name="p754435891556"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="59.28%" id="mcps1.2.4.1.3"><p id="p711326791556"><a name="p711326791556"></a><a name="p711326791556"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3930377391556"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p2948903591556"><a name="p2948903591556"></a><a name="p2948903591556"></a>destination</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.2 "><p id="p270722191556"><a name="p270722191556"></a><a name="p270722191556"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59.28%" headers="mcps1.2.4.1.3 "><a name="ul15801323493"></a><a name="ul15801323493"></a><ul id="ul15801323493"><li>功能说明：路由目的网段</li><li>约束：必须是cidr格式，且目前只支持0.0.0.0/0</li></ul>
    </td>
    </tr>
    <tr id="row6565233911054"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p1623922311054"><a name="p1623922311054"></a><a name="p1623922311054"></a>nexthop</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.2 "><p id="p4377761311054"><a name="p4377761311054"></a><a name="p4377761311054"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59.28%" headers="mcps1.2.4.1.3 "><a name="ul1344883624911"></a><a name="ul1344883624911"></a><ul id="ul1344883624911"><li>功能说明：路由下一跳地址</li><li>约束：必须为IP地址格式，且必须属于本VPC下的子网范围内才能生效</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "vpc": {
            "id": "99d9d709-8478-4b46-9f3f-2206b1023fd3",
            "name": "vpc",
            "cidr": "192.168.0.0/16",
            "status": "OK",
            "enterprise_project_id": "0" 
            "routes": null,
    }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

