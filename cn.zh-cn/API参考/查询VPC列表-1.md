# 查询VPC列表<a name="vpc_apiv3_0003"></a>

## 功能介绍<a name="section1919517351246"></a>

查询vpc列表

## 接口约束<a name="section21961035345"></a>

查询提交请求的租户有权限查看的所有vpc信息，单次查询最多返回2000条数据，超过2000后会返回分页标记

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v3&api=ListVpcs)中直接运行调试该接口。

## URI<a name="section11961635147"></a>

GET /v3/\{project\_id\}/vpc/vpcs

**表 1**  参数说明

<a name="table13981202416619"></a>
<table><thead align="left"><tr id="vpc_apiv3_0010_row12360162617494"><th class="cellrowborder" valign="top" width="19.68%" id="mcps1.2.5.1.1"><p id="vpc_apiv3_0010_p23609262498"><a name="vpc_apiv3_0010_p23609262498"></a><a name="vpc_apiv3_0010_p23609262498"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="10.23%" id="mcps1.2.5.1.2"><p id="vpc_apiv3_0010_p636022610493"><a name="vpc_apiv3_0010_p636022610493"></a><a name="vpc_apiv3_0010_p636022610493"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.47%" id="mcps1.2.5.1.3"><p id="vpc_apiv3_0010_p420133518412"><a name="vpc_apiv3_0010_p420133518412"></a><a name="vpc_apiv3_0010_p420133518412"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="52.62%" id="mcps1.2.5.1.4"><p id="vpc_apiv3_0010_p193601726164911"><a name="vpc_apiv3_0010_p193601726164911"></a><a name="vpc_apiv3_0010_p193601726164911"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_apiv3_0010_row1536072616490"><td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.2.5.1.1 "><p id="vpc_apiv3_0010_p5360162664920"><a name="vpc_apiv3_0010_p5360162664920"></a><a name="vpc_apiv3_0010_p5360162664920"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.23%" headers="mcps1.2.5.1.2 "><p id="vpc_apiv3_0010_p18360192644917"><a name="vpc_apiv3_0010_p18360192644917"></a><a name="vpc_apiv3_0010_p18360192644917"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.47%" headers="mcps1.2.5.1.3 "><p id="vpc_apiv3_0010_p12056351843"><a name="vpc_apiv3_0010_p12056351843"></a><a name="vpc_apiv3_0010_p12056351843"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.62%" headers="mcps1.2.5.1.4 "><p id="vpc_apiv3_0010_p9930182615482"><a name="vpc_apiv3_0010_p9930182615482"></a><a name="vpc_apiv3_0010_p9930182615482"></a>项目ID。</p>
<p id="vpc_apiv3_0010_p10487112"><a name="vpc_apiv3_0010_p10487112"></a><a name="vpc_apiv3_0010_p10487112"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Query参数

