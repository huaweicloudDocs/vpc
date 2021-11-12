# 查询所有网络ACL策略<a name="vpc_firewall_0006"></a>

## 功能介绍<a name="section836818132340"></a>

查询提交请求的租户有权限操作的所有网络ACL策略信息。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=NeutronListFirewallPolicies)中直接运行调试该接口。

## URI<a name="section20177217132340"></a>

GET /v2.0/fwaas/firewall\_policies

分页查询样例：

```
GET https://{Endpoint}/v2.0/fwaas/firewall_policies?limit=2&marker=6b70e321-0c21-4b83-bb8a-a886d1414a5f&page_reverse=False
```

参数说明请参见[表1](#table2168229184411)

**表 1**  参数说明

<a name="table2168229184411"></a>
<table><thead align="left"><tr id="row62731129194416"><th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.2.5.1.1"><p id="p202731029194414"><a name="p202731029194414"></a><a name="p202731029194414"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.2"><p id="p827332934419"><a name="p827332934419"></a><a name="p827332934419"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="27.27272727272727%" id="mcps1.2.5.1.3"><p id="p3273829124411"><a name="p3273829124411"></a><a name="p3273829124411"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.36363636363636%" id="mcps1.2.5.1.4"><p id="p18273529184418"><a name="p18273529184418"></a><a name="p18273529184418"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2027311294446"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p227317292447"><a name="p227317292447"></a><a name="p227317292447"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p1273192914419"><a name="p1273192914419"></a><a name="p1273192914419"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p192737290449"><a name="p192737290449"></a><a name="p192737290449"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p172735292445"><a name="p172735292445"></a><a name="p172735292445"></a>按照网络ACL策略对应的ID过滤查询</p>
</td>
</tr>
<tr id="row1327314298444"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p18273102911445"><a name="p18273102911445"></a><a name="p18273102911445"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p1327342914412"><a name="p1327342914412"></a><a name="p1327342914412"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p1273112954414"><a name="p1273112954414"></a><a name="p1273112954414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p1627318299444"><a name="p1627318299444"></a><a name="p1627318299444"></a>按照网络ACL策略的名称过滤查询</p>
</td>
</tr>
<tr id="row227382915449"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1627342919446"><a name="p1627342919446"></a><a name="p1627342919446"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p02741429174411"><a name="p02741429174411"></a><a name="p02741429174411"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p1727442911446"><a name="p1727442911446"></a><a name="p1727442911446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p16274429204415"><a name="p16274429204415"></a><a name="p16274429204415"></a>按照网络ACL策略的描述过滤查询</p>
</td>
</tr>
<tr id="row22741329104419"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p52741929134414"><a name="p52741929134414"></a><a name="p52741929134414"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p1227415292446"><a name="p1227415292446"></a><a name="p1227415292446"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p18274429154412"><a name="p18274429154412"></a><a name="p18274429154412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p1227413297440"><a name="p1227413297440"></a><a name="p1227413297440"></a>按照网络ACL策略所属的项目ID过滤查询</p>
</td>
</tr>
<tr id="row192740294443"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p192741229104418"><a name="p192741229104418"></a><a name="p192741229104418"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p152741298443"><a name="p152741298443"></a><a name="p152741298443"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p13274229194419"><a name="p13274229194419"></a><a name="p13274229194419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p28526205175853"><a name="p28526205175853"></a><a name="p28526205175853"></a>分页查询的起始资源ID，表示从指定资源的下一条记录开始查询。</p>
<p id="p538818488578"><a name="p538818488578"></a><a name="p538818488578"></a>marker需要和limit配合使用：</p>
<a name="ul12704811125810"></a><a name="ul12704811125810"></a><ul id="ul12704811125810"><li>若不传入marker和limit参数，查询结果返回全部资源记录。</li><li>若不传入marker参数，limit为10，查询结果返回第1~10条资源记录。</li><li>若marker为第10条记录的资源ID，limit为10，查询结果返回第11~20条资源记录。</li><li>若marker为第10条记录的资源ID，不传入limit参数，查询结果返回第11条及之后的所有资源记录。</li></ul>
</td>
</tr>
<tr id="row112741929134413"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p727492918445"><a name="p727492918445"></a><a name="p727492918445"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p72746298445"><a name="p72746298445"></a><a name="p72746298445"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.27272727272727%" headers="mcps1.2.5.1.3 "><p id="p327413298441"><a name="p327413298441"></a><a name="p327413298441"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="36.36363636363636%" headers="mcps1.2.5.1.4 "><p id="p2017153116589"><a name="p2017153116589"></a><a name="p2017153116589"></a>分页查询每页返回的记录个数，取值范围为0~intmax。</p>
<p id="p125192338584"><a name="p125192338584"></a><a name="p125192338584"></a>limit需要和marker配合使用，详细规则请见marker的参数说明。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section49464339132340"></a>

无。

## 响应消息<a name="section60203718132340"></a>

**表 2**  响应参数

<a name="table9250393132340"></a>
<table><thead align="left"><tr id="row50269734132340"><th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.1"><p id="p65065932132340"><a name="p65065932132340"></a><a name="p65065932132340"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.78%" id="mcps1.2.4.1.2"><p id="p19160762132340"><a name="p19160762132340"></a><a name="p19160762132340"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.89%" id="mcps1.2.4.1.3"><p id="p8860905132340"><a name="p8860905132340"></a><a name="p8860905132340"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row66469484132340"><td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.1 "><p id="p23038389132340"><a name="p23038389132340"></a><a name="p23038389132340"></a>firewall_policies</p>
</td>
<td class="cellrowborder" valign="top" width="17.78%" headers="mcps1.2.4.1.2 "><p id="p128475406537"><a name="p128475406537"></a><a name="p128475406537"></a>Array of <a href="#table17002720121127">firewall Policy</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="58.89%" headers="mcps1.2.4.1.3 "><p id="p50197883132340"><a name="p50197883132340"></a><a name="p50197883132340"></a>firewall policy对象。请参见<a href="#table17002720121127">表3</a>。</p>
</td>
</tr>
<tr id="row14916144011474"><td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.1 "><p id="p12902184724718"><a name="p12902184724718"></a><a name="p12902184724718"></a>firewall_policies_links</p>
</td>
<td class="cellrowborder" valign="top" width="17.78%" headers="mcps1.2.4.1.2 "><p id="p0902164713477"><a name="p0902164713477"></a><a name="p0902164713477"></a>Array of <a href="#table25150247450">firewall_policies_link</a> object</p>
</td>
<td class="cellrowborder" valign="top" width="58.89%" headers="mcps1.2.4.1.3 "><p id="p149028478475"><a name="p149028478475"></a><a name="p149028478475"></a>firewall_policies_link对象。请参见<a href="#table25150247450">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  firewall\_Policy对象

<a name="table17002720121127"></a>
<table><thead align="left"><tr id="row16929792121127"><th class="cellrowborder" valign="top" width="32.083208320832085%" id="mcps1.2.4.1.1"><p id="p18873879121127"><a name="p18873879121127"></a><a name="p18873879121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="22.632263226322635%" id="mcps1.2.4.1.2"><p id="p12638309121127"><a name="p12638309121127"></a><a name="p12638309121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="45.28452845284529%" id="mcps1.2.4.1.3"><p id="p61199938121127"><a name="p61199938121127"></a><a name="p61199938121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46402691121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p11805115121127"><a name="p11805115121127"></a><a name="p11805115121127"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p13006089121127"><a name="p13006089121127"></a><a name="p13006089121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p13152683121127"><a name="p13152683121127"></a><a name="p13152683121127"></a><span id="text381715763919"><a name="text381715763919"></a><a name="text381715763919"></a>网络ACL</span><span id="text28171774399"><a name="text28171774399"></a><a name="text28171774399"></a></span>策略uuid标识。</p>
</td>
</tr>
<tr id="row9858171121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p49865700121127"><a name="p49865700121127"></a><a name="p49865700121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p6225460121127"><a name="p6225460121127"></a><a name="p6225460121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p40337147121127"><a name="p40337147121127"></a><a name="p40337147121127"></a><span id="text46551455397"><a name="text46551455397"></a><a name="text46551455397"></a>网络ACL</span><span id="text15655545193910"><a name="text15655545193910"></a><a name="text15655545193910"></a></span>策略名称。</p>
</td>
</tr>
<tr id="row61803802121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p39621949121127"><a name="p39621949121127"></a><a name="p39621949121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p66053143121127"><a name="p66053143121127"></a><a name="p66053143121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p15357220121127"><a name="p15357220121127"></a><a name="p15357220121127"></a><span id="text32111655113917"><a name="text32111655113917"></a><a name="text32111655113917"></a>网络ACL</span><span id="text19211195514394"><a name="text19211195514394"></a><a name="text19211195514394"></a></span>策略描述。</p>
</td>
</tr>
<tr id="row57644277121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p9761241121127"><a name="p9761241121127"></a><a name="p9761241121127"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p20138053121127"><a name="p20138053121127"></a><a name="p20138053121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row33369184121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p16940942121127"><a name="p16940942121127"></a><a name="p16940942121127"></a>firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p122792241376"><a name="p122792241376"></a><a name="p122792241376"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p53455884121127"><a name="p53455884121127"></a><a name="p53455884121127"></a>策略引用的<span id="text144397419406"><a name="text144397419406"></a><a name="text144397419406"></a>网络ACL</span><span id="text1744010454015"><a name="text1744010454015"></a><a name="text1744010454015"></a></span>规则链。</p>
</td>
</tr>
<tr id="row717167121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p30704110121127"><a name="p30704110121127"></a><a name="p30704110121127"></a>audited</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p10804884121127"><a name="p10804884121127"></a><a name="p10804884121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p3925300121127"><a name="p3925300121127"></a><a name="p3925300121127"></a>审计标记。</p>
</td>
</tr>
<tr id="row40905717121127"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p16821838121127"><a name="p16821838121127"></a><a name="p16821838121127"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p49691806121127"><a name="p49691806121127"></a><a name="p49691806121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p31604739121127"><a name="p31604739121127"></a><a name="p31604739121127"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row109594223354"><td class="cellrowborder" valign="top" width="32.083208320832085%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.632263226322635%" headers="mcps1.2.4.1.2 "><p id="p17700201411911"><a name="p17700201411911"></a><a name="p17700201411911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="45.28452845284529%" headers="mcps1.2.4.1.3 "><p id="p763154142816"><a name="p763154142816"></a><a name="p763154142816"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  firewall\_policies\_link对象

<a name="table25150247450"></a>
<table><thead align="left"><tr id="row10561424184513"><th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.1"><p id="p15562102474514"><a name="p15562102474514"></a><a name="p15562102474514"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.2"><p id="p656212464511"><a name="p656212464511"></a><a name="p656212464511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="71.72%" id="mcps1.2.4.1.3"><p id="p856220242456"><a name="p856220242456"></a><a name="p856220242456"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3562132464511"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p13562224194510"><a name="p13562224194510"></a><a name="p13562224194510"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p556214245453"><a name="p556214245453"></a><a name="p556214245453"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p145623247454"><a name="p145623247454"></a><a name="p145623247454"></a>API链接</p>
</td>
</tr>
<tr id="row656292454519"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p1756252484511"><a name="p1756252484511"></a><a name="p1756252484511"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p056210247459"><a name="p056210247459"></a><a name="p056210247459"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p75621724194516"><a name="p75621724194516"></a><a name="p75621724194516"></a>API链接与该API版本的关系</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section35216218132340"></a>

请求样例

```
GET https://{Endpoint}/v2.0/fwaas/firewall_policies
```

响应样例

```
{
    "firewall_policies": [
        {
            "description": "", 
            "firewall_rules": [
                "6c6803e0-ca8c-4aa9-afb3-4f89275b6c32"
            ], 
            "tenant_id": "23c8a121505047b6869edf39f3062712", 
            "public": false, 
            "id": "6b70e321-0c21-4b83-bb8a-a886d1414a5f", 
            "audited": false, 
            "name": "fwp1",
            "project_id": "23c8a121505047b6869edf39f3062712"
        }, 
        {
            "description": "", 
            "firewall_rules": [
                "6c6803e0-ca8c-4aa9-afb3-4f89275b6c32"
            ], 
            "tenant_id": "23c8a121505047b6869edf39f3062712", 
            "public": false, 
            "id": "fce92002-5a15-465d-aaca-9b44453bb738", 
            "audited": false, 
            "name": "fwp2",
            "project_id": "23c8a121505047b6869edf39f3062712"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

