# 查询端口列表<a name="vpc_port02_0001"></a>

## 功能介绍<a name="zh-cn_topic_0062207386_section66569185"></a>

查询提交请求的租户的所有端口，单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="zh-cn_topic_0062207386_section62251757"></a>

GET /v2.0/ports

样例：

```
GET https://{Endpoint}/v2.0/ports?id={port_id}&name={port_name}&admin_state_up={is_admin_status_up}&network_id={network_id}&mac_address={port_mac}&device_id={port_device_id}&device_owner={device_owner}&tenant_id={tenant_id}&status={port_status}&fixed_ips=ip_address={ip_address}&fixed_ips=subnet_id={subnet_id}&dns_name={dns_name}
```

分页查询样例：

```
GET https://{Endpoint}/v2.0/ports?limit=2&marker=791870bd-36a7-4d9b-b015-a78e9b06af08&page_reverse=False
```

参数说明请参见[表1](#table534412611487)。

**表 1**  参数说明

<a name="table534412611487"></a>
<table><thead align="left"><tr id="row448492674817"><th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.2.5.1.1"><p id="p24841926154819"><a name="p24841926154819"></a><a name="p24841926154819"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.2"><p id="p1648432615489"><a name="p1648432615489"></a><a name="p1648432615489"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.2.5.1.3"><p id="p144841026144810"><a name="p144841026144810"></a><a name="p144841026144810"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.5.1.4"><p id="p2484112664814"><a name="p2484112664814"></a><a name="p2484112664814"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row948482644816"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p18484826154812"><a name="p18484826154812"></a><a name="p18484826154812"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p1848410267488"><a name="p1848410267488"></a><a name="p1848410267488"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p104842262481"><a name="p104842262481"></a><a name="p104842262481"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p94841626104816"><a name="p94841626104816"></a><a name="p94841626104816"></a>按照端口的ID过滤查询</p>
</td>
</tr>
<tr id="row8484226114819"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p7484202694817"><a name="p7484202694817"></a><a name="p7484202694817"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p9484162664814"><a name="p9484162664814"></a><a name="p9484162664814"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p1548412269482"><a name="p1548412269482"></a><a name="p1548412269482"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p8485172674817"><a name="p8485172674817"></a><a name="p8485172674817"></a>按照端口的名称过滤查询</p>
</td>
</tr>
<tr id="row1448518262483"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p124851326114815"><a name="p124851326114815"></a><a name="p124851326114815"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p18485112614488"><a name="p18485112614488"></a><a name="p18485112614488"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p13485162694818"><a name="p13485162694818"></a><a name="p13485162694818"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p132122181612"><a name="p132122181612"></a><a name="p132122181612"></a>按照端口的管理状态过滤查询</p>
<p id="p9485122611486"><a name="p9485122611486"></a><a name="p9485122611486"></a>取值范围：true or false</p>
</td>
</tr>
<tr id="row848522612484"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1448516264489"><a name="p1448516264489"></a><a name="p1448516264489"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p154852026124815"><a name="p154852026124815"></a><a name="p154852026124815"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p1048592684818"><a name="p1048592684818"></a><a name="p1048592684818"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p10485132664815"><a name="p10485132664815"></a><a name="p10485132664815"></a>按照端口所属的网络ID过滤查询</p>
</td>
</tr>
<tr id="row1948562624813"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p154851626134817"><a name="p154851626134817"></a><a name="p154851626134817"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p5485726104812"><a name="p5485726104812"></a><a name="p5485726104812"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p11485132644813"><a name="p11485132644813"></a><a name="p11485132644813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p114851326144819"><a name="p114851326144819"></a><a name="p114851326144819"></a>按照端口的mac地址过滤查询</p>
</td>
</tr>
<tr id="row1348552617486"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p4485926194812"><a name="p4485926194812"></a><a name="p4485926194812"></a>device_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p448522624814"><a name="p448522624814"></a><a name="p448522624814"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p648511262487"><a name="p648511262487"></a><a name="p648511262487"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p1548518263489"><a name="p1548518263489"></a><a name="p1548518263489"></a>按照端口的设备ID过滤查询</p>
</td>
</tr>
<tr id="row16485122614487"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p13485192616487"><a name="p13485192616487"></a><a name="p13485192616487"></a>device_owner</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p3485152619489"><a name="p3485152619489"></a><a name="p3485152619489"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p8485102620484"><a name="p8485102620484"></a><a name="p8485102620484"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p64851126204810"><a name="p64851126204810"></a><a name="p64851126204810"></a>按照端口的设备所属过滤查询</p>
</td>
</tr>
<tr id="row0485142618484"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p15485172619482"><a name="p15485172619482"></a><a name="p15485172619482"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p5485172612482"><a name="p5485172612482"></a><a name="p5485172612482"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p2048519261484"><a name="p2048519261484"></a><a name="p2048519261484"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p47831820460"><a name="p47831820460"></a><a name="p47831820460"></a>按照端口状态过滤查询</p>
<p id="p348516264489"><a name="p348516264489"></a><a name="p348516264489"></a>取值范围：ACTIVE、BUILD、DOWN</p>
</td>
</tr>
<tr id="row154851626164815"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p10485926164819"><a name="p10485926164819"></a><a name="p10485926164819"></a>fixed_ips</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p15485826194811"><a name="p15485826194811"></a><a name="p15485826194811"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p11485026164810"><a name="p11485026164810"></a><a name="p11485026164810"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p9486526174813"><a name="p9486526174813"></a><a name="p9486526174813"></a>按照端口的IP地址过滤查询，fixed_ips=ip_address或者fixed_ips=subnet_id过滤查询</p>
</td>
</tr>
<tr id="row84861626204816"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1448672614484"><a name="p1448672614484"></a><a name="p1448672614484"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p13486626114819"><a name="p13486626114819"></a><a name="p13486626114819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p194861626124817"><a name="p194861626124817"></a><a name="p194861626124817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p114861226174812"><a name="p114861226174812"></a><a name="p114861226174812"></a>按照端口所属的项目ID过滤查询</p>
</td>
</tr>
<tr id="row748682684814"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p1148672694815"><a name="p1148672694815"></a><a name="p1148672694815"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p154862263482"><a name="p154862263482"></a><a name="p154862263482"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p11486926134819"><a name="p11486926134819"></a><a name="p11486926134819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p948692684817"><a name="p948692684817"></a><a name="p948692684817"></a>分页查询起始的资源ID，为空时为查询第一页</p>
</td>
</tr>
<tr id="row1048632694819"><td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.2.5.1.1 "><p id="p164861626154814"><a name="p164861626154814"></a><a name="p164861626154814"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.2 "><p id="p1948619268488"><a name="p1948619268488"></a><a name="p1948619268488"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.3 "><p id="p2486142612485"><a name="p2486142612485"></a><a name="p2486142612485"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><p id="p01471215164915"><a name="p01471215164915"></a><a name="p01471215164915"></a>每页返回的个数</p>
<p id="p24869261488"><a name="p24869261488"></a><a name="p24869261488"></a>取值范围：0~intmax</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0062207386_section15938858"></a>

无

## 响应参数<a name="zh-cn_topic_0062207386_section9232000"></a>

**表 2**  响应参数

<a name="zh-cn_topic_0062207386_table48620262"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207386_row18332862"><th class="cellrowborder" valign="top" width="22.32%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207386_p8566882"><a name="zh-cn_topic_0062207386_p8566882"></a><a name="zh-cn_topic_0062207386_p8566882"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="24.67%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207386_p22828842"><a name="zh-cn_topic_0062207386_p22828842"></a><a name="zh-cn_topic_0062207386_p22828842"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.010000000000005%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207386_p60161096"><a name="zh-cn_topic_0062207386_p60161096"></a><a name="zh-cn_topic_0062207386_p60161096"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207386_row41210606"><td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207386_p49724760"><a name="zh-cn_topic_0062207386_p49724760"></a><a name="zh-cn_topic_0062207386_p49724760"></a>ports</p>
</td>
<td class="cellrowborder" valign="top" width="24.67%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207386_p1173742"><a name="zh-cn_topic_0062207386_p1173742"></a><a name="zh-cn_topic_0062207386_p1173742"></a>Array of <a href="#table15919752145624">port</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="53.010000000000005%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207386_p50516929"><a name="zh-cn_topic_0062207386_p50516929"></a><a name="zh-cn_topic_0062207386_p50516929"></a>port对象列表，参见<a href="#table15919752145624">表3</a>。</p>
</td>
</tr>
<tr id="row10838426109"><td class="cellrowborder" valign="top" width="22.32%" headers="mcps1.2.4.1.1 "><p id="p97911291701"><a name="p97911291701"></a><a name="p97911291701"></a>ports_links</p>
</td>
<td class="cellrowborder" valign="top" width="24.67%" headers="mcps1.2.4.1.2 "><p id="p779329805"><a name="p779329805"></a><a name="p779329805"></a>Array of <a href="#table109221759807">ports_link</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="53.010000000000005%" headers="mcps1.2.4.1.3 "><p id="p97972919015"><a name="p97972919015"></a><a name="p97972919015"></a>分页信息，参见<a href="#table109221759807">表8</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  port对象

<a name="table15919752145624"></a>
<table><thead align="left"><tr id="row28529169145624"><th class="cellrowborder" valign="top" width="28.499999999999996%" id="mcps1.2.4.1.1"><p id="p42540009145658"><a name="p42540009145658"></a><a name="p42540009145658"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="28.749999999999996%" id="mcps1.2.4.1.2"><p id="p23188741145658"><a name="p23188741145658"></a><a name="p23188741145658"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.75%" id="mcps1.2.4.1.3"><p id="p13444574145658"><a name="p13444574145658"></a><a name="p13444574145658"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13166425145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p28807446145658"><a name="p28807446145658"></a><a name="p28807446145658"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p51701793145658"><a name="p51701793145658"></a><a name="p51701793145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p5183528145658"><a name="p5183528145658"></a><a name="p5183528145658"></a>端口的ID，最大长度不超过255</p>
<p id="p189962619371"><a name="p189962619371"></a><a name="p189962619371"></a>【使用说明】在查询端口列表时非必选</p>
</td>
</tr>
<tr id="row1387566145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p20696121145658"><a name="p20696121145658"></a><a name="p20696121145658"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p65773124145658"><a name="p65773124145658"></a><a name="p65773124145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p10771861145658"><a name="p10771861145658"></a><a name="p10771861145658"></a>端口的名称</p>
</td>
</tr>
<tr id="row36437767145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p949776145658"><a name="p949776145658"></a><a name="p949776145658"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p9822997145658"><a name="p9822997145658"></a><a name="p9822997145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p36061910145658"><a name="p36061910145658"></a><a name="p36061910145658"></a>所属网络的ID</p>
</td>
</tr>
<tr id="row41410455145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p49567182145658"><a name="p49567182145658"></a><a name="p49567182145658"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p55518807145658"><a name="p55518807145658"></a><a name="p55518807145658"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p26909682145658"><a name="p26909682145658"></a><a name="p26909682145658"></a>管理状态</p>
<p id="p40860550145658"><a name="p40860550145658"></a><a name="p40860550145658"></a>【使用说明】只支持true</p>
</td>
</tr>
<tr id="row11261085145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p58114882145658"><a name="p58114882145658"></a><a name="p58114882145658"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p9685031145658"><a name="p9685031145658"></a><a name="p9685031145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p8831008145658"><a name="p8831008145658"></a><a name="p8831008145658"></a>端口MAC地址，例如："mac_address": "fa:16:3e:9e:ff:55"</p>
<p id="p12370211145658"><a name="p12370211145658"></a><a name="p12370211145658"></a>【使用说明】只支持系统动态分配，不支持指定</p>
</td>
</tr>
<tr id="row59425565145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p25296431145658"><a name="p25296431145658"></a><a name="p25296431145658"></a>fixed_ips</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p35745048145658"><a name="p35745048145658"></a><a name="p35745048145658"></a>Array of <a href="#table4290920914597">fixed_ip</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p48560910145658"><a name="p48560910145658"></a><a name="p48560910145658"></a>端口IP，参见<a href="#table4290920914597">表4</a>。例如："fixed_ips": [{"subnet_id": "4dc70db6-cb7f-4200-9790-a6a910776bba", "ip_address": "192.169.25.79"}]</p>
</td>
</tr>
<tr id="row52336547145624"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p42357933145658"><a name="p42357933145658"></a><a name="p42357933145658"></a>device_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p8440512145658"><a name="p8440512145658"></a><a name="p8440512145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p23990357145658"><a name="p23990357145658"></a><a name="p23990357145658"></a>设备ID</p>
<p id="p14586626145658"><a name="p14586626145658"></a><a name="p14586626145658"></a>【使用说明】不支持设置和更新，由系统自动维护，该字段非空的端口不允许删除</p>
</td>
</tr>
<tr id="row8304195145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p30450002145658"><a name="p30450002145658"></a><a name="p30450002145658"></a>device_owner</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p50531130145658"><a name="p50531130145658"></a><a name="p50531130145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p60282892145658"><a name="p60282892145658"></a><a name="p60282892145658"></a>设备所属（DHCP/Router/ Nova等）</p>
<p id="p2837225125711"><a name="p2837225125711"></a><a name="p2837225125711"></a>【使用说明】不支持更新，只允许用户在创建虚拟IP端口时，为虚拟IP端口设置device_owner为neutron:VIP_PORT，当端口的该字段不为空时，仅支持该字段为neutron:VIP_PORT时的端口删除。</p>
<p id="p1458812975819"><a name="p1458812975819"></a><a name="p1458812975819"></a>该字段非空的端口不允许删除。</p>
</td>
</tr>
<tr id="row47218120145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p43524921145658"><a name="p43524921145658"></a><a name="p43524921145658"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p35857692145658"><a name="p35857692145658"></a><a name="p35857692145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row925022145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p12676379145658"><a name="p12676379145658"></a><a name="p12676379145658"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p20153784145658"><a name="p20153784145658"></a><a name="p20153784145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p12312282145658"><a name="p12312282145658"></a><a name="p12312282145658"></a>端口状态，可以为ACTIVE，BUILD，DOWN；</p>
<p id="p43701677145658"><a name="p43701677145658"></a><a name="p43701677145658"></a>【使用说明】Hana硬直通虚拟机端口状态总为DOWN</p>
</td>
</tr>
<tr id="row36940776145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p48921078145658"><a name="p48921078145658"></a><a name="p48921078145658"></a>security_groups</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p646712486358"><a name="p646712486358"></a><a name="p646712486358"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p4527282145658"><a name="p4527282145658"></a><a name="p4527282145658"></a>扩展属性：安全组的UUID,例如："security_groups": ["a0608cbf-d047-4f54-8b28-cd7b59853fff"]</p>
<p id="p103001912487"><a name="p103001912487"></a><a name="p103001912487"></a>【使用说明】不支持更新为空。</p>
</td>
</tr>
<tr id="row17626705145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p41382197145658"><a name="p41382197145658"></a><a name="p41382197145658"></a>allowed_address_pairs</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p13529152643712"><a name="p13529152643712"></a><a name="p13529152643712"></a>Array of <a href="#zh-cn_topic_0062207355_table57914257">allow_address_pair</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p30975735145658"><a name="p30975735145658"></a><a name="p30975735145658"></a>扩展属性：IP/Mac对列表，allow_address_pair参见<a href="#zh-cn_topic_0062207355_table57914257">表5</a></p>
<p id="p7136530194312"><a name="p7136530194312"></a><a name="p7136530194312"></a>【使用说明】</p>
<a name="ul18386852174311"></a><a name="ul18386852174311"></a><ul id="ul18386852174311"><li>IP地址不允许为 “0.0.0.0”</li><li>如果allowed_address_pairs配置地址池较大的CIDR（掩码小于24位），建议为该port配置一个单独的安全组</li><li>硬件SDN环境不支持ip_address属性配置为CIDR格式</li><li>为虚拟IP配置后端ECS场景，allowed_address_pairs中配置的IP地址，必须为ECS网卡已有的IP地址，否则可能会导致虚拟IP通信异常。</li></ul>
</td>
</tr>
<tr id="row938573145630"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p34089655145658"><a name="p34089655145658"></a><a name="p34089655145658"></a>extra_dhcp_opts</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p440115378365"><a name="p440115378365"></a><a name="p440115378365"></a>Array of <a href="#table5056075615524">extra_dhcp_opt</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p45787521145658"><a name="p45787521145658"></a><a name="p45787521145658"></a>扩展属性：DHCP的扩展Option，参见<a href="#table5056075615524">表6</a></p>
</td>
</tr>
<tr id="row46629855145636"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p62371645145658"><a name="p62371645145658"></a><a name="p62371645145658"></a>binding:vif_details</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p18938488145658"><a name="p18938488145658"></a><a name="p18938488145658"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p62312767145658"><a name="p62312767145658"></a><a name="p62312767145658"></a>vif的详细信息， "ovs_hybrid_plug": 是否为ovs/bridge混合模式</p>
</td>
</tr>
<tr id="row35771758145636"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p7522524145658"><a name="p7522524145658"></a><a name="p7522524145658"></a>binding:profile</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p5344685145658"><a name="p5344685145658"></a><a name="p5344685145658"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p4278449145658"><a name="p4278449145658"></a><a name="p4278449145658"></a>扩展属性：提供用户设置自定义信息</p>
<p id="p38506045145658"><a name="p38506045145658"></a><a name="p38506045145658"></a>【使用说明】</p>
<a name="ul11010089145658"></a><a name="ul11010089145658"></a><ul id="ul11010089145658"><li>internal_elb字段，布尔类型，普通租户可见。只有在创建内网ELB的虚拟IP的网卡时设置为true。普通租户没有权限更改该字段，由系统维护。<p id="p041674418210"><a name="p041674418210"></a><a name="p041674418210"></a>举例：</p>
<p id="p1774284092111"><a name="p1774284092111"></a><a name="p1774284092111"></a>{"internal_elb": true}</p>
</li><li>disable_security_groups字段，布尔类型，普通租户可见。默认为false高性能通信场景下，允许指定为true普通租户可见。仅支持创建port和读取时指定。当前仅支持指定为true，不支持指定为false<p id="p19402030145658"><a name="p19402030145658"></a><a name="p19402030145658"></a>举例：</p>
<p id="p40400544145658"><a name="p40400544145658"></a><a name="p40400544145658"></a>{"disable_security_groups"：true }，</p>
<p id="p28060583145658"><a name="p28060583145658"></a><a name="p28060583145658"></a>当前仅支持指定为true，不支持指定为false，指定为true时，FWaaS功能不生效。</p>
</li></ul>
<a name="ul51218659145658"></a><a name="ul51218659145658"></a>
</td>
</tr>
<tr id="row63233200145636"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p4700493145658"><a name="p4700493145658"></a><a name="p4700493145658"></a>binding:vnic_type</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p45195649145658"><a name="p45195649145658"></a><a name="p45195649145658"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p42146344145658"><a name="p42146344145658"></a><a name="p42146344145658"></a>绑定的vNIC类型</p>
<p id="p43772780145658"><a name="p43772780145658"></a><a name="p43772780145658"></a>normal: 软交换</p>
</td>
</tr>
<tr id="row37613242198"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p20178562198"><a name="p20178562198"></a><a name="p20178562198"></a>port_security_enabled</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p532005162198"><a name="p532005162198"></a><a name="p532005162198"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p184376702198"><a name="p184376702198"></a><a name="p184376702198"></a>端口安全使能标记，如果不使能则安全组和dhcp防欺骗不生效</p>
</td>
</tr>
<tr id="row167271926144411"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p117281926144417"><a name="p117281926144417"></a><a name="p117281926144417"></a>dns_assignment</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534165_p737862619493"><a name="zh-cn_topic_0201534165_p737862619493"></a><a name="zh-cn_topic_0201534165_p737862619493"></a>Array of <a href="#table1960316535179">dns_assignment</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p1472919269447"><a name="p1472919269447"></a><a name="p1472919269447"></a>扩展属性：主网卡默认内网域名信息</p>
<p id="p1834325274510"><a name="p1834325274510"></a><a name="p1834325274510"></a>【使用说明】不支持设置和更新，由系统自动维护</p>
<a name="ul1766216288464"></a><a name="ul1766216288464"></a><ul id="ul1766216288464"><li>hostname：与端口dns_name一致</li><li>ip_address：端口ipv4私有地址</li><li>fqdn：为端口创建默认内网fqdn</li></ul>
</td>
</tr>
<tr id="row119851851490"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p39859518498"><a name="p39859518498"></a><a name="p39859518498"></a>dns_name</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p139852519498"><a name="p139852519498"></a><a name="p139852519498"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p098555164915"><a name="p098555164915"></a><a name="p098555164915"></a>扩展属性：主网卡默认内网DNS名称</p>
<p id="p11538191913508"><a name="p11538191913508"></a><a name="p11538191913508"></a>【使用说明】不支持设置和更新，由系统自动维护,访问该默认内网域名前，请确保子网使用当前系统提供的DNS</p>
</td>
</tr>
<tr id="row8784124710810"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p870051413911"><a name="p870051413911"></a><a name="p870051413911"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p759775317217"><a name="p759775317217"></a><a name="p759775317217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p1675142052312"><a name="p1675142052312"></a><a name="p1675142052312"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
<tr id="row19797526919"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p89991542406"><a name="p89991542406"></a><a name="p89991542406"></a>资源创建时间，UTC时间</p>
<p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>格式yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row124097610917"><td class="cellrowborder" valign="top" width="28.499999999999996%" headers="mcps1.2.4.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="28.749999999999996%" headers="mcps1.2.4.1.2 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.75%" headers="mcps1.2.4.1.3 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间，UTC时间</p>
<p id="p65980291419"><a name="p65980291419"></a><a name="p65980291419"></a>格式yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

**表 4**  fixed\_ip对象

<a name="table4290920914597"></a>
<table><thead align="left"><tr id="row3523499914597"><th class="cellrowborder" valign="top" width="25.95259525952595%" id="mcps1.2.4.1.1"><p id="p6174509115118"><a name="p6174509115118"></a><a name="p6174509115118"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="25.95259525952595%" id="mcps1.2.4.1.2"><p id="p3529643715118"><a name="p3529643715118"></a><a name="p3529643715118"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.09480948094809%" id="mcps1.2.4.1.3"><p id="p2048854115118"><a name="p2048854115118"></a><a name="p2048854115118"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2319879914597"><td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.1 "><p id="p626497215118"><a name="p626497215118"></a><a name="p626497215118"></a>subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.2 "><p id="p3770069415118"><a name="p3770069415118"></a><a name="p3770069415118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.09480948094809%" headers="mcps1.2.4.1.3 "><p id="p2612244315118"><a name="p2612244315118"></a><a name="p2612244315118"></a>所属子网ID</p>
<p id="p3377540315118"><a name="p3377540315118"></a><a name="p3377540315118"></a>【使用说明】不支持更新</p>
</td>
</tr>
<tr id="row636738414597"><td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.1 "><p id="p6042468915118"><a name="p6042468915118"></a><a name="p6042468915118"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="25.95259525952595%" headers="mcps1.2.4.1.2 "><p id="p6256165915118"><a name="p6256165915118"></a><a name="p6256165915118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.09480948094809%" headers="mcps1.2.4.1.3 "><p id="p1336175915118"><a name="p1336175915118"></a><a name="p1336175915118"></a>端口IP地址</p>
<p id="p5314696715118"><a name="p5314696715118"></a><a name="p5314696715118"></a>【使用说明】不支持更新</p>
</td>
</tr>
</tbody>
</table>

**表 5**  allow\_address\_pair对象

<a name="zh-cn_topic_0062207355_table57914257"></a>
<table><thead align="left"><tr id="zh-cn_topic_0062207355_row41852331"><th class="cellrowborder" valign="top" width="25.89%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0062207355_p34595685"><a name="zh-cn_topic_0062207355_p34595685"></a><a name="zh-cn_topic_0062207355_p34595685"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="26.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0062207355_p50787128"><a name="zh-cn_topic_0062207355_p50787128"></a><a name="zh-cn_topic_0062207355_p50787128"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="47.949999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0062207355_p52626454"><a name="zh-cn_topic_0062207355_p52626454"></a><a name="zh-cn_topic_0062207355_p52626454"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0062207355_row34884411"><td class="cellrowborder" valign="top" width="25.89%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207355_p7065065"><a name="zh-cn_topic_0062207355_p7065065"></a><a name="zh-cn_topic_0062207355_p7065065"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="26.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207355_p35399367"><a name="zh-cn_topic_0062207355_p35399367"></a><a name="zh-cn_topic_0062207355_p35399367"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.949999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207355_p64721603"><a name="zh-cn_topic_0062207355_p64721603"></a><a name="zh-cn_topic_0062207355_p64721603"></a>IP地址</p>
<p id="zh-cn_topic_0062207355_p45623521"><a name="zh-cn_topic_0062207355_p45623521"></a><a name="zh-cn_topic_0062207355_p45623521"></a>【使用说明】不支持0.0.0.0</p>
</td>
</tr>
<tr id="zh-cn_topic_0062207355_row7958508"><td class="cellrowborder" valign="top" width="25.89%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0062207355_p40659381"><a name="zh-cn_topic_0062207355_p40659381"></a><a name="zh-cn_topic_0062207355_p40659381"></a>mac_address</p>
</td>
<td class="cellrowborder" valign="top" width="26.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0062207355_p5075526"><a name="zh-cn_topic_0062207355_p5075526"></a><a name="zh-cn_topic_0062207355_p5075526"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.949999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0062207355_p51982593"><a name="zh-cn_topic_0062207355_p51982593"></a><a name="zh-cn_topic_0062207355_p51982593"></a>MAC地址</p>
</td>
</tr>
</tbody>
</table>

**表 6**  extra\_dhcp\_opt对象

<a name="table5056075615524"></a>
<table><thead align="left"><tr id="row739480215524"><th class="cellrowborder" valign="top" width="25.722572257225725%" id="mcps1.2.4.1.1"><p id="p3368663215532"><a name="p3368663215532"></a><a name="p3368663215532"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="26.422642264226422%" id="mcps1.2.4.1.2"><p id="p4426268215532"><a name="p4426268215532"></a><a name="p4426268215532"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="47.85478547854785%" id="mcps1.2.4.1.3"><p id="p3407518415532"><a name="p3407518415532"></a><a name="p3407518415532"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2636755215524"><td class="cellrowborder" valign="top" width="25.722572257225725%" headers="mcps1.2.4.1.1 "><p id="p2765891815532"><a name="p2765891815532"></a><a name="p2765891815532"></a>opt_name</p>
</td>
<td class="cellrowborder" valign="top" width="26.422642264226422%" headers="mcps1.2.4.1.2 "><p id="p2577986315532"><a name="p2577986315532"></a><a name="p2577986315532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.85478547854785%" headers="mcps1.2.4.1.3 "><p id="p5884162715532"><a name="p5884162715532"></a><a name="p5884162715532"></a>Option名称</p>
</td>
</tr>
<tr id="row3942590315524"><td class="cellrowborder" valign="top" width="25.722572257225725%" headers="mcps1.2.4.1.1 "><p id="p1298235215532"><a name="p1298235215532"></a><a name="p1298235215532"></a>opt_value</p>
</td>
<td class="cellrowborder" valign="top" width="26.422642264226422%" headers="mcps1.2.4.1.2 "><p id="p4493762615532"><a name="p4493762615532"></a><a name="p4493762615532"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.85478547854785%" headers="mcps1.2.4.1.3 "><p id="p5057146315532"><a name="p5057146315532"></a><a name="p5057146315532"></a>Option值</p>
</td>
</tr>
</tbody>
</table>

**表 7**  dns\_assignment对象

<a name="table1960316535179"></a>
<table><thead align="left"><tr id="vpc_port01_0006_row860475311718"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="vpc_port01_0006_p85811122186"><a name="vpc_port01_0006_p85811122186"></a><a name="vpc_port01_0006_p85811122186"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="vpc_port01_0006_p145819129183"><a name="vpc_port01_0006_p145819129183"></a><a name="vpc_port01_0006_p145819129183"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="vpc_port01_0006_p95841215189"><a name="vpc_port01_0006_p95841215189"></a><a name="vpc_port01_0006_p95841215189"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="vpc_port01_0006_row126042530175"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="vpc_port01_0006_p5604753181710"><a name="vpc_port01_0006_p5604753181710"></a><a name="vpc_port01_0006_p5604753181710"></a>hostname</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="vpc_port01_0006_p1160475381714"><a name="vpc_port01_0006_p1160475381714"></a><a name="vpc_port01_0006_p1160475381714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="vpc_port01_0006_p5604185321716"><a name="vpc_port01_0006_p5604185321716"></a><a name="vpc_port01_0006_p5604185321716"></a>端口hostname</p>
</td>
</tr>
<tr id="vpc_port01_0006_row12604185316171"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="vpc_port01_0006_p12604185301714"><a name="vpc_port01_0006_p12604185301714"></a><a name="vpc_port01_0006_p12604185301714"></a>ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="vpc_port01_0006_p12604125311719"><a name="vpc_port01_0006_p12604125311719"></a><a name="vpc_port01_0006_p12604125311719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="vpc_port01_0006_p1060417536175"><a name="vpc_port01_0006_p1060417536175"></a><a name="vpc_port01_0006_p1060417536175"></a>端口IP地址</p>
</td>
</tr>
<tr id="vpc_port01_0006_row1860435321719"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="vpc_port01_0006_p760425311178"><a name="vpc_port01_0006_p760425311178"></a><a name="vpc_port01_0006_p760425311178"></a>fqdn</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="vpc_port01_0006_p1960465391715"><a name="vpc_port01_0006_p1960465391715"></a><a name="vpc_port01_0006_p1960465391715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="vpc_port01_0006_p1860485318172"><a name="vpc_port01_0006_p1860485318172"></a><a name="vpc_port01_0006_p1860485318172"></a>端口内网fqdn</p>
</td>
</tr>
</tbody>
</table>

**表 8**  ports\_link对象

<a name="table109221759807"></a>
<table><thead align="left"><tr id="row17420713"><th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.1"><p id="p1941101019"><a name="p1941101019"></a><a name="p1941101019"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.4.1.2"><p id="p641904118"><a name="p641904118"></a><a name="p641904118"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="71.72%" id="mcps1.2.4.1.3"><p id="p194180011"><a name="p194180011"></a><a name="p194180011"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row84506114"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p154170311"><a name="p154170311"></a><a name="p154170311"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p240019116"><a name="p240019116"></a><a name="p240019116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p1842011117"><a name="p1842011117"></a><a name="p1842011117"></a>API链接</p>
</td>
</tr>
<tr id="row1740010112"><td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.1 "><p id="p341401111"><a name="p341401111"></a><a name="p341401111"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.4.1.2 "><p id="p641901218"><a name="p641901218"></a><a name="p641901218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="71.72%" headers="mcps1.2.4.1.3 "><p id="p1942002019"><a name="p1942002019"></a><a name="p1942002019"></a>API链接与该API版本的关系</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0062207386_section15979144"></a>

【样例一】

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/ports?limit=1
    ```

-   响应样例

    ```
    {
     "ports": [{
           "id": "791870bd-36a7-4d9b-b015-a78e9b06af08",
           "name": "port-test",
           "status": "DOWN",
           "admin_state_up": true,
           "fixed_ips": [],
           "mac_address": "fa:16:3e:01:e0:b2",
           "network_id": "00ae08c5-f727-49ab-ad4b-b069398aa171",
           "tenant_id": "db82c9e1415a464ea68048baa8acc6b8",
           "project_id": "db82c9e1415a464ea68048baa8acc6b8",
           "device_id": "",
           "device_owner": "",
           "security_groups": ["d0d58aa9-cda9-414c-9c52-6c3daf8534e6"],
           "extra_dhcp_opts": [],
           "allowed_address_pairs": [],
           "binding: vnic_type": "normal",
           "binding: vif_details": {},
           "binding: profile": {},
           "port_security_enabled": true,
           "created_at": "2018-09-13T01: 43: 41",
           "updated_at": "2018-09-13T01: 43: 41"
     }]
    }
    ```


【样例二】

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/ports?mac_address=fa:16:3e:f1:0b:09
    ```


-   响应样例

    ```
    {
        "ports": [
            {
                "admin_state_up": true,
                "allowed_address_pairs": [],
                "binding:vnic_type": "normal",
                "device_id": "e6c05704-c907-4cc1-8106-69b0996c43b9",
                "device_owner": "compute:az3.dc1",
                "port_security_enabled":true,
                "extra_dhcp_opts": [],
                "fixed_ips": [
                    {
                        "ip_address": "172.16.0.37",
                        "subnet_id": "b3ac1347-63f2-4e82-b853-3d86416a0db5"
                    }
                ],
                "dns_assignment": [
                    {
                        "hostname": "ip-172-16-0-37",
                        "ip_address": "172.16.0.37",
                        "fqdn": "ip-172-16-0-37.xxx.compute.internal."
                    }
                ],
                "dns_name": "ip-172-16-0-37",
                "id": "7bb64706-6e46-4f94-a28a-4bc7caaab87d",
                "mac_address": "fa:16:3e:f1:0b:09",
                "name": "port_vm_50_3",
                "network_id": "a54e1b19-ce78-4b7e-b28b-d2d716cdc161",
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ],
                "status": "ACTIVE",
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41"
            }
        ]
    }
    ```


【样例三】

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/ports?admin_state_up=False
    ```


-   响应样例

    ```
    {
        "ports": [
    
            {
                "admin_state_up": false, 
                "allowed_address_pairs": [], 
                "binding:vnic_type": "normal", 
                "device_id": "", 
                "device_owner": "", 
                "port_security_enabled":true,
                "extra_dhcp_opts": [], 
                "fixed_ips": [
                    {
                        "ip_address": "10.100.100.62", 
                        "subnet_id": "9b28f20c-0234-419f-a0b4-4a84f182f64b"
                    }
                ], 
                "dns_name": "",
                "id": "ffc0bdee-8413-4fa2-bd82-fa8efe5b3a87", 
                "mac_address": "fa:16:3e:2b:bc:57", 
                "name": "small_net_port", 
                "network_id": "b299b151-7a66-4c6f-a313-cdd3b5724296", 
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ], 
                "status": "DOWN", 
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41"
            }
        ]
    }
    ```


【样例四】

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/ports?device_id=e6c05704-c907-4cc1-8106-69b0996c43b9
    ```


