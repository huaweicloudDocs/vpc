# 创建浮动IP<a name="vpc_floatingiP_0003"></a>

## 功能介绍<a name="section3174871621549"></a>

创建浮动IP时需要浮动IP的外部网络ID“floating\_network\_id”。

创建浮动IP时的外部网络UUID，请使用GET /v2.0/networks?router:external=True或neutron net-external-list方式获取。

## URI<a name="section5936537521549"></a>

POST /v2.0/floatingips

## 请求消息<a name="section5012846321549"></a>

**表 1**  请求参数

<a name="table3387369821549"></a>
<table><thead align="left"><tr id="row1358409521549"><th class="cellrowborder" valign="top" width="19.59%" id="mcps1.2.5.1.1"><p id="p2656991721549"><a name="p2656991721549"></a><a name="p2656991721549"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.53%" id="mcps1.2.5.1.2"><p id="p467970821549"><a name="p467970821549"></a><a name="p467970821549"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="8.25%" id="mcps1.2.5.1.3"><p id="p4351210021549"><a name="p4351210021549"></a><a name="p4351210021549"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="54.63%" id="mcps1.2.5.1.4"><p id="p3481919621549"><a name="p3481919621549"></a><a name="p3481919621549"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row178260421549"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.5.1.1 "><p id="p1017324521549"><a name="p1017324521549"></a><a name="p1017324521549"></a>floatingip</p>
</td>
<td class="cellrowborder" valign="top" width="17.53%" headers="mcps1.2.5.1.2 "><p id="p1872651821549"><a name="p1872651821549"></a><a name="p1872651821549"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="8.25%" headers="mcps1.2.5.1.3 "><p id="p4045302421549"><a name="p4045302421549"></a><a name="p4045302421549"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="54.63%" headers="mcps1.2.5.1.4 "><p id="p499181352148"><a name="p499181352148"></a><a name="p499181352148"></a>floatingip对象列表，参见<a href="#table15863423175513">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  floatingip对象

<a name="table15863423175513"></a>
<table><thead align="left"><tr id="row48631623155511"><th class="cellrowborder" valign="top" width="19.939999999999998%" id="mcps1.2.5.1.1"><p id="p23806019164"><a name="p23806019164"></a><a name="p23806019164"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="8.49%" id="mcps1.2.5.1.2"><p id="p868823916540"><a name="p868823916540"></a><a name="p868823916540"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.48%" id="mcps1.2.5.1.3"><p id="p1928287519164"><a name="p1928287519164"></a><a name="p1928287519164"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.09%" id="mcps1.2.5.1.4"><p id="p4943306019164"><a name="p4943306019164"></a><a name="p4943306019164"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7864323175518"><td class="cellrowborder" valign="top" width="19.939999999999998%" headers="mcps1.2.5.1.1 "><p id="p2022646619164"><a name="p2022646619164"></a><a name="p2022646619164"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="8.49%" headers="mcps1.2.5.1.2 "><p id="p17689839165418"><a name="p17689839165418"></a><a name="p17689839165418"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.5.1.3 "><p id="p2773103519164"><a name="p2773103519164"></a><a name="p2773103519164"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.09%" headers="mcps1.2.5.1.4 "><p id="p2292670119164"><a name="p2292670119164"></a><a name="p2292670119164"></a>浮动IP地址。</p>
</td>
</tr>
<tr id="row1686417238557"><td class="cellrowborder" valign="top" width="19.939999999999998%" headers="mcps1.2.5.1.1 "><p id="p345796219164"><a name="p345796219164"></a><a name="p345796219164"></a>floating_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.49%" headers="mcps1.2.5.1.2 "><p id="p1068933955414"><a name="p1068933955414"></a><a name="p1068933955414"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.5.1.3 "><p id="p1165952819164"><a name="p1165952819164"></a><a name="p1165952819164"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.09%" headers="mcps1.2.5.1.4 "><p id="p1389784219164"><a name="p1389784219164"></a><a name="p1389784219164"></a>外部网络的id。</p>
<p id="p186012181292"><a name="p186012181292"></a><a name="p186012181292"></a>只能使用固定的外网，外部网络的信息请通过</p>
<p id="p095071919913"><a name="p095071919913"></a><a name="p095071919913"></a>GET /v2.0/networks?router:external=True或</p>
<p id="p520001217911"><a name="p520001217911"></a><a name="p520001217911"></a>GET /v2.0/networks?name={floating_network}或</p>
<p id="p5797172119164"><a name="p5797172119164"></a><a name="p5797172119164"></a>neutron net-external-list方式查询。</p>
</td>
</tr>
<tr id="row98641023145511"><td class="cellrowborder" valign="top" width="19.939999999999998%" headers="mcps1.2.5.1.1 "><p id="p4886025919164"><a name="p4886025919164"></a><a name="p4886025919164"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="8.49%" headers="mcps1.2.5.1.2 "><p id="p1868973975414"><a name="p1868973975414"></a><a name="p1868973975414"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.5.1.3 "><p id="p6536694419164"><a name="p6536694419164"></a><a name="p6536694419164"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.09%" headers="mcps1.2.5.1.4 "><p id="p2628234219164"><a name="p2628234219164"></a><a name="p2628234219164"></a>端口id</p>
</td>
</tr>
<tr id="row1086519236554"><td class="cellrowborder" valign="top" width="19.939999999999998%" headers="mcps1.2.5.1.1 "><p id="p3380179719164"><a name="p3380179719164"></a><a name="p3380179719164"></a>fixed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="8.49%" headers="mcps1.2.5.1.2 "><p id="p368912399543"><a name="p368912399543"></a><a name="p368912399543"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.5.1.3 "><p id="p5359099919164"><a name="p5359099919164"></a><a name="p5359099919164"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.09%" headers="mcps1.2.5.1.4 "><p id="p1829247919164"><a name="p1829247919164"></a><a name="p1829247919164"></a>关联端口的私有IP地址。</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section6384765421549"></a>