<a name="table821012355420"></a>
<table><thead align="left"><tr id="row182092351548"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p112109355419"><a name="p112109355419"></a><a name="p112109355419"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p121183516416"><a name="p121183516416"></a><a name="p121183516416"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p921111351941"><a name="p921111351941"></a><a name="p921111351941"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p12212173516415"><a name="p12212173516415"></a><a name="p12212173516415"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1068402115251"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1621820357411"><a name="p1621820357411"></a><a name="p1621820357411"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p1921819351445"><a name="p1921819351445"></a><a name="p1921819351445"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p12205351541"><a name="p12205351541"></a><a name="p12205351541"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p44931715275"><a name="p44931715275"></a><a name="p44931715275"></a>功能说明：每页返回的个数</p>
<p id="p755541252719"><a name="p755541252719"></a><a name="p755541252719"></a>取值范围：0-2000</p>
</td>
</tr>
<tr id="row83481241172511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p22214351241"><a name="p22214351241"></a><a name="p22214351241"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p162220351548"><a name="p162220351548"></a><a name="p162220351548"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p52231935548"><a name="p52231935548"></a><a name="p52231935548"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p55741012172716"><a name="p55741012172716"></a><a name="p55741012172716"></a>分页查询起始的资源ID，为空时查询第一页</p>
</td>
</tr>
<tr id="row655535012516"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p42151351441"><a name="p42151351441"></a><a name="p42151351441"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p1121783518415"><a name="p1121783518415"></a><a name="p1121783518415"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p1521711355417"><a name="p1521711355417"></a><a name="p1521711355417"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p82181135348"><a name="p82181135348"></a><a name="p82181135348"></a>VPC资源ID。可以使用该字段过滤VPC</p>
</td>
</tr>
<tr id="row1379165762517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1622443516411"><a name="p1622443516411"></a><a name="p1622443516411"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p322412351643"><a name="p322412351643"></a><a name="p322412351643"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p5224193519418"><a name="p5224193519418"></a><a name="p5224193519418"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p18225183516415"><a name="p18225183516415"></a><a name="p18225183516415"></a>VPC的name信息，可以使用该字段过滤VPC</p>
</td>
</tr>
<tr id="row1191318814260"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p132132351046"><a name="p132132351046"></a><a name="p132132351046"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p6214335144"><a name="p6214335144"></a><a name="p6214335144"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p22143353413"><a name="p22143353413"></a><a name="p22143353413"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p82141351341"><a name="p82141351341"></a><a name="p82141351341"></a>VPC的描述信息。可以使用该字段过滤VPC</p>
</td>
</tr>
<tr id="row6209113510411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1521212352410"><a name="p1521212352410"></a><a name="p1521212352410"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p1821211351046"><a name="p1821211351046"></a><a name="p1821211351046"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p5213153517414"><a name="p5213153517414"></a><a name="p5213153517414"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p62133350413"><a name="p62133350413"></a><a name="p62133350413"></a>VPC的CIDR。可以使用该字段过滤VPC</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section0225535943"></a>

无

## 请求示例<a name="section357011351949"></a>

-   查询VPC列表

    ```
    "GET https://{Endpoint}/v3/{project_id}/vpc/vpcs"
    ```


-   使用ID过滤查询VPC列表

    ```
    "GET https://{Endpoint}/v3/{project_id}/vpc/vpcs?id=01ab4be1-4447-45fb-94be-3ee787ed4ebe&id=02cd5ef2-4447-36fb-75be-3ee787ed6adf"
    ```

-   使用name过滤查询VPC列表

    ```
    "GET https://{Endpoint}/v3/{project_id}/vpc/vpcs?name=vpc-test"
    ```

-   分页查询VPC列表

    ```
    "GET https://{Endpoint}/v3/{project_id}/vpc/vpcs?limit=2&marker=01ab4be1-4447-45fb-94be-3ee787ed4ebe"
    ```


## 响应参数<a name="section6230103513419"></a>

**状态码为 200 时:**

**表 3**  响应Body参数

<a name="zh-cn_topic_0267488966_responseParameter"></a>
<table><thead align="left"><tr id="row1523115359413"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p52324351245"><a name="p52324351245"></a><a name="p52324351245"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p112337353418"><a name="p112337353418"></a><a name="p112337353418"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p122334351845"><a name="p122334351845"></a><a name="p122334351845"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row132314355420"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1623443512410"><a name="p1623443512410"></a><a name="p1623443512410"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1223416357410"><a name="p1223416357410"></a><a name="p1223416357410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2023412358419"><a name="p2023412358419"></a><a name="p2023412358419"></a>请求ID</p>
</td>
</tr>
<tr id="row1231183511414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1823514351147"><a name="p1823514351147"></a><a name="p1823514351147"></a>vpcs</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p523512352411"><a name="p523512352411"></a><a name="p523512352411"></a>Array of <a href="#zh-cn_topic_0267488966_response_Vpc">Vpc</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p623710350414"><a name="p623710350414"></a><a name="p623710350414"></a>VPC列表响应体</p>
</td>
</tr>
<tr id="row823193512418"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1923711352411"><a name="p1923711352411"></a><a name="p1923711352411"></a>page_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p723816351845"><a name="p723816351845"></a><a name="p723816351845"></a><a href="#zh-cn_topic_0267488966_response_PageInfo">PageInfo</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p72388359412"><a name="p72388359412"></a><a name="p72388359412"></a>分页信息</p>
</td>
</tr>
</tbody>
</table>

**表 4**  Vpc

