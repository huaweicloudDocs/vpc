# 更新VPC<a name="vpc_api01_0004"></a>

## 功能介绍<a name="section8079634"></a>

更新虚拟私有云。

## URI<a name="section5607849"></a>

PUT /v1/\{project\_id\}/vpcs/\{vpc\_id\}

参数说明请参见[表1](#table27380479)。

**表 1**  参数说明

<a name="table27380479"></a>
<table><thead align="left"><tr id="row28751554"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p47174532"><a name="p47174532"></a><a name="p47174532"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p63040734"><a name="p63040734"></a><a name="p63040734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p6025849"><a name="p6025849"></a><a name="p6025849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18331773"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p8478608"><a name="p8478608"></a><a name="p8478608"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p15678685"><a name="p15678685"></a><a name="p15678685"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row21254748"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p43913021"><a name="p43913021"></a><a name="p43913021"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p184914"><a name="p184914"></a><a name="p184914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p14978051"><a name="p14978051"></a><a name="p14978051"></a>虚拟私有云唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section50470647"></a>

-   请求参数

    **表 2**  请求参数

    <a name="table4060745715545"></a>
    <table><thead align="left"><tr id="row1619435515545"><th class="cellrowborder" valign="top" width="15.410000000000002%" id="mcps1.2.5.1.1"><p id="p3667439915545"><a name="p3667439915545"></a><a name="p3667439915545"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.980000000000002%" id="mcps1.2.5.1.2"><p id="p1783637615545"><a name="p1783637615545"></a><a name="p1783637615545"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.930000000000003%" id="mcps1.2.5.1.3"><p id="p3546035715545"><a name="p3546035715545"></a><a name="p3546035715545"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="45.68000000000001%" id="mcps1.2.5.1.4"><p id="p5371668715545"><a name="p5371668715545"></a><a name="p5371668715545"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5608438115545"><td class="cellrowborder" valign="top" width="15.410000000000002%" headers="mcps1.2.5.1.1 "><p id="p4654101615545"><a name="p4654101615545"></a><a name="p4654101615545"></a>vpc</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.980000000000002%" headers="mcps1.2.5.1.2 "><p id="p1172592715545"><a name="p1172592715545"></a><a name="p1172592715545"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.930000000000003%" headers="mcps1.2.5.1.3 "><p id="p1027601915545"><a name="p1027601915545"></a><a name="p1027601915545"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.68000000000001%" headers="mcps1.2.5.1.4 "><p id="p4213394815545"><a name="p4213394815545"></a><a name="p4213394815545"></a><a href="#table34290771">vpc对象</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  vpc对象

    <a name="table34290771"></a>
    <table><thead align="left"><tr id="row42952388"><th class="cellrowborder" valign="top" width="14.66%" id="mcps1.2.5.1.1"><p id="p56591389"><a name="p56591389"></a><a name="p56591389"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.35%" id="mcps1.2.5.1.2"><p id="p20499795"><a name="p20499795"></a><a name="p20499795"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.66%" id="mcps1.2.5.1.3"><p id="p17479484174639"><a name="p17479484174639"></a><a name="p17479484174639"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.33%" id="mcps1.2.5.1.4"><p id="p49870669"><a name="p49870669"></a><a name="p49870669"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12992371"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.5.1.1 "><p id="p45749167"><a name="p45749167"></a><a name="p45749167"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.2 "><p id="p14695014"><a name="p14695014"></a><a name="p14695014"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.66%" headers="mcps1.2.5.1.3 "><p id="p6552131174639"><a name="p6552131174639"></a><a name="p6552131174639"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.33%" headers="mcps1.2.5.1.4 "><a name="ul0576257538"></a><a name="ul0576257538"></a><ul id="ul0576257538"><li>功能说明：虚拟私有云名称</li><li>取值范围：0-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li><li>约束：如果名称不为空，则同一个租户下的VPC不允许重名。</li></ul>
    </td>
    </tr>
    <tr id="row12304154151511"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.5.1.1 "><p id="p211618568154"><a name="p211618568154"></a><a name="p211618568154"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.2 "><p id="p1211635651520"><a name="p1211635651520"></a><a name="p1211635651520"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.66%" headers="mcps1.2.5.1.3 "><p id="p18116165611152"><a name="p18116165611152"></a><a name="p18116165611152"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.33%" headers="mcps1.2.5.1.4 "><a name="ul5116195661518"></a><a name="ul5116195661518"></a><ul id="ul5116195661518"><li>功能说明：虚拟私有云描述</li><li>取值范围：0-255个字符，不能包含“&lt;”和“&gt;”。</li></ul>
    </td>
    </tr>
    <tr id="row7722248"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.5.1.1 "><p id="p21522370"><a name="p21522370"></a><a name="p21522370"></a>cidr</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.2 "><p id="p65590400"><a name="p65590400"></a><a name="p65590400"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.66%" headers="mcps1.2.5.1.3 "><p id="p60960565174639"><a name="p60960565174639"></a><a name="p60960565174639"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.33%" headers="mcps1.2.5.1.4 "><a name="ul161253336536"></a><a name="ul161253336536"></a><ul id="ul161253336536"><li>功能说明：虚拟私有云下可用子网的范围</li><li>取值范围：<a name="ul53161626155413"></a><a name="ul53161626155413"></a><ul id="ul53161626155413"><li>10.0.0.0/8~10.255.255.240/28</li><li>172.16.0.0/12 ~ 172.31.255.240/28</li><li>192.168.0.0/16 ~ 192.168.255.240/28</li></ul>
    </li><li>不指定cidr时，默认值为空</li><li>约束：必须是cidr格式，例如:192.168.0.0/16</li></ul>
    </td>
    </tr>
    <tr id="row1151401882715"><td class="cellrowborder" valign="top" width="14.66%" headers="mcps1.2.5.1.1 "><p id="p1470522022711"><a name="p1470522022711"></a><a name="p1470522022711"></a>routes</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.2.5.1.2 "><p id="p770572018273"><a name="p770572018273"></a><a name="p770572018273"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.66%" headers="mcps1.2.5.1.3 "><p id="p570519208272"><a name="p570519208272"></a><a name="p570519208272"></a>Array of <a href="#table1696324019336">route</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.33%" headers="mcps1.2.5.1.4 "><a name="ul13320192141811"></a><a name="ul13320192141811"></a><ul id="ul13320192141811"><li>功能说明：路由信息列表，详情参见<a href="#table3576833291556">表7</a>。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  route对象

    <a name="table1696324019336"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534238_row921218691556"><th class="cellrowborder" valign="top" width="15.110000000000001%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534238_p798956991556"><a name="zh-cn_topic_0201534238_p798956991556"></a><a name="zh-cn_topic_0201534238_p798956991556"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.85%" id="mcps1.2.5.1.2"><p id="p63244160226"><a name="p63244160226"></a><a name="p63244160226"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.530000000000001%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534238_p754435891556"><a name="zh-cn_topic_0201534238_p754435891556"></a><a name="zh-cn_topic_0201534238_p754435891556"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.51%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534238_p711326791556"><a name="zh-cn_topic_0201534238_p711326791556"></a><a name="zh-cn_topic_0201534238_p711326791556"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534238_row3930377391556"><td class="cellrowborder" valign="top" width="15.110000000000001%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534238_p2948903591556"><a name="zh-cn_topic_0201534238_p2948903591556"></a><a name="zh-cn_topic_0201534238_p2948903591556"></a>destination</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.85%" headers="mcps1.2.5.1.2 "><p id="p032471662214"><a name="p032471662214"></a><a name="p032471662214"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.530000000000001%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534238_p270722191556"><a name="zh-cn_topic_0201534238_p270722191556"></a><a name="zh-cn_topic_0201534238_p270722191556"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.51%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534238_ul18181132710558"></a><a name="zh-cn_topic_0201534238_ul18181132710558"></a><ul id="zh-cn_topic_0201534238_ul18181132710558"><li>功能说明：路由目的网段</li><li>约束：必须是cidr格式，且目前只支持0.0.0.0/0</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534238_row6565233911054"><td class="cellrowborder" valign="top" width="15.110000000000001%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534238_p1623922311054"><a name="zh-cn_topic_0201534238_p1623922311054"></a><a name="zh-cn_topic_0201534238_p1623922311054"></a>nexthop</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.85%" headers="mcps1.2.5.1.2 "><p id="p93241416202213"><a name="p93241416202213"></a><a name="p93241416202213"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.530000000000001%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534238_p4377761311054"><a name="zh-cn_topic_0201534238_p4377761311054"></a><a name="zh-cn_topic_0201534238_p4377761311054"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.51%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534238_ul17731193025515"></a><a name="zh-cn_topic_0201534238_ul17731193025515"></a><ul id="zh-cn_topic_0201534238_ul17731193025515"><li>功能说明：路由下一跳地址</li><li>约束：必须为IP地址格式，且必须属于本VPC下的子网范围内才能生效</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    PUT https://{Endpoint}/v1/{project_id}/vpcs/99d9d709-8478-4b46-9f3f-2206b1023fd3
    
    {
        "vpc": {
            "name": "vpc1",
            "description": "test1",
            "cidr": "192.168.0.0/16"
        }
    }
    ```


## 响应消息<a name="section51582645"></a>

-   响应参数

    **表 5**  响应参数

    <a name="table163236181565"></a>
    <table><thead align="left"><tr id="row361709001565"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p441618021565"><a name="p441618021565"></a><a name="p441618021565"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.729999999999997%" id="mcps1.2.4.1.2"><p id="p366208391565"><a name="p366208391565"></a><a name="p366208391565"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.93%" id="mcps1.2.4.1.3"><p id="p134980151565"><a name="p134980151565"></a><a name="p134980151565"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row195974151565"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p438867591565"><a name="p438867591565"></a><a name="p438867591565"></a>vpc</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.729999999999997%" headers="mcps1.2.4.1.2 "><p id="p440032491565"><a name="p440032491565"></a><a name="p440032491565"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.93%" headers="mcps1.2.4.1.3 "><p id="p3322021565"><a name="p3322021565"></a><a name="p3322021565"></a><a href="#table22527411">vpc对象</a></p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  vpc对象

    <a name="table22527411"></a>
    <table><thead align="left"><tr id="row37318421"><th class="cellrowborder" valign="top" width="17.59175917591759%" id="mcps1.2.4.1.1"><p id="p2893298"><a name="p2893298"></a><a name="p2893298"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.822182218221823%" id="mcps1.2.4.1.2"><p id="p32078086174724"><a name="p32078086174724"></a><a name="p32078086174724"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="60.58605860586058%" id="mcps1.2.4.1.3"><p id="p58230900"><a name="p58230900"></a><a name="p58230900"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row19082474"><td class="cellrowborder" valign="top" width="17.59175917591759%" headers="mcps1.2.4.1.1 "><p id="p2176568"><a name="p2176568"></a><a name="p2176568"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.822182218221823%" headers="mcps1.2.4.1.2 "><p id="p48188187174724"><a name="p48188187174724"></a><a name="p48188187174724"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60.58605860586058%" headers="mcps1.2.4.1.3 "><p id="p53389951"><a name="p53389951"></a><a name="p53389951"></a>uuid形式的一个资源标识。</p>
    </td>
    </tr>
    <tr id="row10747513"><td class="cellrowborder" valign="top" width="17.59175917591759%" headers="mcps1.2.4.1.1 "><p id="p65242240"><a name="p65242240"></a><a name="p65242240"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.822182218221823%" headers="mcps1.2.4.1.2 "><p id="p10929060174724"><a name="p10929060174724"></a><a name="p10929060174724"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60.58605860586058%" headers="mcps1.2.4.1.3 "><p id="p47359816174719"><a name="p47359816174719"></a><a name="p47359816174719"></a>虚拟私有云名称。</p>
    </td>
    </tr>
    <tr id="row15698184911617"><td class="cellrowborder" valign="top" width="17.59175917591759%" headers="mcps1.2.4.1.1 "><p id="p174335514162"><a name="p174335514162"></a><a name="p174335514162"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.822182218221823%" headers="mcps1.2.4.1.2 "><p id="p743345115166"><a name="p743345115166"></a><a name="p743345115166"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60.58605860586058%" headers="mcps1.2.4.1.3 "><a name="ul6433175110169"></a><a name="ul6433175110169"></a><ul id="ul6433175110169"><li>功能说明：虚拟私有云描述</li><li>取值范围：0-255个字符，不能包含“&lt;”和“&gt;”。</li></ul>
    </td>
    </tr>
    <tr id="row37632913"><td class="cellrowborder" valign="top" width="17.59175917591759%" headers="mcps1.2.4.1.1 "><p id="p28367147"><a name="p28367147"></a><a name="p28367147"></a>cidr</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.822182218221823%" headers="mcps1.2.4.1.2 "><p id="p12838666174724"><a name="p12838666174724"></a><a name="p12838666174724"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60.58605860586058%" headers="mcps1.2.4.1.3 "><a name="ul10389173917465"></a><a name="ul10389173917465"></a><ul id="ul10389173917465"><li>功能说明：虚拟私有云下可用子网的范围</li><li>取值范围：<a name="ul9987194121820"></a><a name="ul9987194121820"></a><ul id="ul9987194121820"><li>10.0.0.0/8~10.255.255.240/28</li><li>172.16.0.0/12 ~ 172.31.255.240/28</li><li>192.168.0.0/16 ~ 192.168.255.240/28</li></ul>
    </li><li>不指定cidr时，默认值为空</li><li>约束：必须是cidr格式，例如:192.168.0.0/16</li></ul>
    </td>
    </tr>
    <tr id="row14466778"><td class="cellrowborder" valign="top" width="17.59175917591759%" headers="mcps1.2.4.1.1 "><p id="p30958352"><a name="p30958352"></a><a name="p30958352"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.822182218221823%" headers="mcps1.2.4.1.2 "><p id="p33298996174724"><a name="p33298996174724"></a><a name="p33298996174724"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60.58605860586058%" headers="mcps1.2.4.1.3 "><a name="ul74552213513"></a><a name="ul74552213513"></a><ul id="ul74552213513"><li>功能说明：虚拟私有云的状态。</li><li>取值范围：<a name="ul5890854165417"></a><a name="ul5890854165417"></a><ul id="ul5890854165417"><li>CREATING：创建中</li><li>OK：创建成功</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row824411301996"><td class="cellrowborder" valign="top" width="17.59175917591759%" headers="mcps1.2.4.1.1 "><p id="p11990421917"><a name="p11990421917"></a><a name="p11990421917"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.822182218221823%" headers="mcps1.2.4.1.2 "><p id="p119917421894"><a name="p119917421894"></a><a name="p119917421894"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="60.58605860586058%" headers="mcps1.2.4.1.3 "><a name="ul04621553135413"></a><a name="ul04621553135413"></a><ul id="ul04621553135413"><li>功能说明：企业项目ID。</li><li>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。</li></ul>
    </td>
    </tr>
    <tr id="row6192167813568"><td class="cellrowborder" valign="top" width="17.59175917591759%" headers="mcps1.2.4.1.1 "><p id="p4960003413568"><a name="p4960003413568"></a><a name="p4960003413568"></a>routes</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.822182218221823%" headers="mcps1.2.4.1.2 "><p id="p1494185813568"><a name="p1494185813568"></a><a name="p1494185813568"></a>Array&nbsp;of&nbsp;<a href="#table3576833291556">route</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="60.58605860586058%" headers="mcps1.2.4.1.3 "><a name="ul1021319485513"></a><a name="ul1021319485513"></a><ul id="ul1021319485513"><li>功能说明：路由信息列表</li><li>约束：详情参见<a href="#table3576833291556">route对象</a></li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 7**  route对象

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
    <td class="cellrowborder" valign="top" width="59.28%" headers="mcps1.2.4.1.3 "><a name="ul18181132710558"></a><a name="ul18181132710558"></a><ul id="ul18181132710558"><li>功能说明：路由目的网段</li><li>约束：必须是cidr格式，且目前只支持0.0.0.0/0</li></ul>
    </td>
    </tr>
    <tr id="row6565233911054"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p1623922311054"><a name="p1623922311054"></a><a name="p1623922311054"></a>nexthop</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.2.4.1.2 "><p id="p4377761311054"><a name="p4377761311054"></a><a name="p4377761311054"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="59.28%" headers="mcps1.2.4.1.3 "><a name="ul17731193025515"></a><a name="ul17731193025515"></a><ul id="ul17731193025515"><li>功能说明：路由下一跳地址</li><li>约束：必须为IP地址格式，且必须属于本VPC下的子网范围内才能生效</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "vpc": {
            "id": "99d9d709-8478-4b46-9f3f-2206b1023fd3",
            "name": "vpc1",
            "description": "test1",
            "cidr": "192.168.0.0/16",
            "status": "OK",
            "enterprise_project_id": "0",
            "routes": []
        }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

