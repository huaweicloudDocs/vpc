# 查询VPC列表<a name="zh-cn_topic_0020090625"></a>

## 功能介绍<a name="section14477792"></a>

查询虚拟私有云列表。

## URI<a name="section63191266"></a>

GET /v1/\{project\_id\}/vpcs

样例：

```
GET https://{Endpoint}/v1/{project_id}/vpcs?limit=10&marker=13551d6b-755d-4757-b956-536f674975c0
```

参数说明请参见[表1](#table39337169)。

**表 1**  参数说明

<a name="table39337169"></a>
<table><thead align="left"><tr id="row33970761"><th class="cellrowborder" valign="top" width="15.6%" id="mcps1.2.5.1.1"><p id="p168245"><a name="p168245"></a><a name="p168245"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="p13627845"><a name="p13627845"></a><a name="p13627845"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.48%" id="mcps1.2.5.1.3"><p id="p17267522174356"><a name="p17267522174356"></a><a name="p17267522174356"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.94%" id="mcps1.2.5.1.4"><p id="p30113633"><a name="p30113633"></a><a name="p30113633"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row23285234"><td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.5.1.1 "><p id="p7055840"><a name="p7055840"></a><a name="p7055840"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p34652178"><a name="p34652178"></a><a name="p34652178"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.5.1.3 "><p id="p56492018174356"><a name="p56492018174356"></a><a name="p56492018174356"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.94%" headers="mcps1.2.5.1.4 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row28505468"><td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.5.1.1 "><p id="p27241609"><a name="p27241609"></a><a name="p27241609"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p59086710"><a name="p59086710"></a><a name="p59086710"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.5.1.3 "><p id="p12450755174356"><a name="p12450755174356"></a><a name="p12450755174356"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.94%" headers="mcps1.2.5.1.4 "><p id="p24297067174412"><a name="p24297067174412"></a><a name="p24297067174412"></a>分页查询起始的资源ID，为空时为查询第一页</p>
</td>
</tr>
<tr id="row21315230"><td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.5.1.1 "><p id="p48812047"><a name="p48812047"></a><a name="p48812047"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p61461766"><a name="p61461766"></a><a name="p61461766"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.5.1.3 "><p id="p1878236174356"><a name="p1878236174356"></a><a name="p1878236174356"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50.94%" headers="mcps1.2.5.1.4 "><a name="ul15798159502"></a><a name="ul15798159502"></a><ul id="ul15798159502"><li>功能说明：每页返回的个数</li><li>取值范围：0~intmax</li></ul>
</td>
</tr>
<tr id="row1068512542210"><td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.5.1.1 "><p id="p55289571029"><a name="p55289571029"></a><a name="p55289571029"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p15529457128"><a name="p15529457128"></a><a name="p15529457128"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.5.1.3 "><p id="p165291857925"><a name="p165291857925"></a><a name="p165291857925"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.94%" headers="mcps1.2.5.1.4 "><a name="ul152391731105011"></a><a name="ul152391731105011"></a><ul id="ul152391731105011"><li>功能说明：企业项目ID。可以使用该字段过滤某个企业项目下的虚拟私有云。</li><li>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。若需要查询当前用户所有企业项目绑定的虚拟私有云，请传参<strong id="b1618205893315"><a name="b1618205893315"></a><a name="b1618205893315"></a>all_granted_eps</strong>。</li></ul>
<div class="note" id="note104812057325"><a name="note104812057325"></a><a name="note104812057325"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1915862704914"><a name="p1915862704914"></a><a name="p1915862704914"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0126101490.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section31850483"></a>

-   请求参数

    无

-   请求样例

    ```
    GET https://{Endpoint}/v1/{project_id}/vpcs
    ```


## 响应消息<a name="section18218892"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table6229176715519"></a>
    <table><thead align="left"><tr id="row6055323715519"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p586512615519"><a name="p586512615519"></a><a name="p586512615519"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.97%" id="mcps1.2.4.1.2"><p id="p2771539415519"><a name="p2771539415519"></a><a name="p2771539415519"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.690000000000005%" id="mcps1.2.4.1.3"><p id="p3035446115519"><a name="p3035446115519"></a><a name="p3035446115519"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row4279228915519"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p4362334815519"><a name="p4362334815519"></a><a name="p4362334815519"></a>vpcs</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.97%" headers="mcps1.2.4.1.2 "><p id="p26395826172022"><a name="p26395826172022"></a><a name="p26395826172022"></a>Array of <a href="#table65129753">vpcs</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.690000000000005%" headers="mcps1.2.4.1.3 "><p id="p1714182515519"><a name="p1714182515519"></a><a name="p1714182515519"></a>vpc对象</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  vpcs字段说明

    <a name="table65129753"></a>
    <table><thead align="left"><tr id="row16647026"><th class="cellrowborder" valign="top" width="15.870000000000001%" id="mcps1.2.4.1.1"><p id="p6231886"><a name="p6231886"></a><a name="p6231886"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.91%" id="mcps1.2.4.1.2"><p id="p25347041174441"><a name="p25347041174441"></a><a name="p25347041174441"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="62.22%" id="mcps1.2.4.1.3"><p id="p18111828"><a name="p18111828"></a><a name="p18111828"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row57771982"><td class="cellrowborder" valign="top" width="15.870000000000001%" headers="mcps1.2.4.1.1 "><p id="p49018956"><a name="p49018956"></a><a name="p49018956"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.91%" headers="mcps1.2.4.1.2 "><p id="p39844479174441"><a name="p39844479174441"></a><a name="p39844479174441"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><p id="p27697526"><a name="p27697526"></a><a name="p27697526"></a>uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row47951145"><td class="cellrowborder" valign="top" width="15.870000000000001%" headers="mcps1.2.4.1.1 "><p id="p58837506"><a name="p58837506"></a><a name="p58837506"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.91%" headers="mcps1.2.4.1.2 "><p id="p6177377174441"><a name="p6177377174441"></a><a name="p6177377174441"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><a name="ul951112614463"></a><a name="ul951112614463"></a><ul id="ul951112614463"><li>功能说明：虚拟私有云名称</li><li>取值范围：0-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li><li>约束：如果名称不为空，则同一个租户下的名称不能重复</li></ul>
    </td>
    </tr>
    <tr id="row18577115091311"><td class="cellrowborder" valign="top" width="15.870000000000001%" headers="mcps1.2.4.1.1 "><p id="p174994533139"><a name="p174994533139"></a><a name="p174994533139"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.91%" headers="mcps1.2.4.1.2 "><p id="p349935312131"><a name="p349935312131"></a><a name="p349935312131"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><a name="ul16499115318137"></a><a name="ul16499115318137"></a><ul id="ul16499115318137"><li>功能说明：虚拟私有云描述</li><li>取值范围：0-255个字符，不能包含“&lt;”和“&gt;”。</li></ul>
    </td>
    </tr>
    <tr id="row2894687"><td class="cellrowborder" valign="top" width="15.870000000000001%" headers="mcps1.2.4.1.1 "><p id="p33143133"><a name="p33143133"></a><a name="p33143133"></a>cidr</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.91%" headers="mcps1.2.4.1.2 "><p id="p30605552174441"><a name="p30605552174441"></a><a name="p30605552174441"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><a name="ul10389173917465"></a><a name="ul10389173917465"></a><ul id="ul10389173917465"><li>功能说明：虚拟私有云下可用子网的范围</li><li>取值范围：<a name="ul53161626155413"></a><a name="ul53161626155413"></a><ul id="ul53161626155413"><li>10.0.0.0/8~10.255.255.240/28</li><li>172.16.0.0/12 ~ 172.31.255.240/28</li><li>192.168.0.0/16 ~ 192.168.255.240/28</li></ul>
    </li><li>不指定cidr时，默认值为空</li><li>约束：必须是cidr格式，例如:192.168.0.0/16</li></ul>
    </td>
    </tr>
    <tr id="row40205569"><td class="cellrowborder" valign="top" width="15.870000000000001%" headers="mcps1.2.4.1.1 "><p id="p35425694"><a name="p35425694"></a><a name="p35425694"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.91%" headers="mcps1.2.4.1.2 "><p id="p63130643174441"><a name="p63130643174441"></a><a name="p63130643174441"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><a name="ul74552213513"></a><a name="ul74552213513"></a><ul id="ul74552213513"><li>功能说明：虚拟私有云的状态。</li><li>取值范围：<a name="ul5890854165417"></a><a name="ul5890854165417"></a><ul id="ul5890854165417"><li>CREATING：创建中</li><li>OK：创建成功</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row1340951516517"><td class="cellrowborder" valign="top" width="15.870000000000001%" headers="mcps1.2.4.1.1 "><p id="p28181711511"><a name="p28181711511"></a><a name="p28181711511"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.91%" headers="mcps1.2.4.1.2 "><p id="p488171056"><a name="p488171056"></a><a name="p488171056"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><a name="ul10874181418512"></a><a name="ul10874181418512"></a><ul id="ul10874181418512"><li>功能说明：企业项目ID。</li><li>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。若需要查询当前用户所有企业项目绑定的虚拟私有云，请传参<strong id="b188073518203"><a name="b188073518203"></a><a name="b188073518203"></a>all_granted_eps</strong>。</li></ul>
    </td>
    </tr>
    <tr id="row56256918135346"><td class="cellrowborder" valign="top" width="15.870000000000001%" headers="mcps1.2.4.1.1 "><p id="p60516514135346"><a name="p60516514135346"></a><a name="p60516514135346"></a>routes</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.91%" headers="mcps1.2.4.1.2 "><p id="p32811915135346"><a name="p32811915135346"></a><a name="p32811915135346"></a>Array&nbsp;of&nbsp;<a href="#table3576833291556">route</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="62.22%" headers="mcps1.2.4.1.3 "><a name="ul93249349513"></a><a name="ul93249349513"></a><ul id="ul93249349513"><li>功能说明：路由信息列表</li><li>约束：详情参见<a href="#table3576833291556">表4</a>。</li></ul>
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
    <td class="cellrowborder" valign="top" width="59.28%" headers="mcps1.2.4.1.3 "><a name="ul5555115211517"></a><a name="ul5555115211517"></a><ul id="ul5555115211517"><li>功能说明：路由目的网段</li><li>约束：必须是cidr格式，且目前只支持0.0.0.0/0</li></ul>
    </td>
    </tr>
    <tr id="row6565233911054"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p1623922311054"><a name="p1623922311054"></a><a name="p1623922311054"></a>nexthop</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.2 "><p id="p4377761311054"><a name="p4377761311054"></a><a name="p4377761311054"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59.28%" headers="mcps1.2.4.1.3 "><a name="ul69731859205110"></a><a name="ul69731859205110"></a><ul id="ul69731859205110"><li>功能说明：路由下一跳地址</li><li>约束：必须为IP地址格式，且必须属于本VPC下的子网范围内才能生效</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "vpcs": [
            {
                "id": "13551d6b-755d-4757-b956-536f674975c0",
                "name": "default",
                "description": "test",
                "cidr": "172.16.0.0/16",
                "status": "OK",
                "enterprise_project_id": "0",
                "routes": []
            },
            {
                "id": "3ec3b33f-ac1c-4630-ad1c-7dba1ed79d85",
                "name": "222",
                "description": "test",
                "cidr": "192.168.0.0/16",
                "status": "OK",
                "enterprise_project_id": "0635d733-c12d-4308-ba5a-4dc27ec21038",
                "routes": []
            },
            {
                "id": "99d9d709-8478-4b46-9f3f-2206b1023fd3",
                "name": "vpc",
                "description": "test",
                "cidr": "192.168.0.0/16",
                "status": "OK",
                "enterprise_project_id": "0",
                "routes": []
            }
        ]
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

