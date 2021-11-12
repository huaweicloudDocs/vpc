# 添加VPC扩展网段<a name="vpc_apiv3_0007"></a>

## 功能介绍<a name="section78561525125619"></a>

添加VPC的扩展网段

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v3&api=AddVpcExtendCidr)中直接运行调试该接口。

## URI<a name="section48565252569"></a>

PUT /v3/\{project\_id\}/vpc/vpcs/\{vpc\_id\}/add-extend-cidr

**表 1**  参数说明

<a name="table485892585610"></a>
<table><thead align="left"><tr id="vpc_apiv3_0004_row19430724105616"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="vpc_apiv3_0004_p443114247564"><a name="vpc_apiv3_0004_p443114247564"></a><a name="vpc_apiv3_0004_p443114247564"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="vpc_apiv3_0004_p543292465620"><a name="vpc_apiv3_0004_p543292465620"></a><a name="vpc_apiv3_0004_p543292465620"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="vpc_apiv3_0004_p1943314249568"><a name="vpc_apiv3_0004_p1943314249568"></a><a name="vpc_apiv3_0004_p1943314249568"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="vpc_apiv3_0004_p843372415568"><a name="vpc_apiv3_0004_p843372415568"></a><a name="vpc_apiv3_0004_p843372415568"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_apiv3_0004_row144301924125610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="vpc_apiv3_0004_vpc_apiv3_0010_p5360162664920"><a name="vpc_apiv3_0004_vpc_apiv3_0010_p5360162664920"></a><a name="vpc_apiv3_0004_vpc_apiv3_0010_p5360162664920"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="vpc_apiv3_0004_vpc_apiv3_0010_p18360192644917"><a name="vpc_apiv3_0004_vpc_apiv3_0010_p18360192644917"></a><a name="vpc_apiv3_0004_vpc_apiv3_0010_p18360192644917"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="vpc_apiv3_0004_vpc_apiv3_0010_p12056351843"><a name="vpc_apiv3_0004_vpc_apiv3_0010_p12056351843"></a><a name="vpc_apiv3_0004_vpc_apiv3_0010_p12056351843"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="vpc_apiv3_0004_vpc_apiv3_0010_p9930182615482"><a name="vpc_apiv3_0004_vpc_apiv3_0010_p9930182615482"></a><a name="vpc_apiv3_0004_vpc_apiv3_0010_p9930182615482"></a>项目ID。</p>
<p id="vpc_apiv3_0004_vpc_apiv3_0010_p10487112"><a name="vpc_apiv3_0004_vpc_apiv3_0010_p10487112"></a><a name="vpc_apiv3_0004_vpc_apiv3_0010_p10487112"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="vpc_apiv3_0004_row15430192495610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="vpc_apiv3_0004_p184371624145612"><a name="vpc_apiv3_0004_p184371624145612"></a><a name="vpc_apiv3_0004_p184371624145612"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="vpc_apiv3_0004_p5438824115618"><a name="vpc_apiv3_0004_p5438824115618"></a><a name="vpc_apiv3_0004_p5438824115618"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="vpc_apiv3_0004_p343852415563"><a name="vpc_apiv3_0004_p343852415563"></a><a name="vpc_apiv3_0004_p343852415563"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="vpc_apiv3_0004_p1043892418561"><a name="vpc_apiv3_0004_p1043892418561"></a><a name="vpc_apiv3_0004_p1043892418561"></a>VPC资源ID</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section686512520569"></a>

**表 2**  请求Body参数

