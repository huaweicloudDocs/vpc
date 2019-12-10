# 查询网络IP使用情况<a name="vpc_natworkip_0001"></a>

## 功能介绍<a name="section1398541881511"></a>

显示一个指定网络中的IP地址使用情况。

包括此网络中的IP总数以及已用IP总数，以及网络下每一个子网的IP地址总数和可用IP地址总数

>![](public_sys-resources/icon-notice.gif) **须知：**   
>-   系统预留地址指的是子网的第1个以及最后4个地址，一般用于网关、DHCP等服务。  
>-   这里以及下文描述的IP地址总数、已用IP地址总数不包含系统预留地址。  
>-   在分配IP时，用户可以指定系统预留的IP地址。但是不论IP是如何分配的，只要是处于系统预留IP地址段的IP均不会被统计到已用IP地址数目和IP地址总数中。  

## URI<a name="section5633932181719"></a>

GET /v2.0/network-ip-availabilities/\{network\_id\}

参数说明请参见[表1](#table38148684)。

**表 1**  参数说明

<a name="table38148684"></a>
<table><thead align="left"><tr id="row7162954"><th class="cellrowborder" valign="top" width="25.507449255074494%" id="mcps1.2.5.1.1"><p id="p43328398"><a name="p43328398"></a><a name="p43328398"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.5.1.2"><p id="p19939379"><a name="p19939379"></a><a name="p19939379"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.5.1.3"><p id="p4477025"><a name="p4477025"></a><a name="p4477025"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="45.91540845915409%" id="mcps1.2.5.1.4"><p id="p27094719"><a name="p27094719"></a><a name="p27094719"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row47188597"><td class="cellrowborder" valign="top" width="25.507449255074494%" headers="mcps1.2.5.1.1 "><p id="p64180012"><a name="p64180012"></a><a name="p64180012"></a>network_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p31198475"><a name="p31198475"></a><a name="p31198475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.3 "><p id="p44048571"><a name="p44048571"></a><a name="p44048571"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="45.91540845915409%" headers="mcps1.2.5.1.4 "><p id="p11164516"><a name="p11164516"></a><a name="p11164516"></a>网络的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section447915459203"></a>

-   请求参数

    无

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/network-ip-availabilities/6b50d967-779c-40c9-a157-de1df3c17043
    ```


## 响应消息<a name="section752610492226"></a>

-   响应参数

    **表 2**  响应参数

    <a name="table966523163317"></a>
    <table><thead align="left"><tr id="row966563103315"><th class="cellrowborder" valign="top" width="33.333333333333336%" id="mcps1.2.4.1.1"><p id="p866615363313"><a name="p866615363313"></a><a name="p866615363313"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.333333333333336%" id="mcps1.2.4.1.2"><p id="p8666143153316"><a name="p8666143153316"></a><a name="p8666143153316"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.333333333333336%" id="mcps1.2.4.1.3"><p id="p66667320335"><a name="p66667320335"></a><a name="p66667320335"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1166619314334"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p176661383319"><a name="p176661383319"></a><a name="p176661383319"></a>network_ip_availability</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p12666439333"><a name="p12666439333"></a><a name="p12666439333"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p666612311331"><a name="p666612311331"></a><a name="p666612311331"></a>network_ip_avalability对象，请参见<a href="#table4952133061113">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  network\_ip\_availability对象

    <a name="table4952133061113"></a>
    <table><thead align="left"><tr id="row59521030171119"><th class="cellrowborder" valign="top" width="33.333333333333336%" id="mcps1.2.4.1.1"><p id="p109521330171118"><a name="p109521330171118"></a><a name="p109521330171118"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.333333333333336%" id="mcps1.2.4.1.2"><p id="p20952113013119"><a name="p20952113013119"></a><a name="p20952113013119"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.333333333333336%" id="mcps1.2.4.1.3"><p id="p79525309113"><a name="p79525309113"></a><a name="p79525309113"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row17952113001111"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p18952103061110"><a name="p18952103061110"></a><a name="p18952103061110"></a>network_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p9954103081111"><a name="p9954103081111"></a><a name="p9954103081111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p16954130171120"><a name="p16954130171120"></a><a name="p16954130171120"></a>网络ID</p>
    </td>
    </tr>
    <tr id="row19954133091119"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p11954193013117"><a name="p11954193013117"></a><a name="p11954193013117"></a>network_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p195413091117"><a name="p195413091117"></a><a name="p195413091117"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p19541130111110"><a name="p19541130111110"></a><a name="p19541130111110"></a>网络名称</p>
    </td>
    </tr>
    <tr id="row159543309110"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p1295443001116"><a name="p1295443001116"></a><a name="p1295443001116"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p18954430201118"><a name="p18954430201118"></a><a name="p18954430201118"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row13954730161115"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p39551930121112"><a name="p39551930121112"></a><a name="p39551930121112"></a>total_ips</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p179551630111114"><a name="p179551630111114"></a><a name="p179551630111114"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p119559304119"><a name="p119559304119"></a><a name="p119559304119"></a>网络中IP总数（不包含系统预留地址）</p>
    </td>
    </tr>
    <tr id="row295553016117"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p59551830161120"><a name="p59551830161120"></a><a name="p59551830161120"></a>used_ips</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p14955113081119"><a name="p14955113081119"></a><a name="p14955113081119"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p17955193011112"><a name="p17955193011112"></a><a name="p17955193011112"></a>网络中已经使用的IP数目（不包含系统预留地址）</p>
    </td>
    </tr>
    <tr id="row6955830121114"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p19955103061116"><a name="p19955103061116"></a><a name="p19955103061116"></a>subnet_ip_availability</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p89556306114"><a name="p89556306114"></a><a name="p89556306114"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p1395513031116"><a name="p1395513031116"></a><a name="p1395513031116"></a>子网IP使用情况的对象，参见<a href="#table110015141519">表4</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  subnet\_ip\_availability对象说明

    <a name="table110015141519"></a>
    <table><thead align="left"><tr id="row5101145151518"><th class="cellrowborder" valign="top" width="33.33%" id="mcps1.2.4.1.1"><p id="p610120518150"><a name="p610120518150"></a><a name="p610120518150"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33%" id="mcps1.2.4.1.2"><p id="p10101105171513"><a name="p10101105171513"></a><a name="p10101105171513"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.339999999999996%" id="mcps1.2.4.1.3"><p id="p5101145151519"><a name="p5101145151519"></a><a name="p5101145151519"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12101751141514"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.1 "><p id="p110185111151"><a name="p110185111151"></a><a name="p110185111151"></a>used_ips</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.2 "><p id="p9102155131519"><a name="p9102155131519"></a><a name="p9102155131519"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.339999999999996%" headers="mcps1.2.4.1.3 "><p id="p21021251151518"><a name="p21021251151518"></a><a name="p21021251151518"></a>子网中已经使用的IP数目（不包含系统预留地址）</p>
    </td>
    </tr>
    <tr id="row10967175517178"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.1 "><p id="p12968105517179"><a name="p12968105517179"></a><a name="p12968105517179"></a>subnet_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.2 "><p id="p4968175511716"><a name="p4968175511716"></a><a name="p4968175511716"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.339999999999996%" headers="mcps1.2.4.1.3 "><p id="p17968175591718"><a name="p17968175591718"></a><a name="p17968175591718"></a>子网ID</p>
    </td>
    </tr>
    <tr id="row172761838198"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.1 "><p id="p42761137197"><a name="p42761137197"></a><a name="p42761137197"></a>subnet_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.2 "><p id="p7276735198"><a name="p7276735198"></a><a name="p7276735198"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.339999999999996%" headers="mcps1.2.4.1.3 "><p id="p19276193141915"><a name="p19276193141915"></a><a name="p19276193141915"></a>子网名称</p>
    </td>
    </tr>
    <tr id="row28750203194"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.1 "><p id="p128759204193"><a name="p128759204193"></a><a name="p128759204193"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.2 "><p id="p987532012194"><a name="p987532012194"></a><a name="p987532012194"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.339999999999996%" headers="mcps1.2.4.1.3 "><p id="p168761720161914"><a name="p168761720161914"></a><a name="p168761720161914"></a>子网的IP版本，取值为4或者6</p>
    </td>
    </tr>
    <tr id="row1247822162114"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.1 "><p id="p047815214214"><a name="p047815214214"></a><a name="p047815214214"></a>cidr</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.2 "><p id="p1647820252111"><a name="p1647820252111"></a><a name="p1647820252111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.339999999999996%" headers="mcps1.2.4.1.3 "><p id="p1147842182113"><a name="p1147842182113"></a><a name="p1147842182113"></a>子网的CIDR</p>
    </td>
    </tr>
    <tr id="row18913174252716"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.1 "><p id="p19141942112712"><a name="p19141942112712"></a><a name="p19141942112712"></a>total_ips</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.2.4.1.2 "><p id="p209141142102720"><a name="p209141142102720"></a><a name="p209141142102720"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.339999999999996%" headers="mcps1.2.4.1.3 "><p id="p13914942152716"><a name="p13914942152716"></a><a name="p13914942152716"></a>子网中IP总数（不包含系统预留地址）</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
      "network_ip_availability": {
        "used_ips": 4,
        "subnet_ip_availability": [
          {
            "used_ips": 4,
            "subnet_id": "98e343d1-3cb8-4f69-9cd1-00569819480f",
            "subnet_name": "",
            "ip_version": 4,
            "cidr": "10.0.0.0/8",
            "total_ips": 300
          }
        ],
        "network_id": "6b50d967-779c-40c9-a157-de1df3c17043",
        "tenant_id": "7c4b23cb125d481c95cbe4f91b2c11cd",
        "total_ips": 300,
        "network_name": "pch_test_003"
      }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

