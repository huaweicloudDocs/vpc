# 查询私有IP列表<a name="vpc_privateip_0003"></a>

## 功能介绍<a name="section54434571"></a>

查询指定子网下的私有IP列表。

>![](public_sys-resources/icon-note.gif) **说明：** 
>此API无法获取系统保留地址，如DHCP IP，Gateway IP。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=ListPrivateips)中直接运行调试该接口。

## URI<a name="section20149094"></a>

GET /v1/\{project\_id\}/subnets/\{subnet\_id\}/privateips

样例：

```
GET https://{Endpoint}/v1/{project_id}/subnets/{subnet_id}/privateips?limit=10&marker=4779ab1c-7c1a-44b1-a02e-93dfc361b32d
```

参数说明请参见[表1](#table12098568)。

**表 1**  参数说明

<a name="table12098568"></a>
<table><thead align="left"><tr id="row42283611"><th class="cellrowborder" valign="top" width="16.73%" id="mcps1.2.5.1.1"><p id="p2420499"><a name="p2420499"></a><a name="p2420499"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.54%" id="mcps1.2.5.1.2"><p id="p61842715"><a name="p61842715"></a><a name="p61842715"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.61%" id="mcps1.2.5.1.3"><p id="p18030025173211"><a name="p18030025173211"></a><a name="p18030025173211"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.120000000000005%" id="mcps1.2.5.1.4"><p id="p43203995"><a name="p43203995"></a><a name="p43203995"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row9862716"><td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.1 "><p id="p60682533"><a name="p60682533"></a><a name="p60682533"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.54%" headers="mcps1.2.5.1.2 "><p id="p16338175"><a name="p16338175"></a><a name="p16338175"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.61%" headers="mcps1.2.5.1.3 "><p id="p51145882173211"><a name="p51145882173211"></a><a name="p51145882173211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row32261252"><td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.1 "><p id="p63024590"><a name="p63024590"></a><a name="p63024590"></a>subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.54%" headers="mcps1.2.5.1.2 "><p id="p4718148"><a name="p4718148"></a><a name="p4718148"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.61%" headers="mcps1.2.5.1.3 "><p id="p49175772173211"><a name="p49175772173211"></a><a name="p49175772173211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p44471500173244"><a name="p44471500173244"></a><a name="p44471500173244"></a>私有IP所在子网的唯一标识</p>
<p id="p3938441164618"><a name="p3938441164618"></a><a name="p3938441164618"></a>如果您使用管理控制台，此值即为子网详情中的“网络ID”参数值。</p>
</td>
</tr>
<tr id="row33082261"><td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.1 "><p id="p62417507"><a name="p62417507"></a><a name="p62417507"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="16.54%" headers="mcps1.2.5.1.2 "><p id="p22653281"><a name="p22653281"></a><a name="p22653281"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.61%" headers="mcps1.2.5.1.3 "><p id="p23814582173211"><a name="p23814582173211"></a><a name="p23814582173211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p28526205175853"><a name="p28526205175853"></a><a name="p28526205175853"></a>分页查询的起始资源ID，表示从指定资源的下一条记录开始查询。</p>
<p id="p538818488578"><a name="p538818488578"></a><a name="p538818488578"></a>marker需要和limit配合使用：</p>
<a name="ul12704811125810"></a><a name="ul12704811125810"></a><ul id="ul12704811125810"><li>若不传入marker和limit参数，查询结果返回全部资源记录。</li><li>若不传入marker参数，limit为10，查询结果返回第1~10条资源记录。</li><li>若marker为第10条记录的资源ID，limit为10，查询结果返回第11~20条资源记录。</li><li>若marker为第10条记录的资源ID，不传入limit参数，查询结果返回第11条及之后的所有资源记录。</li></ul>
</td>
</tr>
<tr id="row39717249"><td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.1 "><p id="p62980604"><a name="p62980604"></a><a name="p62980604"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="16.54%" headers="mcps1.2.5.1.2 "><p id="p1155275"><a name="p1155275"></a><a name="p1155275"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.61%" headers="mcps1.2.5.1.3 "><p id="p49933009173211"><a name="p49933009173211"></a><a name="p49933009173211"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="48.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p2017153116589"><a name="p2017153116589"></a><a name="p2017153116589"></a>分页查询每页返回的记录个数，取值范围为0~intmax。</p>
<p id="p125192338584"><a name="p125192338584"></a><a name="p125192338584"></a>limit需要和marker配合使用，详细规则请见marker的参数说明。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section47124125"></a>

-   请求参数

    无

-   请求样例

    ```
    GET https://{Endpoint}/v1/{project_id}/subnets/{subnet_id}/privateips
    ```


## 响应消息<a name="section21463943"></a>

-   请求参数

    **表 2**  请求参数

    <a name="table16726122155915"></a>
    <table><thead align="left"><tr id="row50660459155915"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p9856497155915"><a name="p9856497155915"></a><a name="p9856497155915"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="p42646948155915"><a name="p42646948155915"></a><a name="p42646948155915"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="p31850784155915"><a name="p31850784155915"></a><a name="p31850784155915"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row29776745155915"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p63106150155915"><a name="p63106150155915"></a><a name="p63106150155915"></a>privateips</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p44872862155915"><a name="p44872862155915"></a><a name="p44872862155915"></a>Array of <a href="#table21538022">privateip</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p30300018155915"><a name="p30300018155915"></a><a name="p30300018155915"></a>私有IP列表对象，请参见<a href="#table21538022">表3</a>。</p>
    <p id="p15992181219214"><a name="p15992181219214"></a><a name="p15992181219214"></a>说明：不支持显示预留的系统接口，如有需要请登录管理控制台查看。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  privateip字段说明

    <a name="table21538022"></a>
    <table><thead align="left"><tr id="row33313579"><th class="cellrowborder" valign="top" width="22.17778222177782%" id="mcps1.2.4.1.1"><p id="p14045344"><a name="p14045344"></a><a name="p14045344"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.477852214778522%" id="mcps1.2.4.1.2"><p id="p42744433173254"><a name="p42744433173254"></a><a name="p42744433173254"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.34436556344365%" id="mcps1.2.4.1.3"><p id="p11033160"><a name="p11033160"></a><a name="p11033160"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row21270730"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p45207585"><a name="p45207585"></a><a name="p45207585"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p39747058173254"><a name="p39747058173254"></a><a name="p39747058173254"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><a name="ul13978236183119"></a><a name="ul13978236183119"></a><ul id="ul13978236183119"><li>功能说明：私有IP的状态</li><li>取值范围：<a name="ul948092312377"></a><a name="ul948092312377"></a><ul id="ul948092312377"><li>ACTIVE：活动的</li><li>DOWN：不可用</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row44135236"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p18184391"><a name="p18184391"></a><a name="p18184391"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p65395131173254"><a name="p65395131173254"></a><a name="p65395131173254"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><p id="p47453675"><a name="p47453675"></a><a name="p47453675"></a>私有IP标识</p>
    </td>
    </tr>
    <tr id="row53320433"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p23987813"><a name="p23987813"></a><a name="p23987813"></a>subnet_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p62514293173254"><a name="p62514293173254"></a><a name="p62514293173254"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><p id="p26383427"><a name="p26383427"></a><a name="p26383427"></a>分配IP的子网标识</p>
    <p id="p21021525477"><a name="p21021525477"></a><a name="p21021525477"></a>如果您使用管理控制台，此值即为子网详情中的“网络ID”参数值。</p>
    </td>
    </tr>
    <tr id="row8629350181540"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p22152840181542"><a name="p22152840181542"></a><a name="p22152840181542"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p54098843181542"><a name="p54098843181542"></a><a name="p54098843181542"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><p id="p126338192113"><a name="p126338192113"></a><a name="p126338192113"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row40871974"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p22295564"><a name="p22295564"></a><a name="p22295564"></a>device_owner</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p30493000173254"><a name="p30493000173254"></a><a name="p30493000173254"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><a name="ul1878734133215"></a><a name="ul1878734133215"></a><ul id="ul1878734133215"><li>功能说明：私有IP的使用者，空表示未使用</li><li>取值范围：network:dhcp，network:router_interface_distributed，compute:xxx(xxx对应具体的可用区名称，例如compute:aa-bb-cc表示是被可用区aa-bb-cc上的ECS使用)，neutron:VIP_PORT</li><li>约束：此处的取值范围只是本服务支持的类型，其他类型未做标注</li></ul>
    </td>
    </tr>
    <tr id="row35044283"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p20014644"><a name="p20014644"></a><a name="p20014644"></a>ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p54013915173254"><a name="p54013915173254"></a><a name="p54013915173254"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><p id="p57619553"><a name="p57619553"></a><a name="p57619553"></a>申请到的私有IP</p>
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
                "id": "d600542a-b231-45ed-af05-e9930cb14f78",
                "subnet_id": "531dec0f-3116-411b-a21b-e612e42349fd",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "device_owner": "",
                "ip_address": "192.168.1.11"
            },
            {
                "status": "DOWN",
                "id": "d600542a-b231-45ed-af05-e9930cb14f79",
                "subnet_id": "531dec0f-3116-411b-a21b-e612e42349fd",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "device_owner": "",
                "ip_address": "192.168.1.12"
            }
        ]
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

