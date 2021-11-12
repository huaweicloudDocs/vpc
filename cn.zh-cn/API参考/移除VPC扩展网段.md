# 移除VPC扩展网段<a name="vpc_apiv3_0008"></a>

## 功能介绍<a name="section13881741116"></a>

移除VPC扩展网段

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v3&api=RemoveVpcExtendCidr)中直接运行调试该接口。

## URI<a name="section1538920416117"></a>

PUT /v3/\{project\_id\}/vpc/vpcs/\{vpc\_id\}/remove-extend-cidr

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

## 请求参数<a name="section8442342016"></a>

**表 2**  请求Body参数

<a name="zh-cn_topic_0267488922_requestParameter"></a>
<table><thead align="left"><tr id="row3450140113"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p7451940110"><a name="p7451940110"></a><a name="p7451940110"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p64521441714"><a name="p64521441714"></a><a name="p64521441714"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p4452941718"><a name="p4452941718"></a><a name="p4452941718"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p1045314411"><a name="p1045314411"></a><a name="p1045314411"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1245015413117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1387542565613"><a name="p1387542565613"></a><a name="p1387542565613"></a>dry_run</p>
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
<tr id="row12450541318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p14458145111"><a name="p14458145111"></a><a name="p14458145111"></a>vpc</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p184593411116"><a name="p184593411116"></a><a name="p184593411116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p5459144719"><a name="p5459144719"></a><a name="p5459144719"></a><a href="#zh-cn_topic_0267488922_request_RemoveExtendCidrOption">RemoveExtendCidrOption</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p1946015412115"><a name="p1946015412115"></a><a name="p1946015412115"></a>移除VPC扩展网段请求体</p>
</td>
</tr>
</tbody>
</table>

**表 3**  RemoveExtendCidrOption

<a name="zh-cn_topic_0267488922_request_RemoveExtendCidrOption"></a>
<table><thead align="left"><tr id="row346174518"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p84631341416"><a name="p84631341416"></a><a name="p84631341416"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p1846454713"><a name="p1846454713"></a><a name="p1846454713"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.3"><p id="p1646414419111"><a name="p1646414419111"></a><a name="p1646414419111"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.5.1.4"><p id="p154641849114"><a name="p154641849114"></a><a name="p154641849114"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1546224917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p94651847114"><a name="p94651847114"></a><a name="p94651847114"></a>extend_cidrs</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p1465164613"><a name="p1465164613"></a><a name="p1465164613"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.3 "><p id="p114661414118"><a name="p114661414118"></a><a name="p114661414118"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.5.1.4 "><p id="p7690113420573"><a name="p7690113420573"></a><a name="p7690113420573"></a>功能说明：移除VPC扩展网段</p>
<p id="p172091344185713"><a name="p172091344185713"></a><a name="p172091344185713"></a>取值范围：该VPC已经存在的扩展网段</p>
<div class="p" id="p830244819574"><a name="p830244819574"></a><a name="p830244819574"></a>约束：<a name="ul1841745575716"></a><a name="ul1841745575716"></a><ul id="ul1841745575716"><li>移除扩展网段前，请先清理该VPC下对应cidr范围内的subnet</li><li>当前只支持一个一个移除</li></ul>
</div>
</td>
</tr>
</tbody>
</table>

## 请求示例<a name="section568215412112"></a>

移除单个VPC的扩展网段

```
PUT https://{Endpoint}/v3/{project_id}/vpc/vpcs/99d9d709-8478-4b46-9f3f-2206b1023fd3/remove-extend-cidr

{
    "vpc": {
        "extend_cidrs": [
            "23.8.0.0/16"
        ]
    }
}
```

## 响应参数<a name="section04675415110"></a>

**状态码为 200 时:**

**表 4**  响应Body参数

<a name="zh-cn_topic_0267488922_responseParameter"></a>
<table><thead align="left"><tr id="row16469114117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p847494312"><a name="p847494312"></a><a name="p847494312"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p1647513415120"><a name="p1647513415120"></a><a name="p1647513415120"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p9476144714"><a name="p9476144714"></a><a name="p9476144714"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row124691141613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19477445116"><a name="p19477445116"></a><a name="p19477445116"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10477141515"><a name="p10477141515"></a><a name="p10477141515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6478741115"><a name="p6478741115"></a><a name="p6478741115"></a>请求ID</p>
</td>
</tr>
<tr id="row12469194412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14478841418"><a name="p14478841418"></a><a name="p14478841418"></a>vpc</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5479164513"><a name="p5479164513"></a><a name="p5479164513"></a><a href="#zh-cn_topic_0267488960_response_Vpc">Vpc</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p124791848118"><a name="p124791848118"></a><a name="p124791848118"></a>移除VPC扩展网段</p>
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

<a name="table1527164818"></a>
<table><thead align="left"><tr id="row1752816413117"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p9529241118"><a name="p9529241118"></a><a name="p9529241118"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p352914414118"><a name="p352914414118"></a><a name="p352914414118"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1253012415120"><a name="p1253012415120"></a><a name="p1253012415120"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1852894116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p55321441715"><a name="p55321441715"></a><a name="p55321441715"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p155332419118"><a name="p155332419118"></a><a name="p155332419118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12536749119"><a name="p12536749119"></a><a name="p12536749119"></a>请求ID</p>
</td>
</tr>
<tr id="row85281647116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14538147114"><a name="p14538147114"></a><a name="p14538147114"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p155381044112"><a name="p155381044112"></a><a name="p155381044112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p195391141812"><a name="p195391141812"></a><a name="p195391141812"></a>错误消息</p>
</td>
</tr>
<tr id="row145282041916"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p145402417112"><a name="p145402417112"></a><a name="p145402417112"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p145401341312"><a name="p145401341312"></a><a name="p145401341312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p125403414118"><a name="p125403414118"></a><a name="p125403414118"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 401 时:**