<a name="zh-cn_topic_0267488966_response_Vpc"></a>
<table><thead align="left"><tr id="row32401335442"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1924415358410"><a name="p1924415358410"></a><a name="p1924415358410"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p112452351441"><a name="p112452351441"></a><a name="p112452351441"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p182453351149"><a name="p182453351149"></a><a name="p182453351149"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row202401735343"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p182459358417"><a name="p182459358417"></a><a name="p182459358417"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1224611359417"><a name="p1224611359417"></a><a name="p1224611359417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p147621949123014"><a name="p147621949123014"></a><a name="p147621949123014"></a>功能描述：VPC对应的唯一标识</p>
<p id="p1624615351749"><a name="p1624615351749"></a><a name="p1624615351749"></a>取值范围：带“-”的UUID格式</p>
</td>
</tr>
<tr id="row1324112353419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2024743519418"><a name="p2024743519418"></a><a name="p2024743519418"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p202470351349"><a name="p202470351349"></a><a name="p202470351349"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1861522303"><a name="p1861522303"></a><a name="p1861522303"></a>功能说明：VPC对应的名称</p>
<p id="p1424763515411"><a name="p1424763515411"></a><a name="p1424763515411"></a>取值范围：0-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</p>
</td>
</tr>
<tr id="row924119351741"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3248193512418"><a name="p3248193512418"></a><a name="p3248193512418"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p224810353417"><a name="p224810353417"></a><a name="p224810353417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8400159163012"><a name="p8400159163012"></a><a name="p8400159163012"></a>功能说明：VPC的描述信息</p>
<p id="p724933520410"><a name="p724933520410"></a><a name="p724933520410"></a>取值范围：0-255个字符，不能包含“&lt;”和“&gt;”</p>
</td>
</tr>
<tr id="row72415350414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p724943517413"><a name="p724943517413"></a><a name="p724943517413"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p82501435142"><a name="p82501435142"></a><a name="p82501435142"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6822171083113"><a name="p6822171083113"></a><a name="p6822171083113"></a>功能说明：VPC下可用子网的范围</p>
<p id="p102501135945"><a name="p102501135945"></a><a name="p102501135945"></a>取值范围：</p>
<a name="ul1125017358417"></a><a name="ul1125017358417"></a><ul id="ul1125017358417"><li>10.0.0.0/8~10.255.255.240/28</li><li>172.16.0.0/12 ~ 172.31.255.240/28</li><li>192.168.0.0/16 ~ 192.168.255.240/28</li></ul>
<p id="p43640344319"><a name="p43640344319"></a><a name="p43640344319"></a>不指定cidr时，默认值为“”</p>
<a name="ul1375143493111"></a><a name="ul1375143493111"></a><ul id="ul1375143493111"><li>约束：必须是ipv4 cidr格式，例如:192.168.0.0/16</li></ul>
</td>
</tr>
<tr id="row1924117352412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p102514351449"><a name="p102514351449"></a><a name="p102514351449"></a>extend_cidrs</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22520352411"><a name="p22520352411"></a><a name="p22520352411"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p183445114323"><a name="p183445114323"></a><a name="p183445114323"></a>功能描述：VPC的扩展网段</p>
<p id="p10962252328"><a name="p10962252328"></a><a name="p10962252328"></a>取值范围：</p>
<p id="p1253113511411"><a name="p1253113511411"></a><a name="p1253113511411"></a>约束：目前只支持ipv4</p>
</td>
</tr>
<tr id="row724112351846"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p112545351547"><a name="p112545351547"></a><a name="p112545351547"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1255235744"><a name="p1255235744"></a><a name="p1255235744"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p158881511334"><a name="p158881511334"></a><a name="p158881511334"></a>功能说明：VPC对应的状态</p>
<div class="p" id="p149071393317"><a name="p149071393317"></a><a name="p149071393317"></a>取值范围：<a name="ul13491816153310"></a><a name="ul13491816153310"></a><ul id="ul13491816153310"><li>PENDING：创建中</li><li>ACTIVE：创建成功</li></ul>
</div>
</td>
</tr>
<tr id="row1424218354418"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12572351742"><a name="p12572351742"></a><a name="p12572351742"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p625714351042"><a name="p625714351042"></a><a name="p625714351042"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p925819351443"><a name="p925819351443"></a><a name="p925819351443"></a>功能说明：VPC所属的项目ID</p>
</td>
</tr>
<tr id="row624211355411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p625811359417"><a name="p625811359417"></a><a name="p625811359417"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p182590351748"><a name="p182590351748"></a><a name="p182590351748"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p181707261335"><a name="p181707261335"></a><a name="p181707261335"></a>功能说明：VPC所属的企业项目ID。</p>
<p id="p7259635047"><a name="p7259635047"></a><a name="p7259635047"></a>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。</p>
</td>
</tr>
<tr id="row524213517410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p132591351943"><a name="p132591351943"></a><a name="p132591351943"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62603351646"><a name="p62603351646"></a><a name="p62603351646"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5516102920336"><a name="p5516102920336"></a><a name="p5516102920336"></a>功能说明：VPC创建时间</p>
<p id="p1326073514414"><a name="p1326073514414"></a><a name="p1326073514414"></a>取值范围：UTC时间格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row16242835448"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p132603351414"><a name="p132603351414"></a><a name="p132603351414"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p132615351242"><a name="p132615351242"></a><a name="p132615351242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p021217337338"><a name="p021217337338"></a><a name="p021217337338"></a>功能说明：VPC更新时间</p>
<p id="p152612351445"><a name="p152612351445"></a><a name="p152612351445"></a>取值范围：UTC时间格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row102421351647"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p226118357412"><a name="p226118357412"></a><a name="p226118357412"></a>cloud_resources</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19262103516411"><a name="p19262103516411"></a><a name="p19262103516411"></a>Array of <a href="#zh-cn_topic_0267488966_response_CloudResource">CloudResource</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p66552345330"><a name="p66552345330"></a><a name="p66552345330"></a>功能说明：VPC关联资源类型和数量</p>
<p id="p16262153515419"><a name="p16262153515419"></a><a name="p16262153515419"></a>取值范围：目前只返回VPC关联的routetable和virsubnet</p>
</td>
</tr>
<tr id="row32421735447"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p826214352419"><a name="p826214352419"></a><a name="p826214352419"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1826319351949"><a name="p1826319351949"></a><a name="p1826319351949"></a>Array of <a href="#zh-cn_topic_0267488966_response_Tag">Tag</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5529164010339"><a name="p5529164010339"></a><a name="p5529164010339"></a>功能说明：VPC的标签信息，详情参见Tag对象</p>
<p id="p1126323517413"><a name="p1126323517413"></a><a name="p1126323517413"></a>取值范围：0-10个标签键值对</p>
</td>
</tr>
</tbody>
</table>