<a name="zh-cn_topic_0267488960_requestParameter"></a>
<table><thead align="left"><tr id="row188701325185614"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p0872182515566"><a name="p0872182515566"></a><a name="p0872182515566"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p20873192514565"><a name="p20873192514565"></a><a name="p20873192514565"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p108741625155618"><a name="p108741625155618"></a><a name="p108741625155618"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p68751425175611"><a name="p68751425175611"></a><a name="p68751425175611"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row7870112525611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1387542565613"><a name="p1387542565613"></a><a name="p1387542565613"></a>dry_run</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p6876202510565"><a name="p6876202510565"></a><a name="p6876202510565"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p2876142555610"><a name="p2876142555610"></a><a name="p2876142555610"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p1794843515444"><a name="p1794843515444"></a><a name="p1794843515444"></a>功能说明：是否只预检此次请求</p>
<p id="p592163714415"><a name="p592163714415"></a><a name="p592163714415"></a>取值范围：</p>
<a name="ul7832551104415"></a><a name="ul7832551104415"></a><ul id="ul7832551104415"><li>true：发送检查请求，不会添加扩展网段。检查项包括是否填写了必需参数、请求格式、业务限制。如果检查不通过，则返回对应错误。如果检查通过，则返回响应码202。</li><li>false（默认值）：发送正常请求，并直接添加VPC扩展网段。</li></ul>
</td>
</tr>
<tr id="row11871152565616"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p18877122512567"><a name="p18877122512567"></a><a name="p18877122512567"></a>vpc</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p128771225125611"><a name="p128771225125611"></a><a name="p128771225125611"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p5878122515563"><a name="p5878122515563"></a><a name="p5878122515563"></a><a href="#zh-cn_topic_0267488960_request_AddExtendCidrOption">AddExtendCidrOption</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p988116257566"><a name="p988116257566"></a><a name="p988116257566"></a>添加扩展网段请求体</p>
</td>
</tr>
</tbody>
</table>

**表 3**  AddExtendCidrOption

<a name="zh-cn_topic_0267488960_request_AddExtendCidrOption"></a>
<table><thead align="left"><tr id="row138827252566"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p16884192516565"><a name="p16884192516565"></a><a name="p16884192516565"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p688482535618"><a name="p688482535618"></a><a name="p688482535618"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p11885152515569"><a name="p11885152515569"></a><a name="p11885152515569"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p14885192519566"><a name="p14885192519566"></a><a name="p14885192519566"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row12882192517562"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1888610259563"><a name="p1888610259563"></a><a name="p1888610259563"></a>extend_cidrs</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p16886132575611"><a name="p16886132575611"></a><a name="p16886132575611"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p14887102535611"><a name="p14887102535611"></a><a name="p14887102535611"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p917012244516"><a name="p917012244516"></a><a name="p917012244516"></a>功能说明：扩展cidr列表</p>
<p id="p1997823653318"><a name="p1997823653318"></a><a name="p1997823653318"></a>取值范围：不能包含以下网段</p>
<a name="ul1194783912339"></a><a name="ul1194783912339"></a><ul id="ul1194783912339"><li>100.64.0.0/10</li><li>214.0.0.0/7</li><li>198.18.0.0/15</li><li>169.254.0.0/16</li><li>0.0.0.0/8</li><li>127.0.0.0/8</li><li>240.0.0.0/4</li><li>172.31.0.0/16</li><li>192.168.0.0/16</li></ul>
<p id="p188882025105611"><a name="p188882025105611"></a><a name="p188882025105611"></a>约束：当前只支持添加一个</p>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section3334202655618"></a>

-   给单个VPC添加扩展网段

    ```
    PUT https://{Endpoint}/v3/{project_id}/vpc/vpcs/99d9d709-8478-4b46-9f3f-2206b1023fd3/add-extend-cidr
    
    {
        "vpc": {
            "extend_cidrs": [
                "23.8.0.0/16"
            ]
        }
    }
    ```


## 响应参数<a name="section1788962535612"></a>

**状态码为 200 时:**

**表 4**  响应Body参数