**表 9**  响应Body参数

<a name="table25411412113"></a>
<table><thead align="left"><tr id="row6544641417"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1854554813"><a name="p1854554813"></a><a name="p1854554813"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p125461741918"><a name="p125461741918"></a><a name="p125461741918"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p16546441414"><a name="p16546441414"></a><a name="p16546441414"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row18544114118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p75478414115"><a name="p75478414115"></a><a name="p75478414115"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1954715416111"><a name="p1954715416111"></a><a name="p1954715416111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9548542018"><a name="p9548542018"></a><a name="p9548542018"></a>请求ID</p>
</td>
</tr>
<tr id="row15441241814"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1354816413112"><a name="p1354816413112"></a><a name="p1354816413112"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4549041415"><a name="p4549041415"></a><a name="p4549041415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p165503415110"><a name="p165503415110"></a><a name="p165503415110"></a>错误消息</p>
</td>
</tr>
<tr id="row5544174214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p05500417111"><a name="p05500417111"></a><a name="p05500417111"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p175511647113"><a name="p175511647113"></a><a name="p175511647113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p185521741019"><a name="p185521741019"></a><a name="p185521741019"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 403 时:**

**表 10**  响应Body参数

<a name="table55521141613"></a>
<table><thead align="left"><tr id="row355464119"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p20555940118"><a name="p20555940118"></a><a name="p20555940118"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p9555748116"><a name="p9555748116"></a><a name="p9555748116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1455644112"><a name="p1455644112"></a><a name="p1455644112"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1554541914"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p35561841617"><a name="p35561841617"></a><a name="p35561841617"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19557643119"><a name="p19557643119"></a><a name="p19557643119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p255734918"><a name="p255734918"></a><a name="p255734918"></a>请求ID</p>
</td>
</tr>
<tr id="row105541941215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p455711414112"><a name="p455711414112"></a><a name="p455711414112"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1055824619"><a name="p1055824619"></a><a name="p1055824619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p195581545113"><a name="p195581545113"></a><a name="p195581545113"></a>错误消息</p>
</td>
</tr>
<tr id="row8554134915"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p355914412120"><a name="p355914412120"></a><a name="p355914412120"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19559134918"><a name="p19559134918"></a><a name="p19559134918"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p35599415117"><a name="p35599415117"></a><a name="p35599415117"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 409 时:**

**表 11**  响应Body参数

<a name="table25601041117"></a>
<table><thead align="left"><tr id="row1556111419118"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p10562648119"><a name="p10562648119"></a><a name="p10562648119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p13562441717"><a name="p13562441717"></a><a name="p13562441717"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p856754616"><a name="p856754616"></a><a name="p856754616"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row145611241113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p856834212"><a name="p856834212"></a><a name="p856834212"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p145681141118"><a name="p145681141118"></a><a name="p145681141118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15681341219"><a name="p15681341219"></a><a name="p15681341219"></a>请求ID</p>
</td>
</tr>
<tr id="row45611448116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1656914420118"><a name="p1656914420118"></a><a name="p1656914420118"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p175692041917"><a name="p175692041917"></a><a name="p175692041917"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1857094517"><a name="p1857094517"></a><a name="p1857094517"></a>错误消息</p>
</td>
</tr>
<tr id="row1756113413112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p65701246114"><a name="p65701246114"></a><a name="p65701246114"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p75711242115"><a name="p75711242115"></a><a name="p75711242115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19571124012"><a name="p19571124012"></a><a name="p19571124012"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

**状态码为 500 时:**

**表 12**  响应Body参数

<a name="table12572147116"></a>
<table><thead align="left"><tr id="row05731842111"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1868113414119"><a name="p1868113414119"></a><a name="p1868113414119"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p18681741319"><a name="p18681741319"></a><a name="p18681741319"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p206814416118"><a name="p206814416118"></a><a name="p206814416118"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row1157354210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p06811413120"><a name="p06811413120"></a><a name="p06811413120"></a>request_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p136817413115"><a name="p136817413115"></a><a name="p136817413115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p168117416116"><a name="p168117416116"></a><a name="p168117416116"></a>请求ID</p>
</td>
</tr>
<tr id="row1757354119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19681164418"><a name="p19681164418"></a><a name="p19681164418"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1681741412"><a name="p1681741412"></a><a name="p1681741412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p66819414113"><a name="p66819414113"></a><a name="p66819414113"></a>错误消息</p>
</td>
</tr>
<tr id="row6573114118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p96813417117"><a name="p96813417117"></a><a name="p96813417117"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7682745119"><a name="p7682745119"></a><a name="p7682745119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3682449118"><a name="p3682449118"></a><a name="p3682449118"></a>错误码</p>
</td>
</tr>
</tbody>
</table>

## 响应示例<a name="section46821145116"></a>

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
        "extend_cidrs": [ ], 
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

