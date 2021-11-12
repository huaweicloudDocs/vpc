# 查询VPC详情<a name="vpc_apiv3_0004"></a>

## 功能介绍<a name="section174284242563"></a>

查询vpc详情

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v3&api=ShowVpc)中直接运行调试该接口。

## URI<a name="section1442942465615"></a>

GET /v3/\{project\_id\}/vpc/vpcs/\{vpc\_id\}

**表 1**  参数说明

<a name="table1743192435614"></a>
<table><thead align="left"><tr id="row19430724105616"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p443114247564"><a name="p443114247564"></a><a name="p443114247564"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p543292465620"><a name="p543292465620"></a><a name="p543292465620"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1943314249568"><a name="p1943314249568"></a><a name="p1943314249568"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p843372415568"><a name="p843372415568"></a><a name="p843372415568"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row144301924125610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="vpc_apiv3_0010_p5360162664920"><a name="vpc_apiv3_0010_p5360162664920"></a><a name="vpc_apiv3_0010_p5360162664920"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="vpc_apiv3_0010_p18360192644917"><a name="vpc_apiv3_0010_p18360192644917"></a><a name="vpc_apiv3_0010_p18360192644917"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="vpc_apiv3_0010_p12056351843"><a name="vpc_apiv3_0010_p12056351843"></a><a name="vpc_apiv3_0010_p12056351843"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="vpc_apiv3_0010_p9930182615482"><a name="vpc_apiv3_0010_p9930182615482"></a><a name="vpc_apiv3_0010_p9930182615482"></a>项目ID。</p>
<p id="vpc_apiv3_0010_p10487112"><a name="vpc_apiv3_0010_p10487112"></a><a name="vpc_apiv3_0010_p10487112"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row15430192495610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p184371624145612"><a name="p184371624145612"></a><a name="p184371624145612"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p5438824115618"><a name="p5438824115618"></a><a name="p5438824115618"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p343852415563"><a name="p343852415563"></a><a name="p343852415563"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p1043892418561"><a name="p1043892418561"></a><a name="p1043892418561"></a>VPC资源ID</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section943912411565"></a>

无

## 请求示例<a name="section05211924145620"></a>

-   查询vpc详情

    ```
    "GET https://{Endpoint}/v3/{project_id}/vpc/vpcs/99d9d709-8478-4b46-9f3f-2206b1023fd3"
    ```


## 响应参数<a name="section84451724115618"></a>

**状态码为 200 时:**

**表 2**  响应Body参数

<a name="zh-cn_topic_0267488955_responseParameter"></a>
<table><thead align="left"><tr id="row134471224145616"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p3448112416565"><a name="p3448112416565"></a><a name="p3448112416565"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p16449112435612"><a name="p16449112435612"></a><a name="p16449112435612"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p24501724155614"><a name="p24501724155614"></a><a name="p24501724155614"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row54471724115615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4451112425615"><a name="p4451112425615"></a><a name="p4451112425615"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p645232413566"><a name="p645232413566"></a><a name="p645232413566"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p846042485612"><a name="p846042485612"></a><a name="p846042485612"></a>请求ID</p>
</td>
</tr>
<tr id="row744752411560"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7461172410567"><a name="p7461172410567"></a><a name="p7461172410567"></a>vpc</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14462202455611"><a name="p14462202455611"></a><a name="p14462202455611"></a><a href="#zh-cn_topic_0267488955_response_Vpc">Vpc</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p84632024195617"><a name="p84632024195617"></a><a name="p84632024195617"></a>VPC响应体</p>
</td>
</tr>
</tbody>
</table>

**表 3**  Vpc