<a name="zh-cn_topic_0267488960_responseParameter"></a>
<table><thead align="left"><tr id="row138921725205615"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p15893102565616"><a name="p15893102565616"></a><a name="p15893102565616"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p14893825195610"><a name="p14893825195610"></a><a name="p14893825195610"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p689342515611"><a name="p689342515611"></a><a name="p689342515611"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row289218258567"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19894132513567"><a name="p19894132513567"></a><a name="p19894132513567"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18894132585617"><a name="p18894132585617"></a><a name="p18894132585617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17895172511568"><a name="p17895172511568"></a><a name="p17895172511568"></a>请求ID</p>
</td>
</tr>
<tr id="row1489210254569"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9895112514568"><a name="p9895112514568"></a><a name="p9895112514568"></a>vpc</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p189602514562"><a name="p189602514562"></a><a name="p189602514562"></a><a href="#zh-cn_topic_0267488960_response_Vpc">Vpc</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12896192513568"><a name="p12896192513568"></a><a name="p12896192513568"></a>添加扩展网段响应体</p>
</td>
</tr>
</tbody>
</table>

**表 5**  Vpc

<a name="zh-cn_topic_0267488960_response_Vpc"></a>
<table><thead align="left"><tr id="row13378130135016"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p23781930135013"><a name="p23781930135013"></a><a name="p23781930135013"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p0378133015505"><a name="p0378133015505"></a><a name="p0378133015505"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p11378173010504"><a name="p11378173010504"></a><a name="p11378173010504"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row10387153055016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p33871330155017"><a name="p33871330155017"></a><a name="p33871330155017"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p838713025013"><a name="p838713025013"></a><a name="p838713025013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p338710303509"><a name="p338710303509"></a><a name="p338710303509"></a>功能描述：VPC对应的唯一标识</p>
<p id="p238711303506"><a name="p238711303506"></a><a name="p238711303506"></a>取值范围：带“-”的UUID格式</p>
</td>
</tr>
<tr id="row8387183010506"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1638763017503"><a name="p1638763017503"></a><a name="p1638763017503"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9387130105012"><a name="p9387130105012"></a><a name="p9387130105012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p43879309501"><a name="p43879309501"></a><a name="p43879309501"></a>功能说明：VPC对应的名称</p>
<p id="p638793005014"><a name="p638793005014"></a><a name="p638793005014"></a>取值范围：0-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</p>
</td>
</tr>
<tr id="row15387630165010"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p73875306503"><a name="p73875306503"></a><a name="p73875306503"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16387173014509"><a name="p16387173014509"></a><a name="p16387173014509"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1638753075020"><a name="p1638753075020"></a><a name="p1638753075020"></a>功能说明：VPC的描述信息</p>
<p id="p1638733020506"><a name="p1638733020506"></a><a name="p1638733020506"></a>取值范围：0-255个字符，不能包含“&lt;”和“&gt;”</p>
</td>
</tr>
<tr id="row438753014503"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1038763014502"><a name="p1038763014502"></a><a name="p1038763014502"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8387930115018"><a name="p8387930115018"></a><a name="p8387930115018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8387183016507"><a name="p8387183016507"></a><a name="p8387183016507"></a>功能说明：VPC下可用子网的范围</p>
<p id="p6387133018508"><a name="p6387133018508"></a><a name="p6387133018508"></a>取值范围：</p>
<a name="ul538717301504"></a><a name="ul538717301504"></a><ul id="ul538717301504"><li>10.0.0.0/8~10.255.255.240/28</li><li>172.16.0.0/12 ~ 172.31.255.240/28</li><li>192.168.0.0/16 ~ 192.168.255.240/28</li></ul>
<p id="p63873303507"><a name="p63873303507"></a><a name="p63873303507"></a>不指定cidr时，默认值为“”</p>
<a name="ul138703025012"></a><a name="ul138703025012"></a><ul id="ul138703025012"><li>约束：必须是ipv4 cidr格式，例如:192.168.0.0/16</li></ul>
</td>
</tr>
<tr id="row4388143035016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p163879300500"><a name="p163879300500"></a><a name="p163879300500"></a>extend_cidrs</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13877308501"><a name="p13877308501"></a><a name="p13877308501"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1238853045014"><a name="p1238853045014"></a><a name="p1238853045014"></a>功能描述：VPC的扩展网段</p>
<p id="p1638883016506"><a name="p1638883016506"></a><a name="p1638883016506"></a>取值范围：</p>
<p id="p4388430175015"><a name="p4388430175015"></a><a name="p4388430175015"></a>约束：目前只支持ipv4</p>
</td>
</tr>
<tr id="row12388230135019"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1438883010509"><a name="p1438883010509"></a><a name="p1438883010509"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16388153017503"><a name="p16388153017503"></a><a name="p16388153017503"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9388183016507"><a name="p9388183016507"></a><a name="p9388183016507"></a>功能说明：VPC对应的状态</p>
<div class="p" id="p238893012508"><a name="p238893012508"></a><a name="p238893012508"></a>取值范围：<a name="ul3388153095011"></a><a name="ul3388153095011"></a><ul id="ul3388153095011"><li>PENDING：创建中</li><li>ACTIVE：创建成功</li></ul>
</div>
</td>
</tr>
<tr id="row1138843005018"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1638813012503"><a name="p1638813012503"></a><a name="p1638813012503"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1938812305507"><a name="p1938812305507"></a><a name="p1938812305507"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p163881330195018"><a name="p163881330195018"></a><a name="p163881330195018"></a>功能说明：VPC所属的项目ID</p>
</td>
</tr>
<tr id="row12388430115015"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1438815302507"><a name="p1438815302507"></a><a name="p1438815302507"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13388230165013"><a name="p13388230165013"></a><a name="p13388230165013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p338817309506"><a name="p338817309506"></a><a name="p338817309506"></a>功能说明：VPC所属的企业项目ID。</p>
<p id="p1438873035020"><a name="p1438873035020"></a><a name="p1438873035020"></a>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。</p>
</td>
</tr>
<tr id="row20388143035015"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p338813018502"><a name="p338813018502"></a><a name="p338813018502"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7388183019506"><a name="p7388183019506"></a><a name="p7388183019506"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p93881330155016"><a name="p93881330155016"></a><a name="p93881330155016"></a>功能说明：VPC创建时间</p>
<p id="p17388130125011"><a name="p17388130125011"></a><a name="p17388130125011"></a>取值范围：UTC时间格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row1538803012502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p238833016509"><a name="p238833016509"></a><a name="p238833016509"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p438883085013"><a name="p438883085013"></a><a name="p438883085013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1538863075017"><a name="p1538863075017"></a><a name="p1538863075017"></a>功能说明：VPC更新时间</p>
<p id="p123880307502"><a name="p123880307502"></a><a name="p123880307502"></a>取值范围：UTC时间格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row1838893085020"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p838817300506"><a name="p838817300506"></a><a name="p838817300506"></a>cloud_resources</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18388163035018"><a name="p18388163035018"></a><a name="p18388163035018"></a>Array of <a href="#zh-cn_topic_0267488960_response_CloudResource">CloudResource</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5388230105014"><a name="p5388230105014"></a><a name="p5388230105014"></a>功能说明：VPC关联资源类型和数量</p>
<p id="p33881530135015"><a name="p33881530135015"></a><a name="p33881530135015"></a>取值范围：目前只返回VPC关联的routetable和virsubnet</p>
</td>
</tr>
<tr id="row17388193012505"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p43881430105010"><a name="p43881430105010"></a><a name="p43881430105010"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11388153010500"><a name="p11388153010500"></a><a name="p11388153010500"></a>Array of <a href="#zh-cn_topic_0267488960_response_Tag">Tag</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1038812302501"><a name="p1038812302501"></a><a name="p1038812302501"></a>功能说明：VPC的标签信息，详情参见Tag对象</p>
<p id="p4388930195012"><a name="p4388930195012"></a><a name="p4388930195012"></a>取值范围：0-10个标签键值对</p>
</td>
</tr>
</tbody>
</table>

