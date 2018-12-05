# 查询私有IP列表<a name="ZH-CN_TOPIC_0020090612"></a>

## 功能介绍<a name="section54434571"></a>

查询指定子网下的私有IP列表。

## URI<a name="section20149094"></a>

GET /v1/\{project\_id\}/subnets/\{subnet\_id\}/privateips

样例：

```
/v1/{project_id}/subnets/{subnet_id}/privateips?limit=10&marker=4779ab1c-7c1a-44b1-a02e-93dfc361b32d
```

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
<td class="cellrowborder" valign="top" width="48.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p48323826"><a name="p48323826"></a><a name="p48323826"></a>项目ID</p>
</td>
</tr>
<tr id="row32261252"><td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.1 "><p id="p63024590"><a name="p63024590"></a><a name="p63024590"></a>subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.54%" headers="mcps1.2.5.1.2 "><p id="p4718148"><a name="p4718148"></a><a name="p4718148"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.61%" headers="mcps1.2.5.1.3 "><p id="p49175772173211"><a name="p49175772173211"></a><a name="p49175772173211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p44471500173244"><a name="p44471500173244"></a><a name="p44471500173244"></a>私有IP所在子网的唯一标识</p>
</td>
</tr>
<tr id="row33082261"><td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.1 "><p id="p62417507"><a name="p62417507"></a><a name="p62417507"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="16.54%" headers="mcps1.2.5.1.2 "><p id="p22653281"><a name="p22653281"></a><a name="p22653281"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.61%" headers="mcps1.2.5.1.3 "><p id="p23814582173211"><a name="p23814582173211"></a><a name="p23814582173211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.120000000000005%" headers="mcps1.2.5.1.4 "><p id="p49152270"><a name="p49152270"></a><a name="p49152270"></a>分页查询起始的资源id，为空时为查询第一页</p>
</td>
</tr>
<tr id="row39717249"><td class="cellrowborder" valign="top" width="16.73%" headers="mcps1.2.5.1.1 "><p id="p62980604"><a name="p62980604"></a><a name="p62980604"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="16.54%" headers="mcps1.2.5.1.2 "><p id="p1155275"><a name="p1155275"></a><a name="p1155275"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.61%" headers="mcps1.2.5.1.3 "><p id="p49933009173211"><a name="p49933009173211"></a><a name="p49933009173211"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="48.120000000000005%" headers="mcps1.2.5.1.4 "><a name="ul18965173516362"></a><a name="ul18965173516362"></a><ul id="ul18965173516362"><li>功能说明：每页返回的个数</li><li>取值范围：0~intmax</li></ul>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section47124125"></a>

-   请求参数

    无

-   请求样例

    无


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
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p44872862155915"><a name="p44872862155915"></a><a name="p44872862155915"></a><em id="i1202578155915"><a name="i1202578155915"></a><a name="i1202578155915"></a>列表数据结构</em></p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p30300018155915"><a name="p30300018155915"></a><a name="p30300018155915"></a>私有IP列表对象</p>
    <p id="p15992181219214"><a name="p15992181219214"></a><a name="p15992181219214"></a>说明：不支持显示预留的系统接口，如有需要请登录管理控制台查看。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  privateips字段说明

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
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><a name="ul26091654163716"></a><a name="ul26091654163716"></a><ul id="ul26091654163716"><li>功能说明：私有IP的状态</li><li>取值范围：ACTIVE ,DOWN</li></ul>
    </td>
    </tr>
    <tr id="row44135236"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p18184391"><a name="p18184391"></a><a name="p18184391"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p65395131173254"><a name="p65395131173254"></a><a name="p65395131173254"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><p id="p28294113"><a name="p28294113"></a><a name="p28294113"></a>私有IP标识</p>
    </td>
    </tr>
    <tr id="row53320433"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p23987813"><a name="p23987813"></a><a name="p23987813"></a>subnet_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p62514293173254"><a name="p62514293173254"></a><a name="p62514293173254"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><p id="p56737113"><a name="p56737113"></a><a name="p56737113"></a>分配IP的子网标识</p>
    </td>
    </tr>
    <tr id="row8629350181540"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p22152840181542"><a name="p22152840181542"></a><a name="p22152840181542"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p54098843181542"><a name="p54098843181542"></a><a name="p54098843181542"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><p id="p19930183181542"><a name="p19930183181542"></a><a name="p19930183181542"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row40871974"><td class="cellrowborder" valign="top" width="22.17778222177782%" headers="mcps1.2.4.1.1 "><p id="p22295564"><a name="p22295564"></a><a name="p22295564"></a>device_owner</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.477852214778522%" headers="mcps1.2.4.1.2 "><p id="p30493000173254"><a name="p30493000173254"></a><a name="p30493000173254"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.34436556344365%" headers="mcps1.2.4.1.3 "><a name="ul82162733817"></a><a name="ul82162733817"></a><ul id="ul82162733817"><li>功能说明：私有IP的使用者，空表示未使用</li><li>取值范围：network:dhcp，network:router_interface_distributed，compute:xxx(xxx对应具体的az名称，例如compute:aa-bb-cc表示是被aa-bb-cc上的虚拟机使用)，neutron:VIP_PORT</li><li>约束：此处的取值范围只是本服务支持的类型，其他类型未做标注</li></ul>
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