<a name="zh-cn_topic_0267488955_response_Vpc"></a>
<table><thead align="left"><tr id="row58802032114110"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p888063219415"><a name="p888063219415"></a><a name="p888063219415"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p168801332134117"><a name="p168801332134117"></a><a name="p168801332134117"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1088063215417"><a name="p1088063215417"></a><a name="p1088063215417"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row989013214413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1689093216410"><a name="p1689093216410"></a><a name="p1689093216410"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17890632154112"><a name="p17890632154112"></a><a name="p17890632154112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15890123234111"><a name="p15890123234111"></a><a name="p15890123234111"></a>功能描述：VPC对应的唯一标识</p>
<p id="p589013215410"><a name="p589013215410"></a><a name="p589013215410"></a>取值范围：带“-”的UUID格式</p>
</td>
</tr>
<tr id="row2890133214117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10890143218418"><a name="p10890143218418"></a><a name="p10890143218418"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7890183234112"><a name="p7890183234112"></a><a name="p7890183234112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p68909325415"><a name="p68909325415"></a><a name="p68909325415"></a>功能说明：VPC对应的名称</p>
<p id="p1289015326417"><a name="p1289015326417"></a><a name="p1289015326417"></a>取值范围：0-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</p>
</td>
</tr>
<tr id="row78901532134110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p148903323412"><a name="p148903323412"></a><a name="p148903323412"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19890103284111"><a name="p19890103284111"></a><a name="p19890103284111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p289083210412"><a name="p289083210412"></a><a name="p289083210412"></a>功能说明：VPC的描述信息</p>
<p id="p28901532134116"><a name="p28901532134116"></a><a name="p28901532134116"></a>取值范围：0-255个字符，不能包含“&lt;”和“&gt;”</p>
</td>
</tr>
<tr id="row8891133214115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p889063220419"><a name="p889063220419"></a><a name="p889063220419"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p489020328416"><a name="p489020328416"></a><a name="p489020328416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1589033214419"><a name="p1589033214419"></a><a name="p1589033214419"></a>功能说明：VPC下可用子网的范围</p>
<p id="p178901532114110"><a name="p178901532114110"></a><a name="p178901532114110"></a>取值范围：</p>
<a name="ul1589163214411"></a><a name="ul1589163214411"></a><ul id="ul1589163214411"><li>10.0.0.0/8~10.255.255.240/28</li><li>172.16.0.0/12 ~ 172.31.255.240/28</li><li>192.168.0.0/16 ~ 192.168.255.240/28</li></ul>
<p id="p3891632154115"><a name="p3891632154115"></a><a name="p3891632154115"></a>不指定cidr时，默认值为“”</p>
<a name="ul17891123224111"></a><a name="ul17891123224111"></a><ul id="ul17891123224111"><li>约束：必须是ipv4 cidr格式，例如:192.168.0.0/16</li></ul>
</td>
</tr>
<tr id="row19891133210413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4891163219415"><a name="p4891163219415"></a><a name="p4891163219415"></a>extend_cidrs</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p589153284115"><a name="p589153284115"></a><a name="p589153284115"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10891173214411"><a name="p10891173214411"></a><a name="p10891173214411"></a>功能描述：VPC的扩展网段</p>
<p id="p12891153218410"><a name="p12891153218410"></a><a name="p12891153218410"></a>取值范围：</p>
<p id="p28911532194112"><a name="p28911532194112"></a><a name="p28911532194112"></a>约束：目前只支持ipv4</p>
</td>
</tr>
<tr id="row1089116325417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13891193211415"><a name="p13891193211415"></a><a name="p13891193211415"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6891163210418"><a name="p6891163210418"></a><a name="p6891163210418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19891932124114"><a name="p19891932124114"></a><a name="p19891932124114"></a>功能说明：VPC对应的状态</p>
<div class="p" id="p10891163284118"><a name="p10891163284118"></a><a name="p10891163284118"></a>取值范围：<a name="ul5891132154119"></a><a name="ul5891132154119"></a><ul id="ul5891132154119"><li>PENDING：创建中</li><li>ACTIVE：创建成功</li></ul>
</div>
</td>
</tr>
<tr id="row1891232114113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p489115325418"><a name="p489115325418"></a><a name="p489115325418"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1689112325416"><a name="p1689112325416"></a><a name="p1689112325416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p158918328418"><a name="p158918328418"></a><a name="p158918328418"></a>功能说明：VPC所属的项目ID</p>
</td>
</tr>
<tr id="row128917323418"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p289113215419"><a name="p289113215419"></a><a name="p289113215419"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2891163274115"><a name="p2891163274115"></a><a name="p2891163274115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7891153214119"><a name="p7891153214119"></a><a name="p7891153214119"></a>功能说明：VPC所属的企业项目ID。</p>
<p id="p4891832194110"><a name="p4891832194110"></a><a name="p4891832194110"></a>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。</p>
</td>
</tr>
<tr id="row6892032174112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p78927329416"><a name="p78927329416"></a><a name="p78927329416"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11892532144113"><a name="p11892532144113"></a><a name="p11892532144113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1892133214418"><a name="p1892133214418"></a><a name="p1892133214418"></a>功能说明：VPC创建时间</p>
<p id="p789212325415"><a name="p789212325415"></a><a name="p789212325415"></a>取值范围：UTC时间格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row5892132194112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1289273220417"><a name="p1289273220417"></a><a name="p1289273220417"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p158928325418"><a name="p158928325418"></a><a name="p158928325418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5892113218419"><a name="p5892113218419"></a><a name="p5892113218419"></a>功能说明：VPC更新时间</p>
<p id="p28921032204117"><a name="p28921032204117"></a><a name="p28921032204117"></a>取值范围：UTC时间格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row10892193214110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p789243213419"><a name="p789243213419"></a><a name="p789243213419"></a>cloud_resources</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1189211327418"><a name="p1189211327418"></a><a name="p1189211327418"></a>Array of <a href="#zh-cn_topic_0267488955_response_CloudResource">CloudResource</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p789213216416"><a name="p789213216416"></a><a name="p789213216416"></a>功能说明：VPC关联资源类型和数量</p>
<p id="p19892232114111"><a name="p19892232114111"></a><a name="p19892232114111"></a>取值范围：目前只返回VPC关联的routetable和virsubnet</p>
</td>
</tr>
<tr id="row1589253264110"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p489243224118"><a name="p489243224118"></a><a name="p489243224118"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20892232164116"><a name="p20892232164116"></a><a name="p20892232164116"></a>Array of <a href="#zh-cn_topic_0267488955_response_Tag">Tag</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p689273284110"><a name="p689273284110"></a><a name="p689273284110"></a>功能说明：VPC的标签信息，详情参见Tag对象</p>
<p id="p17892163234120"><a name="p17892163234120"></a><a name="p17892163234120"></a>取值范围：0-10个标签键值对</p>
</td>
</tr>
</tbody>
</table>