-   响应样例

    ```
    {
        "ports": [
            {
                "admin_state_up": true, 
                "allowed_address_pairs": [], 
                "binding:vnic_type": "normal", 
                "device_id": "e6c05704-c907-4cc1-8106-69b0996c43b9", 
                "device_owner": "compute:az3.dc1", 
                "port_security_enabled":true,
                "extra_dhcp_opts": [], 
                "fixed_ips": [
                    {
                        "ip_address": "10.1.0.37", 
                        "subnet_id": "b3ac1347-63f2-4e82-b853-3d86416a0db5"
                    }
                ], 
                "dns_assignment": [
                    {
                        "hostname": "ip-10-1-0-37",
                        "ip_address": "10.1.0.37",
                        "fqdn": "ip-10-1-0-37.xxx.compute.internal."//xxx为区域名称。
                    }
                ],
                "dns_name": "ip-10-1-0-37",
                "id": "7bb64706-6e46-4f94-a28a-4bc7caaab87d", 
                "mac_address": "fa:16:3e:f1:0b:09", 
                "name": "port_vm_50_3", 
                "network_id": "a54e1b19-ce78-4b7e-b28b-d2d716cdc161", 
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ], 
                "status": "ACTIVE", 
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "6c9298ec8c874f7f99688489ab65f90e" ,
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41"
            }
        ]
    }
    ```


