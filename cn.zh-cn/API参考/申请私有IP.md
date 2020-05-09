# 申请私有IP<a name="vpc_privateip_0001"></a>

## 功能介绍<a name="section31644779"></a>

申请私有IP。

## URI<a name="section16367560"></a>

POST /v1/\{project\_id\}/privateips

参数说明请参见[表1](#table57906226)。

**表 1**  参数说明

<a name="table57906226"></a>
<table><thead align="left"><tr id="row33939988"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p64784526"><a name="p64784526"></a><a name="p64784526"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p13055244"><a name="p13055244"></a><a name="p13055244"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p50841847"><a name="p50841847"></a><a name="p50841847"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row24548918"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p42305330"><a name="p42305330"></a><a name="p42305330"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p4179666"><a name="p4179666"></a><a name="p4179666"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section13090320"></a>

-   请求参数

    **表 2**  请求参数

    <a name="table6906072155755"></a>
    <table><thead align="left"><tr id="row11778955155755"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="p14571261155755"><a name="p14571261155755"></a><a name="p14571261155755"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="p39421508155755"><a name="p39421508155755"></a><a name="p39421508155755"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="p39025608155755"><a name="p39025608155755"></a><a name="p39025608155755"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.18%" id="mcps1.2.5.1.4"><p id="p6957680155755"><a name="p6957680155755"></a><a name="p6957680155755"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row26701221155755"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p15315278155755"><a name="p15315278155755"></a><a name="p15315278155755"></a>privateips</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p32578004155755"><a name="p32578004155755"></a><a name="p32578004155755"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p21572638155755"><a name="p21572638155755"></a><a name="p21572638155755"></a>Array of <a href="#table45335391">privateip</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p22979132155755"><a name="p22979132155755"></a><a name="p22979132155755"></a>私有IP列表对象，请参见<a href="#table45335391">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  privateip字段说明

    <a name="table45335391"></a>
    <table><thead align="left"><tr id="row64244561"><th class="cellrowborder" valign="top" width="16.91830816918308%" id="mcps1.2.5.1.1"><p id="p36426933"><a name="p36426933"></a><a name="p36426933"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.478252174782526%" id="mcps1.2.5.1.2"><p id="p64900454"><a name="p64900454"></a><a name="p64900454"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.04819518048195%" id="mcps1.2.5.1.3"><p id="p2779229717298"><a name="p2779229717298"></a><a name="p2779229717298"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.55524447555245%" id="mcps1.2.5.1.4"><p id="p22445387"><a name="p22445387"></a><a name="p22445387"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row6137036"><td class="cellrowborder" valign="top" width="16.91830816918308%" headers="mcps1.2.5.1.1 "><p id="p27337939"><a name="p27337939"></a><a name="p27337939"></a>subnet_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.478252174782526%" headers="mcps1.2.5.1.2 "><p id="p66889413"><a name="p66889413"></a><a name="p66889413"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.04819518048195%" headers="mcps1.2.5.1.3 "><p id="p3658359317298"><a name="p3658359317298"></a><a name="p3658359317298"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.55524447555245%" headers="mcps1.2.5.1.4 "><p id="p41347315"><a name="p41347315"></a><a name="p41347315"></a>分配IP的子网标识</p>
    </td>
    </tr>
    <tr id="row36581520"><td class="cellrowborder" valign="top" width="16.91830816918308%" headers="mcps1.2.5.1.1 "><p id="p10313144"><a name="p10313144"></a><a name="p10313144"></a>ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.478252174782526%" headers="mcps1.2.5.1.2 "><p id="p30058349"><a name="p30058349"></a><a name="p30058349"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.04819518048195%" headers="mcps1.2.5.1.3 "><p id="p1048103717298"><a name="p1048103717298"></a><a name="p1048103717298"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.55524447555245%" headers="mcps1.2.5.1.4 "><a name="ul10782731123015"></a><a name="ul10782731123015"></a><ul id="ul10782731123015"><li>功能说明：指定IP地址申请</li><li>取值范围：子网网段中的可以使用且未分配的IP地址，不指定时由系统自动分配</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    POST https://{Endpoint}/v1/{project_id}/privateips
    
    {
      "privateips": 
       [ 
        {
            "subnet_id": "531dec0f-3116-411b-a21b-e612e42349fd"
        },
        {
            "subnet_id": "531dec0f-3116-411b-a21b-e612e42349fd",
             "ip_address": "192.168.1.17"
        }
       ]
    }
    ```


## 响应消息<a name="section50704018"></a>

-   响应参数

    **表 4**  响应参数

    <a name="table38560739155852"></a>
    <table><thead align="left"><tr id="row1158370155852"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p26719126155852"><a name="p26719126155852"></a><a name="p26719126155852"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="p15835596155852"><a name="p15835596155852"></a><a name="p15835596155852"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="p7614877155852"><a name="p7614877155852"></a><a name="p7614877155852"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12825332155852"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p32218934155852"><a name="p32218934155852"></a><a name="p32218934155852"></a>privateips</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p26395826172022"><a name="p26395826172022"></a><a name="p26395826172022"></a>Array of <a href="#table34571880">privateip</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p14320614155852"><a name="p14320614155852"></a><a name="p14320614155852"></a>私有IP列表对象，请参见<a href="#table34571880">表5</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  privateip字段说明

    <a name="table34571880"></a>
    <table><thead align="left"><tr id="row51070612"><th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.2.4.1.1"><p id="p43078913"><a name="p43078913"></a><a name="p43078913"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.132813281328133%" id="mcps1.2.4.1.2"><p id="p42083530172955"><a name="p42083530172955"></a><a name="p42083530172955"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.644964496449646%" id="mcps1.2.4.1.3"><p id="p45326617"><a name="p45326617"></a><a name="p45326617"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row47577364"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.4.1.1 "><p id="p28561251"><a name="p28561251"></a><a name="p28561251"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.132813281328133%" headers="mcps1.2.4.1.2 "><p id="p53322749172955"><a name="p53322749172955"></a><a name="p53322749172955"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.644964496449646%" headers="mcps1.2.4.1.3 "><a name="ul13978236183119"></a><a name="ul13978236183119"></a><ul id="ul13978236183119"><li>功能说明：私有IP的状态</li><li>取值范围：<a name="ul948092312377"></a><a name="ul948092312377"></a><ul id="ul948092312377"><li>ACTIVE：活动的</li><li>DOWN：不可用</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row38031802"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.4.1.1 "><p id="p60677108"><a name="p60677108"></a><a name="p60677108"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.132813281328133%" headers="mcps1.2.4.1.2 "><p id="p24175384172955"><a name="p24175384172955"></a><a name="p24175384172955"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.644964496449646%" headers="mcps1.2.4.1.3 "><p id="p47453675"><a name="p47453675"></a><a name="p47453675"></a>私有IP标识</p>
    </td>
    </tr>
    <tr id="row24429894"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.4.1.1 "><p id="p32664435"><a name="p32664435"></a><a name="p32664435"></a>subnet_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.132813281328133%" headers="mcps1.2.4.1.2 "><p id="p12049092172955"><a name="p12049092172955"></a><a name="p12049092172955"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.644964496449646%" headers="mcps1.2.4.1.3 "><p id="p26383427"><a name="p26383427"></a><a name="p26383427"></a>分配IP的子网标识</p>
    </td>
    </tr>
    <tr id="row1899134118131"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.4.1.1 "><p id="p6190364318131"><a name="p6190364318131"></a><a name="p6190364318131"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.132813281328133%" headers="mcps1.2.4.1.2 "><p id="p696029318131"><a name="p696029318131"></a><a name="p696029318131"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.644964496449646%" headers="mcps1.2.4.1.3 "><p id="p1071642181111"><a name="p1071642181111"></a><a name="p1071642181111"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row36124251"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.4.1.1 "><p id="p40383225"><a name="p40383225"></a><a name="p40383225"></a>device_owner</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.132813281328133%" headers="mcps1.2.4.1.2 "><p id="p36452392172955"><a name="p36452392172955"></a><a name="p36452392172955"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.644964496449646%" headers="mcps1.2.4.1.3 "><a name="ul1878734133215"></a><a name="ul1878734133215"></a><ul id="ul1878734133215"><li>功能说明：私有IP的使用者，空表示未使用</li><li>取值范围：network:dhcp，network:router_interface_distributed，compute:xxx(xxx对应具体的可用区名称，例如compute:aa-bb-cc表示是被可用区aa-bb-cc上的ECS使用)，neutron:VIP_PORT</li><li>约束：此处的取值范围只是本服务支持的类型，其他类型未做标注</li></ul>
    </td>
    </tr>
    <tr id="row64744584"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.4.1.1 "><p id="p9819961"><a name="p9819961"></a><a name="p9819961"></a>ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.132813281328133%" headers="mcps1.2.4.1.2 "><p id="p66962669172955"><a name="p66962669172955"></a><a name="p66962669172955"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.644964496449646%" headers="mcps1.2.4.1.3 "><p id="p38322691"><a name="p38322691"></a><a name="p38322691"></a>申请到的私有IP</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "privateips": [
            {
                "status": "DOWN",
                "id": "c60c2ce1-1e73-44bd-bf48-fd688448ff7b",
                "subnet_id": "531dec0f-3116-411b-a21b-e612e42349fd",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "device_owner": "",
                "ip_address": "192.168.1.10"
            },
            {
                "status": "DOWN",
                "id": "4b123c18-ae92-4dfa-92cd-d44002359aa1",
                "subnet_id": "531dec0f-3116-411b-a21b-e612e42349fd",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "device_owner": "",
                "ip_address": "192.168.1.17"
            }
        ]
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