**表 5**  CloudResource

<a name="zh-cn_topic_0267488966_response_CloudResource"></a>
<table><thead align="left"><tr id="row7264735641"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p22653355416"><a name="p22653355416"></a><a name="p22653355416"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p226517354416"><a name="p226517354416"></a><a name="p226517354416"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p0265203514415"><a name="p0265203514415"></a><a name="p0265203514415"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1726414351846"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p42667351410"><a name="p42667351410"></a><a name="p42667351410"></a>resource_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6266735148"><a name="p6266735148"></a><a name="p6266735148"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p726717351948"><a name="p726717351948"></a><a name="p726717351948"></a>功能描述：资源类型</p>
</td>
</tr>
<tr id="row92641435649"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1626710351418"><a name="p1626710351418"></a><a name="p1626710351418"></a>resource_count</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62672351416"><a name="p62672351416"></a><a name="p62672351416"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p926819353412"><a name="p926819353412"></a><a name="p926819353412"></a>功能说明：资源数量</p>
</td>
</tr>
</tbody>
</table>

**表 6**  Tag

<a name="zh-cn_topic_0267488966_response_Tag"></a>
<table><thead align="left"><tr id="row2269835745"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p527019351344"><a name="p527019351344"></a><a name="p527019351344"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1827016358412"><a name="p1827016358412"></a><a name="p1827016358412"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p72711351842"><a name="p72711351842"></a><a name="p72711351842"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1426911354410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1227219351348"><a name="p1227219351348"></a><a name="p1227219351348"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1827213357411"><a name="p1827213357411"></a><a name="p1827213357411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p573942310345"><a name="p573942310345"></a><a name="p573942310345"></a>功能说明：标签键</p>
<div class="p" id="p1656442820345"><a name="p1656442820345"></a><a name="p1656442820345"></a>取值范围：<a name="ul10307153213414"></a><a name="ul10307153213414"></a><ul id="ul10307153213414"><li>最大长度36个unicode字符。</li><li>key不能为空。不能包含非打印字符ASCII(0-31)，*,&lt;,&gt;,,=</li></ul>
</div>
</td>
</tr>
<tr id="row172691535946"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p727323511410"><a name="p727323511410"></a><a name="p727323511410"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p192735351744"><a name="p192735351744"></a><a name="p192735351744"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p188224345344"><a name="p188224345344"></a><a name="p188224345344"></a>功能描述：标签值</p>
<p id="p1782104073410"><a name="p1782104073410"></a><a name="p1782104073410"></a>取值范围：</p>
<a name="ul4352184273414"></a><a name="ul4352184273414"></a><ul id="ul4352184273414"><li>每个值最大长度43个unicode字符，可以为空字符串。</li><li>不能包含非打印字符ASCII(0-31)，*,&lt;,&gt;,,=</li></ul>
</td>
</tr>
</tbody>
</table>