**表 6**  CloudResource

<a name="zh-cn_topic_0267488960_response_CloudResource"></a>
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

**表 7**  Tag

<a name="zh-cn_topic_0267488960_response_Tag"></a>
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

**状态码为 400 时:**

**表 8**  响应Body参数

<a name="table129531025185617"></a>
<table><thead align="left"><tr id="row10953925185614"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p5954182525618"><a name="p5954182525618"></a><a name="p5954182525618"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p09552025195613"><a name="p09552025195613"></a><a name="p09552025195613"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p695612515617"><a name="p695612515617"></a><a name="p695612515617"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row19532256562"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39571125175616"><a name="p39571125175616"></a><a name="p39571125175616"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p295822555619"><a name="p295822555619"></a><a name="p295822555619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p995818251566"><a name="p995818251566"></a><a name="p995818251566"></a>请求ID</p>
</td>
</tr>
<tr id="row1995312516564"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29591125165612"><a name="p29591125165612"></a><a name="p29591125165612"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p696072575615"><a name="p696072575615"></a><a name="p696072575615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p39613259569"><a name="p39613259569"></a><a name="p39613259569"></a>错误消息</p>
</td>
</tr>
<tr id="row119546254566"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3962182535618"><a name="p3962182535618"></a><a name="p3962182535618"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16962825125616"><a name="p16962825125616"></a><a name="p16962825125616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p159631825145612"><a name="p159631825145612"></a><a name="p159631825145612"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 401 时:**