【样例五】

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/ports?tenant_id=6c9298ec8c874f7f99688489ab65f90e&name=port_vm_50_3
    ```


-   响应样例

    ```
    {
        "ports": [
            {
                "admin_state_up": true, 
                "allowed_address_pairs": [], 
                "binding:vnic_type": "normal", 
                "device_id": "e6c05704-c907-4cc1-8106-69b0996c43b9", 
                "device_owner": "compute:az3.dc1", 
                "port_secuirty_enabled":true,
                "extra_dhcp_opts": [], 
                "fixed_ips": [
                    {
                        "ip_address": "10.1.0.37", 
                        "subnet_id": "b3ac1347-63f2-4e82-b853-3d86416a0db5"
                    }
                ], 
                "dns_assignment": [
                    {
                        "hostname": "ip-10-1-0-37",
                        "ip_address": "10.1.0.37",
                        "fqdn": "ip-10-1-0-37.xxx.compute.internal."//xxx为区域名称。
                    }
                ],
                "dns_name": "ip-10-1-0-37",
                "id": "7bb64706-6e46-4f94-a28a-4bc7caaab87d", 
                "mac_address": "fa:16:3e:f1:0b:09", 
                "name": "port_vm_50_3", 
                "network_id": "a54e1b19-ce78-4b7e-b28b-d2d716cdc161", 
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ], 
                "status": "ACTIVE", 
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "6c9298ec8c874f7f99688489ab65f90e" ,
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41"
            }
        ]
    }
    ```


【样例六】

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/ports?name=port_vm_50_3
    ```