**表 7**  PageInfo

<a name="zh-cn_topic_0267488966_response_PageInfo"></a>
<table><thead align="left"><tr id="row127512351840"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p14276133519410"><a name="p14276133519410"></a><a name="p14276133519410"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p92768354414"><a name="p92768354414"></a><a name="p92768354414"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p11277103519412"><a name="p11277103519412"></a><a name="p11277103519412"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row16275123512416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12771935242"><a name="p12771935242"></a><a name="p12771935242"></a>previous_marker</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1277935843"><a name="p1277935843"></a><a name="p1277935843"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15278153510411"><a name="p15278153510411"></a><a name="p15278153510411"></a>当前页第一条记录</p>
</td>
</tr>
<tr id="row627517351846"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1127833516414"><a name="p1127833516414"></a><a name="p1127833516414"></a>current_count</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p202788357417"><a name="p202788357417"></a><a name="p202788357417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2279203518419"><a name="p2279203518419"></a><a name="p2279203518419"></a>当前页总数</p>
</td>
</tr>
<tr id="row4275143520410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12791351843"><a name="p12791351843"></a><a name="p12791351843"></a>next_marker</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1027943516412"><a name="p1027943516412"></a><a name="p1027943516412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19280113517416"><a name="p19280113517416"></a><a name="p19280113517416"></a>当前页最后一条记录，最后一页时无next_marker字段</p>
</td>
</tr>
</tbody>
</table>

**状态码为 400 时:**

**表 8**  响应Body参数

<a name="table428010351647"></a>
<table><thead align="left"><tr id="row1128173514419"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1228218351443"><a name="p1228218351443"></a><a name="p1228218351443"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p3282163510414"><a name="p3282163510414"></a><a name="p3282163510414"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p52833351646"><a name="p52833351646"></a><a name="p52833351646"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1028118352416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1728483512413"><a name="p1728483512413"></a><a name="p1728483512413"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p628453519413"><a name="p628453519413"></a><a name="p628453519413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16285203517415"><a name="p16285203517415"></a><a name="p16285203517415"></a>请求ID</p>
</td>
</tr>
<tr id="row628123514416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2028716351740"><a name="p2028716351740"></a><a name="p2028716351740"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22871635143"><a name="p22871635143"></a><a name="p22871635143"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p162891351345"><a name="p162891351345"></a><a name="p162891351345"></a>错误消息</p>
</td>
</tr>
<tr id="row102816351047"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p182892350418"><a name="p182892350418"></a><a name="p182892350418"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p182896351642"><a name="p182896351642"></a><a name="p182896351642"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10290173515418"><a name="p10290173515418"></a><a name="p10290173515418"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 401 时:**

**表 9**  响应Body参数

