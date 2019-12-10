# 查询私有IP<a name="ZH-CN_TOPIC_0201534217"></a>

## 功能介绍<a name="section9185002"></a>

指定IP的ID查询私有IP。

## URI<a name="section15556157"></a>

GET /v1/\{project\_id\}/privateips/\{privateip\_id\}

参数说明请参见[表1](#table4378562)。

**表 1**  参数说明

<a name="table4378562"></a>
<table><thead align="left"><tr id="row14851049"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p62084314"><a name="p62084314"></a><a name="p62084314"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p62773503"><a name="p62773503"></a><a name="p62773503"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p51488960"><a name="p51488960"></a><a name="p51488960"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row9856263"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p60159801"><a name="p60159801"></a><a name="p60159801"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p41105728"><a name="p41105728"></a><a name="p41105728"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row35522984"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p58789457"><a name="p58789457"></a><a name="p58789457"></a>privateip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p64325611"><a name="p64325611"></a><a name="p64325611"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p42992030"><a name="p42992030"></a><a name="p42992030"></a>私有IP唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section5787686"></a>

-   请求参数

    无

-   请求样例

    ```
    GET https://{Endpoint}/v1/{project_id}/privateips/d600542a-b231-45ed-af05-e9930cb14f78
    ```


## 响应<a name="section52089174"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table66473901155923"></a>
    <table><thead align="left"><tr id="row7115943155923"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p39520483155923"><a name="p39520483155923"></a><a name="p39520483155923"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="p52352674155923"><a name="p52352674155923"></a><a name="p52352674155923"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="p12708212155923"><a name="p12708212155923"></a><a name="p12708212155923"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row22732275155923"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p29374982155923"><a name="p29374982155923"></a><a name="p29374982155923"></a>privateip</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p59712266155923"><a name="p59712266155923"></a><a name="p59712266155923"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p43698339155923"><a name="p43698339155923"></a><a name="p43698339155923"></a>私有IP对象，请参见<a href="#table23250319">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  privateip字段说明

    <a name="table23250319"></a>
    <table><thead align="left"><tr id="row21723514"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="p14774201"><a name="p14774201"></a><a name="p14774201"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.2"><p id="p21721490173058"><a name="p21721490173058"></a><a name="p21721490173058"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="54%" id="mcps1.2.4.1.3"><p id="p28338386"><a name="p28338386"></a><a name="p28338386"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row13707899"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p36597996"><a name="p36597996"></a><a name="p36597996"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="p14610233173058"><a name="p14610233173058"></a><a name="p14610233173058"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><a name="ul13978236183119"></a><a name="ul13978236183119"></a><ul id="ul13978236183119"><li>功能说明：私有IP的状态</li><li>取值范围：<a name="ul948092312377"></a><a name="ul948092312377"></a><ul id="ul948092312377"><li>ACTIVE：活动的</li><li>DOWN：不可用</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row53064224"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p3234911"><a name="p3234911"></a><a name="p3234911"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="p42578245173058"><a name="p42578245173058"></a><a name="p42578245173058"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><p id="p47453675"><a name="p47453675"></a><a name="p47453675"></a>私有IP标识</p>
    </td>
    </tr>
    <tr id="row36801206"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p28107703"><a name="p28107703"></a><a name="p28107703"></a>subnet_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="p26285854173058"><a name="p26285854173058"></a><a name="p26285854173058"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><p id="p26383427"><a name="p26383427"></a><a name="p26383427"></a>分配IP的子网标识</p>
    </td>
    </tr>
    <tr id="row54031349181512"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p4774073181513"><a name="p4774073181513"></a><a name="p4774073181513"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="p49967057181513"><a name="p49967057181513"></a><a name="p49967057181513"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><p id="p167315119118"><a name="p167315119118"></a><a name="p167315119118"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row25113108"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p20895830"><a name="p20895830"></a><a name="p20895830"></a>device_owner</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="p48779435173058"><a name="p48779435173058"></a><a name="p48779435173058"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><a name="ul1878734133215"></a><a name="ul1878734133215"></a><ul id="ul1878734133215"><li>功能说明：私有IP的使用者，空表示未使用</li><li>取值范围：network:dhcp，network:router_interface_distributed，compute:xxx(xxx对应具体的可用区名称，例如compute:aa-bb-cc表示是被可用区aa-bb-cc上的ECS使用)，neutron:VIP_PORT</li><li>约束：此处的取值范围只是本服务支持的类型，其他类型未做标注</li></ul>
    </td>
    </tr>
    <tr id="row46793790"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p32200631"><a name="p32200631"></a><a name="p32200631"></a>ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="p58820181173058"><a name="p58820181173058"></a><a name="p58820181173058"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.4.1.3 "><p id="p19644001"><a name="p19644001"></a><a name="p19644001"></a>申请到的私有IP</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "privateip": 
            {
                "status": "DOWN",
                "id": "d600542a-b231-45ed-af05-e9930cb14f78",
                "subnet_id": "531dec0f-3116-411b-a21b-e612e42349fd",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "device_owner": "",
                "ip_address": "192.168.1.11"
            }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