**表 4**  CloudResource

<a name="zh-cn_topic_0267488955_response_CloudResource"></a>
<table><thead align="left"><tr id="vpc_apiv3_0003_row7264735641"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="vpc_apiv3_0003_p22653355416"><a name="vpc_apiv3_0003_p22653355416"></a><a name="vpc_apiv3_0003_p22653355416"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="vpc_apiv3_0003_p226517354416"><a name="vpc_apiv3_0003_p226517354416"></a><a name="vpc_apiv3_0003_p226517354416"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="vpc_apiv3_0003_p0265203514415"><a name="vpc_apiv3_0003_p0265203514415"></a><a name="vpc_apiv3_0003_p0265203514415"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_apiv3_0003_row1726414351846"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="vpc_apiv3_0003_p42667351410"><a name="vpc_apiv3_0003_p42667351410"></a><a name="vpc_apiv3_0003_p42667351410"></a>resource_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="vpc_apiv3_0003_p6266735148"><a name="vpc_apiv3_0003_p6266735148"></a><a name="vpc_apiv3_0003_p6266735148"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="vpc_apiv3_0003_p726717351948"><a name="vpc_apiv3_0003_p726717351948"></a><a name="vpc_apiv3_0003_p726717351948"></a>功能描述：资源类型</p>
</td>
</tr>
<tr id="vpc_apiv3_0003_row92641435649"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="vpc_apiv3_0003_p1626710351418"><a name="vpc_apiv3_0003_p1626710351418"></a><a name="vpc_apiv3_0003_p1626710351418"></a>resource_count</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="vpc_apiv3_0003_p62672351416"><a name="vpc_apiv3_0003_p62672351416"></a><a name="vpc_apiv3_0003_p62672351416"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="vpc_apiv3_0003_p926819353412"><a name="vpc_apiv3_0003_p926819353412"></a><a name="vpc_apiv3_0003_p926819353412"></a>功能说明：资源数量</p>
</td>
</tr>
</tbody>
</table>

