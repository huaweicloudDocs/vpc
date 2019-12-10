# 创建VPC<a name="ZH-CN_TOPIC_0201534275"></a>

## 功能介绍<a name="section20114008"></a>

创建虚拟私有云。

## URI<a name="section46808346"></a>

POST /v1/\{project\_id\}/vpcs

参数说明请参见[表1](#table3672032)。

**表 1**  参数说明

<a name="table3672032"></a>
<table><thead align="left"><tr id="row10026740"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p6859639"><a name="p6859639"></a><a name="p6859639"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p18759866"><a name="p18759866"></a><a name="p18759866"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p43154149"><a name="p43154149"></a><a name="p43154149"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5825185"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p2077973"><a name="p2077973"></a><a name="p2077973"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p34098154"><a name="p34098154"></a><a name="p34098154"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section18621933"></a>

-   请求参数

    **表 2**  请求参数

    <a name="table59675338144730"></a>
    <table><thead align="left"><tr id="row22732874144730"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="p29423469144730"><a name="p29423469144730"></a><a name="p29423469144730"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="p34490826144730"><a name="p34490826144730"></a><a name="p34490826144730"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.8%" id="mcps1.2.5.1.3"><p id="p42293511144730"><a name="p42293511144730"></a><a name="p42293511144730"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.81%" id="mcps1.2.5.1.4"><p id="p3222348144730"><a name="p3222348144730"></a><a name="p3222348144730"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59683650144730"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p2537488144730"><a name="p2537488144730"></a><a name="p2537488144730"></a>vpc</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p4210015144730"><a name="p4210015144730"></a><a name="p4210015144730"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.8%" headers="mcps1.2.5.1.3 "><p id="p41691159213"><a name="p41691159213"></a><a name="p41691159213"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.81%" headers="mcps1.2.5.1.4 "><p id="p32639071144730"><a name="p32639071144730"></a><a name="p32639071144730"></a><a href="#table33750194">vpc对象</a></p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  vpc对象

    <a name="table33750194"></a>
    <table><thead align="left"><tr id="row51192804"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="p52976421"><a name="p52976421"></a><a name="p52976421"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="p63231703"><a name="p63231703"></a><a name="p63231703"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.73%" id="mcps1.2.5.1.3"><p id="p2491821616557"><a name="p2491821616557"></a><a name="p2491821616557"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.88%" id="mcps1.2.5.1.4"><p id="p21494305"><a name="p21494305"></a><a name="p21494305"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row63317164"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p28416672"><a name="p28416672"></a><a name="p28416672"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p20049059"><a name="p20049059"></a><a name="p20049059"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.3 "><p id="p510960516557"><a name="p510960516557"></a><a name="p510960516557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.88%" headers="mcps1.2.5.1.4 "><a name="ul122583362468"></a><a name="ul122583362468"></a><ul id="ul122583362468"><li>功能说明：虚拟私有云名称</li><li>取值范围：0-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li><li>约束：如果名称不为空，则同一个租户下的名称不能重复</li></ul>
    </td>
    </tr>
    <tr id="row1034214180910"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p19990426299"><a name="p19990426299"></a><a name="p19990426299"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p149901726897"><a name="p149901726897"></a><a name="p149901726897"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.3 "><p id="p59901262916"><a name="p59901262916"></a><a name="p59901262916"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.88%" headers="mcps1.2.5.1.4 "><a name="ul49905267911"></a><a name="ul49905267911"></a><ul id="ul49905267911"><li>功能说明：虚拟私有云的描述</li><li>取值范围：0-255个字符，不能包含“&lt;”和“&gt;”。</li></ul>
    </td>
    </tr>
    <tr id="row18134306"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p59592696"><a name="p59592696"></a><a name="p59592696"></a>cidr</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p62279078"><a name="p62279078"></a><a name="p62279078"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.3 "><p id="p1122484216557"><a name="p1122484216557"></a><a name="p1122484216557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.88%" headers="mcps1.2.5.1.4 "><a name="ul10389173917465"></a><a name="ul10389173917465"></a><ul id="ul10389173917465"><li>功能说明：虚拟私有云下可用子网的范围</li><li>取值范围：<a name="ul53161626155413"></a><a name="ul53161626155413"></a><ul id="ul53161626155413"><li>10.0.0.0/8~10.255.255.240/28</li><li>172.16.0.0/12 ~ 172.31.255.240/28</li><li>192.168.0.0/16 ~ 192.168.255.240/28</li></ul>
    </li><li>不指定cidr时，默认值为空</li><li>约束：必须是cidr格式，例如:192.168.0.0/16</li></ul>
    </td>
    </tr>
    <tr id="row14131555104815"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p315455194820"><a name="p315455194820"></a><a name="p315455194820"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p101514558488"><a name="p101514558488"></a><a name="p101514558488"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.3 "><p id="p171555513485"><a name="p171555513485"></a><a name="p171555513485"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.88%" headers="mcps1.2.5.1.4 "><a name="ul6464125124610"></a><a name="ul6464125124610"></a><ul id="ul6464125124610"><li>功能说明：企业项目ID。创建虚拟私有云时，给虚拟私有云绑定企业项目ID。</li><li>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。</li></ul>
    <div class="note" id="note61091327154914"><a name="note61091327154914"></a><a name="note61091327154914"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1915862704914"><a name="p1915862704914"></a><a name="p1915862704914"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0126101490.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    POST https://{Endpoint}/v1/{project_id}/vpcs
    
    {
        "vpc": {
            "name": "vpc",
            "description": "test",
            "cidr": "192.168.0.0/16",
            "enterprise_project_id": "0aad99bc-f5f6-4f78-8404-c598d76b0ed2"
        }
    }
    ```


## 响应消息<a name="section33379675"></a>

-   响应参数

    **表 4**  响应参数

    <a name="table1969410815449"></a>
    <table><thead align="left"><tr id="row2499368515449"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p1122260615449"><a name="p1122260615449"></a><a name="p1122260615449"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.15%" id="mcps1.2.4.1.2"><p id="p1310021915449"><a name="p1310021915449"></a><a name="p1310021915449"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="59.51%" id="mcps1.2.4.1.3"><p id="p5448479815449"><a name="p5448479815449"></a><a name="p5448479815449"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5119248915449"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p5295094915449"><a name="p5295094915449"></a><a name="p5295094915449"></a>vpc</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.15%" headers="mcps1.2.4.1.2 "><p id="p18458338205916"><a name="p18458338205916"></a><a name="p18458338205916"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="59.51%" headers="mcps1.2.4.1.3 "><p id="p393482915449"><a name="p393482915449"></a><a name="p393482915449"></a><a href="#table39714111">vpc对象</a></p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  vpc对象

    <a name="table39714111"></a>
    <table><thead align="left"><tr id="row36411928"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.4.1.1"><p id="p63685038"><a name="p63685038"></a><a name="p63685038"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="23%" id="mcps1.2.4.1.2"><p id="p3336232165612"><a name="p3336232165612"></a><a name="p3336232165612"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p17753217"><a name="p17753217"></a><a name="p17753217"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row28724493"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p44982630"><a name="p44982630"></a><a name="p44982630"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.4.1.2 "><p id="p1799372165612"><a name="p1799372165612"></a><a name="p1799372165612"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p53364125"><a name="p53364125"></a><a name="p53364125"></a>uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row10515080"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p46415143"><a name="p46415143"></a><a name="p46415143"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.4.1.2 "><p id="p11531473165612"><a name="p11531473165612"></a><a name="p11531473165612"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><a name="ul951112614463"></a><a name="ul951112614463"></a><ul id="ul951112614463"><li>功能说明：虚拟私有云名称</li><li>取值范围：0-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li><li>约束：如果名称不为空，则同一个租户下的名称不能重复</li></ul>
    </td>
    </tr>
    <tr id="row1228919121119"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p10612132071113"><a name="p10612132071113"></a><a name="p10612132071113"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.4.1.2 "><p id="p9612132031119"><a name="p9612132031119"></a><a name="p9612132031119"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><a name="ul56121201111"></a><a name="ul56121201111"></a><ul id="ul56121201111"><li>功能说明：虚拟私有云描述</li><li>取值范围：0-255个字符，不能包含“&lt;”和“&gt;”。</li></ul>
    </td>
    </tr>
    <tr id="row19659738"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p48934940"><a name="p48934940"></a><a name="p48934940"></a>cidr</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.4.1.2 "><p id="p61634143165612"><a name="p61634143165612"></a><a name="p61634143165612"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><a name="ul62941023970"></a><a name="ul62941023970"></a><ul id="ul62941023970"><li>功能说明：虚拟私有云下可用子网的范围</li><li>取值范围：<a name="ul162941223376"></a><a name="ul162941223376"></a><ul id="ul162941223376"><li>10.0.0.0/8~10.255.255.240/28</li><li>172.16.0.0/12 ~ 172.31.255.240/28</li><li>192.168.0.0/16 ~ 192.168.255.240/28</li></ul>
    </li><li>不指定cidr时，默认值为空</li><li>约束：必须是cidr格式，例如:192.168.0.0/16</li></ul>
    </td>
    </tr>
    <tr id="row55195381"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p41640866"><a name="p41640866"></a><a name="p41640866"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.4.1.2 "><p id="p26309661165612"><a name="p26309661165612"></a><a name="p26309661165612"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><a name="ul14742195924610"></a><a name="ul14742195924610"></a><ul id="ul14742195924610"><li>功能说明：虚拟私有云的状态</li><li>取值范围：<a name="ul87091357163310"></a><a name="ul87091357163310"></a><ul id="ul87091357163310"><li>CREATING：创建中。</li><li>OK：创建成功。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row680983192136"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p55159683192136"><a name="p55159683192136"></a><a name="p55159683192136"></a>routes</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.4.1.2 "><p id="p51691433192136"><a name="p51691433192136"></a><a name="p51691433192136"></a>Array of <a href="#table3576833291556">route</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><a name="ul088823124710"></a><a name="ul088823124710"></a><ul id="ul088823124710"><li>功能说明：路由信息列表</li><li>约束：详情参见<a href="#table3576833291556">route对象</a>。</li></ul>
    </td>
    </tr>
    <tr id="row14513192217564"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p195139222567"><a name="p195139222567"></a><a name="p195139222567"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.2.4.1.2 "><p id="p151332225616"><a name="p151332225616"></a><a name="p151332225616"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><a name="ul2680192019477"></a><a name="ul2680192019477"></a><ul id="ul2680192019477"><li>功能说明：企业项目ID。</li><li>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  route对象

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
    <td class="cellrowborder" valign="top" width="59.28%" headers="mcps1.2.4.1.3 "><a name="ul391783612478"></a><a name="ul391783612478"></a><ul id="ul391783612478"><li>功能说明：路由目的网段</li><li>约束：必须是cidr格式，且目前只支持0.0.0.0/0</li></ul>
    </td>
    </tr>
    <tr id="row6565233911054"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p1623922311054"><a name="p1623922311054"></a><a name="p1623922311054"></a>nexthop</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.2 "><p id="p4377761311054"><a name="p4377761311054"></a><a name="p4377761311054"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59.28%" headers="mcps1.2.4.1.3 "><a name="ul10508545114715"></a><a name="ul10508545114715"></a><ul id="ul10508545114715"><li>功能说明：路由下一跳地址</li><li>约束：必须为IP地址格式，且必须属于本VPC下的子网范围内才能生效</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
     "vpc": 
         {
         "id": "99d9d709-8478-4b46-9f3f-2206b1023fd3",
         "name": "vpc",
         "description": "test",
         "cidr": "192.168.0.0/16",
         "status": "CREATING",
         "enterprise_project_id": "0aad99bc-f5f6-4f78-8404-c598d76b0ed2", 
         "routes": []
         }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