**表 3**  响应参数

<a name="table427745721549"></a>
<table><thead align="left"><tr id="row435809221549"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="p1746120521549"><a name="p1746120521549"></a><a name="p1746120521549"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.11%" id="mcps1.2.4.1.2"><p id="p507150621549"><a name="p507150621549"></a><a name="p507150621549"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="59.540000000000006%" id="mcps1.2.4.1.3"><p id="p5526791421549"><a name="p5526791421549"></a><a name="p5526791421549"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4751605321549"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="p2359506021549"><a name="p2359506021549"></a><a name="p2359506021549"></a>floatingip</p>
</td>
<td class="cellrowborder" valign="top" width="19.11%" headers="mcps1.2.4.1.2 "><p id="p3215169621549"><a name="p3215169621549"></a><a name="p3215169621549"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="59.540000000000006%" headers="mcps1.2.4.1.3 "><p id="p2411791621549"><a name="p2411791621549"></a><a name="p2411791621549"></a>floatingip对象列表，参见<a href="#table8139247714">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  floatingip对象

<a name="table8139247714"></a>
<table><thead align="left"><tr id="row18132240714"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p101201250870"><a name="p101201250870"></a><a name="p101201250870"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p161211850674"><a name="p161211850674"></a><a name="p161211850674"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p41217502719"><a name="p41217502719"></a><a name="p41217502719"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2014192410713"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p6028218019164"><a name="p6028218019164"></a><a name="p6028218019164"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p5101843519164"><a name="p5101843519164"></a><a name="p5101843519164"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p6000412319164"><a name="p6000412319164"></a><a name="p6000412319164"></a>网络状态，可以为ACTIVE， DOWN或ERROR。</p>
<a name="ul10603143175810"></a><a name="ul10603143175810"></a><ul id="ul10603143175810"><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ERROR ：异常</li></ul>
</td>
</tr>
<tr id="row4141241070"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p5513524919164"><a name="p5513524919164"></a><a name="p5513524919164"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p212111505713"><a name="p212111505713"></a><a name="p212111505713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p4121850371"><a name="p4121850371"></a><a name="p4121850371"></a>浮动IP地址的id。</p>
</td>
</tr>
<tr id="row614132416712"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1912112509713"><a name="p1912112509713"></a><a name="p1912112509713"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p11211850072"><a name="p11211850072"></a><a name="p11211850072"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p16122205017713"><a name="p16122205017713"></a><a name="p16122205017713"></a>浮动IP地址。</p>
</td>
</tr>
<tr id="row115102414717"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p61223503712"><a name="p61223503712"></a><a name="p61223503712"></a>floating_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1812220507714"><a name="p1812220507714"></a><a name="p1812220507714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p16122550274"><a name="p16122550274"></a><a name="p16122550274"></a>外部网络的id。</p>
</td>
</tr>
<tr id="row19155241277"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p201223504719"><a name="p201223504719"></a><a name="p201223504719"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1122155015714"><a name="p1122155015714"></a><a name="p1122155015714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p812212506713"><a name="p812212506713"></a><a name="p812212506713"></a>所属路由器id。</p>
</td>
</tr>
<tr id="row101514247714"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p412218502718"><a name="p412218502718"></a><a name="p412218502718"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p612213506716"><a name="p612213506716"></a><a name="p612213506716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p141228504716"><a name="p141228504716"></a><a name="p141228504716"></a>端口id</p>
</td>
</tr>
<tr id="row3164249715"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p01237508720"><a name="p01237508720"></a><a name="p01237508720"></a>fixed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p111239501770"><a name="p111239501770"></a><a name="p111239501770"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1712316501972"><a name="p1712316501972"></a><a name="p1712316501972"></a>关联端口的私有IP地址。</p>
</td>
</tr>
<tr id="row21662416711"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p812355018717"><a name="p812355018717"></a><a name="p812355018717"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p612316509712"><a name="p612316509712"></a><a name="p612316509712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
<p id="p51231950174"><a name="p51231950174"></a><a name="p51231950174"></a>。</p>
</td>
</tr>
<tr id="row11176241720"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p11222111885214"><a name="p11222111885214"></a><a name="p11222111885214"></a>dns_name</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p122232018115215"><a name="p122232018115215"></a><a name="p122232018115215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p18223161825216"><a name="p18223161825216"></a><a name="p18223161825216"></a>DNS名称</p>
</td>
</tr>
<tr id="row17174241670"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p492133065713"><a name="p492133065713"></a><a name="p492133065713"></a>dns_domain</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p16929300573"><a name="p16929300573"></a><a name="p16929300573"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p3921230175711"><a name="p3921230175711"></a><a name="p3921230175711"></a>DNS域地址</p>
</td>
</tr>
<tr id="row1418142410714"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1953114119914"><a name="p1953114119914"></a><a name="p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p595318416919"><a name="p595318416919"></a><a name="p595318416919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1395374115919"><a name="p1395374115919"></a><a name="p1395374115919"></a>资源创建时间</p>
<p id="p1232884613478"><a name="p1232884613478"></a><a name="p1232884613478"></a>采用UTC时间</p>
<p id="p2070141994713"><a name="p2070141994713"></a><a name="p2070141994713"></a>格式：YYYY-MM-DDTHH:MM:SS</p>
</td>
</tr>
<tr id="row1188246714"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p139719548912"><a name="p139719548912"></a><a name="p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p53971154594"><a name="p53971154594"></a><a name="p53971154594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1339713549918"><a name="p1339713549918"></a><a name="p1339713549918"></a>资源更新时间</p>
<p id="p876511114816"><a name="p876511114816"></a><a name="p876511114816"></a>采用UTC时间</p>
<p id="p137222218476"><a name="p137222218476"></a><a name="p137222218476"></a>格式：YYYY-MM-DDTHH:MM:SS</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section1573465921549"></a>

请求样例

```
POST https://{Endpoint}/v2.0/floatingips 

{
    "floatingip": {
           "floating_network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975"
    }
}
```

响应样例

```
{
    "floatingip": {
        "id": "b997e0d4-3359-4c74-8f88-bc0af81cd5a2",
        "status": "DOWN",
        "router_id": null,
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "floating_network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
        "fixed_ip_address": null,
        "floating_ip_address": "88.88.215.205",
        "port_id": null,
        "created_at": "2018-09-20T02:10:02",
        "updated_at": "2018-09-20T02:10:02"
    }
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

