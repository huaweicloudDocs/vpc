# 查询VPC<a name="ZH-CN_TOPIC_0201534259"></a>

## 功能介绍<a name="section48604061"></a>

查询虚拟私有云。

## URI<a name="section34783366"></a>

GET /v1/\{project\_id\}/vpcs/\{vpc\_id\}

参数说明请参见[表1](#table26431778)。

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
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
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

    ```
    GET https://{Endpoint}/v1/{project_id}/vpcs/99d9d709-8478-4b46-9f3f-2206b1023fd3
    ```


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
    <td class="cellrowborder" valign="top" width="24.16%" headers="mcps1.2.4.1.2 "><p id="p41691159213"><a name="p41691159213"></a><a name="p41691159213"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.49999999999999%" headers="mcps1.2.4.1.3 "><p id="p652911041556"><a name="p652911041556"></a><a name="p652911041556"></a><a href="#table1945411214515">vpc对象</a></p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  vpc对象

    <a name="table1945411214515"></a>
    <table><thead align="left"><tr id="row15454222515"><th class="cellrowborder" valign="top" width="21.66%" id="mcps1.2.4.1.1"><p id="p164549255115"><a name="p164549255115"></a><a name="p164549255115"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.32%" id="mcps1.2.4.1.2"><p id="p15454182165114"><a name="p15454182165114"></a><a name="p15454182165114"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.02%" id="mcps1.2.4.1.3"><p id="p1045413215513"><a name="p1045413215513"></a><a name="p1045413215513"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1945414213517"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p64541721513"><a name="p64541721513"></a><a name="p64541721513"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p134540217519"><a name="p134540217519"></a><a name="p134540217519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><p id="p17454223516"><a name="p17454223516"></a><a name="p17454223516"></a>uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row54543212511"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p1145412211516"><a name="p1145412211516"></a><a name="p1145412211516"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p645413265113"><a name="p645413265113"></a><a name="p645413265113"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><a name="ul951112614463"></a><a name="ul951112614463"></a><ul id="ul951112614463"><li>功能说明：虚拟私有云名称</li><li>取值范围：0-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li><li>约束：如果名称不为空，则同一个租户下的名称不能重复</li></ul>
    </td>
    </tr>
    <tr id="row57274330378"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p572773313373"><a name="p572773313373"></a><a name="p572773313373"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p272783315379"><a name="p272783315379"></a><a name="p272783315379"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><a name="ul621614305363"></a><a name="ul621614305363"></a><ul id="ul621614305363"><li>功能说明：虚拟私有云描述</li><li>取值范围：0-255个字符，不能包含“&lt;”和“&gt;”。</li></ul>
    </td>
    </tr>
    <tr id="row445515275116"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p545592185110"><a name="p545592185110"></a><a name="p545592185110"></a>cidr</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p745592125117"><a name="p745592125117"></a><a name="p745592125117"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><a name="ul10389173917465"></a><a name="ul10389173917465"></a><ul id="ul10389173917465"><li>功能说明：虚拟私有云下可用子网的范围</li><li>取值范围：<a name="ul53161626155413"></a><a name="ul53161626155413"></a><ul id="ul53161626155413"><li>10.0.0.0/8~10.255.255.240/28</li><li>172.16.0.0/12 ~ 172.31.255.240/28</li><li>192.168.0.0/16 ~ 192.168.255.240/28</li></ul>
    </li><li>不指定cidr时，默认值为空</li><li>约束：必须是cidr格式，例如:192.168.0.0/16</li></ul>
    </td>
    </tr>
    <tr id="row645513212511"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p124551621516"><a name="p124551621516"></a><a name="p124551621516"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p1545552115110"><a name="p1545552115110"></a><a name="p1545552115110"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><a name="ul74552213513"></a><a name="ul74552213513"></a><ul id="ul74552213513"><li>功能说明：虚拟私有云的状态。</li><li>取值范围：<a name="ul5890854165417"></a><a name="ul5890854165417"></a><ul id="ul5890854165417"><li>CREATING：创建中</li><li>OK：创建成功</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row134563245111"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p145614219511"><a name="p145614219511"></a><a name="p145614219511"></a>routes</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p539717333282"><a name="p539717333282"></a><a name="p539717333282"></a>Array of <a href="#table3576833291556">route</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><a name="ul34563265116"></a><a name="ul34563265116"></a><ul id="ul34563265116"><li>功能说明：路由信息列表。</li><li>约束：详情参见<a href="#table3576833291556">route对象</a>。</li></ul>
    </td>
    </tr>
    <tr id="row1345682125118"><td class="cellrowborder" valign="top" width="21.66%" headers="mcps1.2.4.1.1 "><p id="p14456162195113"><a name="p14456162195113"></a><a name="p14456162195113"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.2.4.1.2 "><p id="p24567210516"><a name="p24567210516"></a><a name="p24567210516"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.02%" headers="mcps1.2.4.1.3 "><a name="ul44565215110"></a><a name="ul44565215110"></a><ul id="ul44565215110"><li>功能说明：企业项目ID。</li><li>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  route对象

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
            "description": "test",
            "cidr": "192.168.0.0/16",
            "status": "OK",
            "enterprise_project_id": "0" ,
            "routes": []
    }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