-   响应样例

    ```
    {
        "ports": [
            {
                "status": "DOWN",
                "allowed_address_pairs": [],
                "extra_dhcp_opts": [],
                "device_owner": "",
                "port_security_enabled":true,
                "fixed_ips": [
                    {
                        "subnet_id": "391c74f7-e3b1-405c-8473-2f71a0aec7dc",
                        "ip_address": "10.1.0.33"
                    }
                ],
                "dns_name": "",
                "id": "0f405555-739f-4a19-abb7-ec11d005b3a9",
                "security_groups": [
                    "043548bc-1020-4be0-885a-caac8530e8f6"
                ],
                "device_id": "",
                "port_security_enabled":true,
                "name": "port_vm_50_3",
                "admin_state_up": true,
                "network_id": "9898a82d-7795-4ad5-bf2c-0ed8b822be4f",
                "tenant_id": "3e4a1816927f405cacbc3dca1e05111e",
                "project_id": "3e4a1816927f405cacbc3dca1e05111e",
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41",
                "binding:vnic_type": "normal",
                "mac_address": "fa:16:3e:b0:d9:cf"
            },
            {
                "status": "ACTIVE",
                "allowed_address_pairs": [],
                "extra_dhcp_opts": [],
                "device_owner": "compute:az3.dc1",
                "port_security_enabled":true,
                "fixed_ips": [
                    {
                        "subnet_id": "b3ac1347-63f2-4e82-b853-3d86416a0db5",
                        "ip_address": "10.1.0.37"
                    }
                ],
                "dns_assignment": [
                    {
                        "hostname": "ip-10-1-0-37",
                        "ip_address": "10.1.0.37",
                        "fqdn": "ip-10-1-0-37.xxx.compute.internal."//xxx为区域名称。
                     }  
                ],
                "dns_name": "ip-10-1-0-37",
                "id": "7bb64706-6e46-4f94-a28a-4bc7caaab87d",
                "security_groups": [
                    "ef69bc60-2f4b-4f97-b95b-e3b68df0c0b2"
                ],
                "device_id": "e6c05704-c907-4cc1-8106-69b0996c43b9",
                "name": "port_vm_50_3",
                "admin_state_up": true,
                "network_id": "a54e1b19-ce78-4b7e-b28b-d2d716cdc161",
                "tenant_id": "6c9298ec8c874f7f99688489ab65f90e",
                "project_id": "3e4a1816927f405cacbc3dca1e05111e",
                "created_at": "2018-09-13T01: 43: 41",
                "updated_at": "2018-09-13T01: 43: 41",
                 "binding:vnic_type": "normal", 
                "binding:vnic_type": "normal",
                "mac_address": "fa:16:3e:f1:0b:09"
            }
        ]
    }
    ```


## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