**表 9**  响应Body参数

<a name="table199641625115616"></a>
<table><thead align="left"><tr id="row18965625155617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p09801825185616"><a name="p09801825185616"></a><a name="p09801825185616"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1998220253569"><a name="p1998220253569"></a><a name="p1998220253569"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p2983162545611"><a name="p2983162545611"></a><a name="p2983162545611"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row199661625195618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p159851259562"><a name="p159851259562"></a><a name="p159851259562"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1798632555614"><a name="p1798632555614"></a><a name="p1798632555614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1798742585620"><a name="p1798742585620"></a><a name="p1798742585620"></a>请求ID</p>
</td>
</tr>
<tr id="row179675256563"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p79871825195610"><a name="p79871825195610"></a><a name="p79871825195610"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14988192535615"><a name="p14988192535615"></a><a name="p14988192535615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p129891025105612"><a name="p129891025105612"></a><a name="p129891025105612"></a>错误消息</p>
</td>
</tr>
<tr id="row17967172525612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4989152514565"><a name="p4989152514565"></a><a name="p4989152514565"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1899019252564"><a name="p1899019252564"></a><a name="p1899019252564"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19901025185614"><a name="p19901025185614"></a><a name="p19901025185614"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 403 时:**

**表 10**  响应Body参数

<a name="table179903250566"></a>
<table><thead align="left"><tr id="row1299102516562"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p2993202545613"><a name="p2993202545613"></a><a name="p2993202545613"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1993152515564"><a name="p1993152515564"></a><a name="p1993152515564"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1399422513565"><a name="p1399422513565"></a><a name="p1399422513565"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1499142545615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p129941525135614"><a name="p129941525135614"></a><a name="p129941525135614"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19995152515616"><a name="p19995152515616"></a><a name="p19995152515616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p599572535615"><a name="p599572535615"></a><a name="p599572535615"></a>请求ID</p>
</td>
</tr>
<tr id="row09919255560"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p699612515563"><a name="p699612515563"></a><a name="p699612515563"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p29961925145614"><a name="p29961925145614"></a><a name="p29961925145614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1399702518565"><a name="p1399702518565"></a><a name="p1399702518565"></a>错误消息</p>
</td>
</tr>
<tr id="row89917257561"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29972252567"><a name="p29972252567"></a><a name="p29972252567"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p169981425165617"><a name="p169981425165617"></a><a name="p169981425165617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p159994257567"><a name="p159994257567"></a><a name="p159994257567"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 404 时:**

**表 11**  响应Body参数