<a name="table1029014351342"></a>
<table><thead align="left"><tr id="row112913351544"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p229213517420"><a name="p229213517420"></a><a name="p229213517420"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p7293203517413"><a name="p7293203517413"></a><a name="p7293203517413"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p429314351845"><a name="p429314351845"></a><a name="p429314351845"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row22911235748"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p529318351645"><a name="p529318351645"></a><a name="p529318351645"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p52941735845"><a name="p52941735845"></a><a name="p52941735845"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2029416357413"><a name="p2029416357413"></a><a name="p2029416357413"></a>请求ID</p>
</td>
</tr>
<tr id="row14291153512415"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10294123511414"><a name="p10294123511414"></a><a name="p10294123511414"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p82957357411"><a name="p82957357411"></a><a name="p82957357411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1929583512415"><a name="p1929583512415"></a><a name="p1929583512415"></a>错误消息</p>
</td>
</tr>
<tr id="row19291143518419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9295143513416"><a name="p9295143513416"></a><a name="p9295143513416"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18296935748"><a name="p18296935748"></a><a name="p18296935748"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1729613510416"><a name="p1729613510416"></a><a name="p1729613510416"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 403 时:**

**表 10**  响应Body参数

<a name="table1229614356410"></a>
<table><thead align="left"><tr id="row62973351247"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p192986356410"><a name="p192986356410"></a><a name="p192986356410"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1829816354419"><a name="p1829816354419"></a><a name="p1829816354419"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1029912357410"><a name="p1029912357410"></a><a name="p1029912357410"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row7297173513412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4299103510415"><a name="p4299103510415"></a><a name="p4299103510415"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p729923513411"><a name="p729923513411"></a><a name="p729923513411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p153009353418"><a name="p153009353418"></a><a name="p153009353418"></a>请求ID</p>
</td>
</tr>
<tr id="row229717359410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1530017351848"><a name="p1530017351848"></a><a name="p1530017351848"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1256215351410"><a name="p1256215351410"></a><a name="p1256215351410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p356214351942"><a name="p356214351942"></a><a name="p356214351942"></a>错误消息</p>
</td>
</tr>
<tr id="row1329716355410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12562173515419"><a name="p12562173515419"></a><a name="p12562173515419"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p205625351844"><a name="p205625351844"></a><a name="p205625351844"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p25622358420"><a name="p25622358420"></a><a name="p25622358420"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 404 时:**

**表 11**  响应Body参数

<a name="table330313351242"></a>
<table><thead align="left"><tr id="row1130413516412"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1456213354414"><a name="p1456213354414"></a><a name="p1456213354414"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p7562335347"><a name="p7562335347"></a><a name="p7562335347"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p7562335746"><a name="p7562335746"></a><a name="p7562335746"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row15304123510412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p85626351042"><a name="p85626351042"></a><a name="p85626351042"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1256216351247"><a name="p1256216351247"></a><a name="p1256216351247"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16563103515419"><a name="p16563103515419"></a><a name="p16563103515419"></a>请求ID</p>
</td>
</tr>
<tr id="row173048358410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p185630351349"><a name="p185630351349"></a><a name="p185630351349"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p155636351640"><a name="p155636351640"></a><a name="p155636351640"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4563935747"><a name="p4563935747"></a><a name="p4563935747"></a>错误消息</p>
</td>
</tr>
<tr id="row10304143517411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p135630356413"><a name="p135630356413"></a><a name="p135630356413"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p256319359411"><a name="p256319359411"></a><a name="p256319359411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1556303520412"><a name="p1556303520412"></a><a name="p1556303520412"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 409 时:**

**表 12**  响应Body参数

<a name="table1331215353419"></a>
<table><thead align="left"><tr id="row6312335545"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p3564835645"><a name="p3564835645"></a><a name="p3564835645"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p656417353415"><a name="p656417353415"></a><a name="p656417353415"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p256453511413"><a name="p256453511413"></a><a name="p256453511413"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1531263510412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p256411351142"><a name="p256411351142"></a><a name="p256411351142"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p65641135842"><a name="p65641135842"></a><a name="p65641135842"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p105647354412"><a name="p105647354412"></a><a name="p105647354412"></a>请求ID</p>
</td>
</tr>
<tr id="row63122358414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1256414358415"><a name="p1256414358415"></a><a name="p1256414358415"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7564133510419"><a name="p7564133510419"></a><a name="p7564133510419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p356483519415"><a name="p356483519415"></a><a name="p356483519415"></a>错误消息</p>
</td>
</tr>
<tr id="row133123351544"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p75643351047"><a name="p75643351047"></a><a name="p75643351047"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17569435242"><a name="p17569435242"></a><a name="p17569435242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p165691735946"><a name="p165691735946"></a><a name="p165691735946"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 500 时:**