**表 5**  Tag

<a name="zh-cn_topic_0267488955_response_Tag"></a>
<table><thead align="left"><tr id="vpc_apiv3_0003_row2269835745"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="vpc_apiv3_0003_p527019351344"><a name="vpc_apiv3_0003_p527019351344"></a><a name="vpc_apiv3_0003_p527019351344"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="vpc_apiv3_0003_p1827016358412"><a name="vpc_apiv3_0003_p1827016358412"></a><a name="vpc_apiv3_0003_p1827016358412"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="vpc_apiv3_0003_p72711351842"><a name="vpc_apiv3_0003_p72711351842"></a><a name="vpc_apiv3_0003_p72711351842"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_apiv3_0003_row1426911354410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="vpc_apiv3_0003_p1227219351348"><a name="vpc_apiv3_0003_p1227219351348"></a><a name="vpc_apiv3_0003_p1227219351348"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="vpc_apiv3_0003_p1827213357411"><a name="vpc_apiv3_0003_p1827213357411"></a><a name="vpc_apiv3_0003_p1827213357411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="vpc_apiv3_0003_p573942310345"><a name="vpc_apiv3_0003_p573942310345"></a><a name="vpc_apiv3_0003_p573942310345"></a>功能说明：标签键</p>
<div class="p" id="vpc_apiv3_0003_p1656442820345"><a name="vpc_apiv3_0003_p1656442820345"></a><a name="vpc_apiv3_0003_p1656442820345"></a>取值范围：<a name="vpc_apiv3_0003_ul10307153213414"></a><a name="vpc_apiv3_0003_ul10307153213414"></a><ul id="vpc_apiv3_0003_ul10307153213414"><li>最大长度36个unicode字符。</li><li>key不能为空。不能包含非打印字符ASCII(0-31)，*,&lt;,&gt;,,=</li></ul>
</div>
</td>
</tr>
<tr id="vpc_apiv3_0003_row172691535946"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="vpc_apiv3_0003_p727323511410"><a name="vpc_apiv3_0003_p727323511410"></a><a name="vpc_apiv3_0003_p727323511410"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="vpc_apiv3_0003_p192735351744"><a name="vpc_apiv3_0003_p192735351744"></a><a name="vpc_apiv3_0003_p192735351744"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="vpc_apiv3_0003_p188224345344"><a name="vpc_apiv3_0003_p188224345344"></a><a name="vpc_apiv3_0003_p188224345344"></a>功能描述：标签值</p>
<p id="vpc_apiv3_0003_p1782104073410"><a name="vpc_apiv3_0003_p1782104073410"></a><a name="vpc_apiv3_0003_p1782104073410"></a>取值范围：</p>
<a name="vpc_apiv3_0003_ul4352184273414"></a><a name="vpc_apiv3_0003_ul4352184273414"></a><ul id="vpc_apiv3_0003_ul4352184273414"><li>每个值最大长度43个unicode字符，可以为空字符串。</li><li>不能包含非打印字符ASCII(0-31)，*,&lt;,&gt;,,=</li></ul>
</td>
</tr>
</tbody>
</table>

## 响应示例<a name="section185228243561"></a>

**状态码为 200 时:**

OK

```
{
    "request_id": "84eb4f775d66dd916db121768ec55626", 
    "vpc": {
        "id": "0552091e-b83a-49dd-88a7-4a5c86fd9ec3", 
        "name": "name-test", 
        "description": "description-test", 
        "cidr": "192.168.0.0/16", 
        "extend_cidrs": [
            "21.8.0.0/16"
        ], 
        "enterprise_project_id": "0", 
        "tags": [
            {
                "key": "key", 
                "value": "value"
            }
        ], 
        "cloud_resources": [
            {
                "resrource_type": "routetable", 
                "resrource_count": 1
            }
        ], 
        "status": "ACTIVE", 
        "project_id": "060576782980d5762f9ec014dd2f1148", 
        "created_at": "2018-03-23T09:26:08", 
        "updated_at": "2018-08-24T08:49:53"
    }
}
```

## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section936082313394"></a>

请参见[错误码](错误码.md)。