<a name="table170192645617"></a>
<table><thead align="left"><tr id="row5014260565"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p151426155616"><a name="p151426155616"></a><a name="p151426155616"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1321426145613"><a name="p1321426145613"></a><a name="p1321426145613"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p162152645610"><a name="p162152645610"></a><a name="p162152645610"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row190102625618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15322615563"><a name="p15322615563"></a><a name="p15322615563"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13462635611"><a name="p13462635611"></a><a name="p13462635611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p114102612567"><a name="p114102612567"></a><a name="p114102612567"></a>请求ID</p>
</td>
</tr>
<tr id="row00122614567"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p651426115612"><a name="p651426115612"></a><a name="p651426115612"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14522675612"><a name="p14522675612"></a><a name="p14522675612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12582625612"><a name="p12582625612"></a><a name="p12582625612"></a>错误消息</p>
</td>
</tr>
<tr id="row7022615611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19614262565"><a name="p19614262565"></a><a name="p19614262565"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p36162655615"><a name="p36162655615"></a><a name="p36162655615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1071726195611"><a name="p1071726195611"></a><a name="p1071726195611"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 409 时:**

**表 12**  响应Body参数

<a name="table58112665618"></a>
<table><thead align="left"><tr id="row89526125612"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p12330102617567"><a name="p12330102617567"></a><a name="p12330102617567"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p143304269561"><a name="p143304269561"></a><a name="p143304269561"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p6330926125611"><a name="p6330926125611"></a><a name="p6330926125611"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row159102618564"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p733122625616"><a name="p733122625616"></a><a name="p733122625616"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p163311526125614"><a name="p163311526125614"></a><a name="p163311526125614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5331426175617"><a name="p5331426175617"></a><a name="p5331426175617"></a>请求ID</p>
</td>
</tr>
<tr id="row2913263564"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p533110266564"><a name="p533110266564"></a><a name="p533110266564"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6332426185616"><a name="p6332426185616"></a><a name="p6332426185616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p63323269565"><a name="p63323269565"></a><a name="p63323269565"></a>错误消息</p>
</td>
</tr>
<tr id="row1896267568"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1332026125619"><a name="p1332026125619"></a><a name="p1332026125619"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9332226155614"><a name="p9332226155614"></a><a name="p9332226155614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19332172610568"><a name="p19332172610568"></a><a name="p19332172610568"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 500 时:**

**表 13**  响应Body参数

<a name="table1215626145612"></a>
<table><thead align="left"><tr id="row3161326115617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p733372610563"><a name="p733372610563"></a><a name="p733372610563"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p8333172695611"><a name="p8333172695611"></a><a name="p8333172695611"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p183331826175612"><a name="p183331826175612"></a><a name="p183331826175612"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row3161226175615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1333312695615"><a name="p1333312695615"></a><a name="p1333312695615"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4334192619567"><a name="p4334192619567"></a><a name="p4334192619567"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p63341326125617"><a name="p63341326125617"></a><a name="p63341326125617"></a>请求ID</p>
</td>
</tr>
<tr id="row111692615620"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19334152615611"><a name="p19334152615611"></a><a name="p19334152615611"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p833432614566"><a name="p833432614566"></a><a name="p833432614566"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1433462617564"><a name="p1433462617564"></a><a name="p1433462617564"></a>错误消息</p>
</td>
</tr>
<tr id="row316182610563"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9334626145614"><a name="p9334626145614"></a><a name="p9334626145614"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p733412265566"><a name="p733412265566"></a><a name="p733412265566"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17334182685611"><a name="p17334182685611"></a><a name="p17334182685611"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

## 响应示例<a name="section14336326155620"></a>

**状态码为 200 时:**

OK

```
{
    "request_id": "84eb4f775d66dd916db121768ec55626", 
    "vpc": {
        "id": "0552091e-b83a-49dd-88a7-4a5c86fd9ec3", 
        "name": "vpc1", 
        "description": "test1", 
        "cidr": "192.168.0.0/16", 
        "extend_cidrs": [
            "23.8.0.0/16"
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