**表 13**  响应Body参数

<a name="table13218354416"></a>
<table><thead align="left"><tr id="row103223351844"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p195691435149"><a name="p195691435149"></a><a name="p195691435149"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p135699351649"><a name="p135699351649"></a><a name="p135699351649"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p15706351941"><a name="p15706351941"></a><a name="p15706351941"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1232210356413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p457063513419"><a name="p457063513419"></a><a name="p457063513419"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p857073516419"><a name="p857073516419"></a><a name="p857073516419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4570103518414"><a name="p4570103518414"></a><a name="p4570103518414"></a>请求ID</p>
</td>
</tr>
<tr id="row1532210352417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p125701235143"><a name="p125701235143"></a><a name="p125701235143"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p45701435142"><a name="p45701435142"></a><a name="p45701435142"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p135701035544"><a name="p135701035544"></a><a name="p135701035544"></a>错误消息</p>
</td>
</tr>
<tr id="row1132218351945"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4570133520418"><a name="p4570133520418"></a><a name="p4570133520418"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p557014351417"><a name="p557014351417"></a><a name="p557014351417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4570163517415"><a name="p4570163517415"></a><a name="p4570163517415"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

## 响应示例<a name="section857011352414"></a>

**状态码为 200 时:**

OK

```
{
    "request_id": "9c1838ba498249547be43dd618b58d27", 
    "vpcs": [
        {
            "id": "01da5a65-0bb9-4638-8ab7-74c64e24a9a7", 
            "name": "API-PERF-TEST-14bd44c121", 
            "description": "", 
            "cidr": "192.168.0.0/16", 
            "extend_cidrs": [ ], 
            "status": "ACTIVE", 
            "project_id": "087679f0aa80d32a2f4ec0172f5e902b", 
            "enterprise_project_id": "0", 
            "tags": [ ], 
            "created_at": "2020-06-16T02:32:18Z", 
            "updated_at": "2020-06-16T02:32:18Z", 
            "cloud_resources": [
                {
                    "resource_type": "routetable", 
                    "resource_count": 1
                }, 
                {
                    "resource_type": "virsubnet", 
                    "resource_count": 0
                }
            ]
        }, 
        {
            "id": "43fd79b0-f7d7-4e9b-828b-2d4d7bfae428", 
            "name": "API-PERF-TEST_m2n33", 
            "description": "", 
            "cidr": "192.168.0.0/16", 
            "extend_cidrs": [ ], 
            "status": "ACTIVE", 
            "project_id": "087679f0aa80d32a2f4ec0172f5e902b", 
            "enterprise_project_id": "0", 
            "tags": [ ], 
            "created_at": "2020-06-15T06:29:40Z", 
            "updated_at": "2020-06-15T06:29:41Z", 
            "cloud_resources": [
                {
                    "resource_type": "routetable", 
                    "resource_count": 1
                }, 
                {
                    "resource_type": "virsubnet", 
                    "resource_count": 1
                }
            ]
        }, 
        {
            "id": "5ed053ba-b46c-4dce-a1ae-e9d8a7015f21", 
            "name": "API-PERF-TEST-c34b1c4b12", 
            "description": "", 
            "cidr": "192.168.0.0/16", 
            "extend_cidrs": [ ], 
            "status": "ACTIVE", 
            "project_id": "087679f0aa80d32a2f4ec0172f5e902b", 
            "enterprise_project_id": "0", 
            "tags": [ ], 
            "created_at": "2020-06-16T02:32:33Z", 
            "updated_at": "2020-06-16T02:32:33Z", 
            "cloud_resources": [
                {
                    "resource_type": "routetable", 
                    "resource_count": 1
                }, 
                {
                    "resource_type": "virsubnet", 
                    "resource_count": 0
                }
            ]
        }
    ], 
    "page_info": {
        "previous_marker": "01da5a65-0bb9-4638-8ab7-74c64e24a9a7", 
        "current_count": 3
    }
}
```

## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section936082313394"></a>

请参见[错误码](错误码.md)。

