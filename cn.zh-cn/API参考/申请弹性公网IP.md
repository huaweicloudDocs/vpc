# 申请弹性公网IP<a name="ZH-CN_TOPIC_0201534274"></a>

## 功能介绍<a name="section12153337"></a>

申请弹性公网IP，支持IPv4和IPv6。

弹性公网IP（Elastic IP）提供独立的公网IP资源，包括公网IP地址与公网出口带宽服务。可以与弹性云服务器、裸金属服务器、虚拟IP、弹性负载均衡、NAT网关等资源灵活地绑定及解绑。拥有多种灵活的计费方式，可以满足各种业务场景的需要。

## URI<a name="section42271171"></a>

POST /v1/\{project\_id\}/publicips

参数说明请参见[表1](#table57311924)。

**表 1**  参数说明

<a name="table57311924"></a>
<table><thead align="left"><tr id="row11854613"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p20699582"><a name="p20699582"></a><a name="p20699582"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p66053444"><a name="p66053444"></a><a name="p66053444"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p48728718"><a name="p48728718"></a><a name="p48728718"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row54712068"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p2492560"><a name="p2492560"></a><a name="p2492560"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p570775"><a name="p570775"></a><a name="p570775"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section44896221"></a>

-   请求参数

    **表 2**  请求参数

    <a name="table62031189151043"></a>
    <table><thead align="left"><tr id="row4339910151043"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="p15988448151043"><a name="p15988448151043"></a><a name="p15988448151043"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="p19995902151043"><a name="p19995902151043"></a><a name="p19995902151043"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="p9055369151043"><a name="p9055369151043"></a><a name="p9055369151043"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.18%" id="mcps1.2.5.1.4"><p id="p62396264151043"><a name="p62396264151043"></a><a name="p62396264151043"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row20932612151043"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p17819972151043"><a name="p17819972151043"></a><a name="p17819972151043"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p34131600151043"><a name="p34131600151043"></a><a name="p34131600151043"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p13196241151043"><a name="p13196241151043"></a><a name="p13196241151043"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p23492844151043"><a name="p23492844151043"></a><a name="p23492844151043"></a>弹性公网IP对象，请参见<a href="#table4491214">表3</a>。</p>
    </td>
    </tr>
    <tr id="row13560713151050"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p24675975151050"><a name="p24675975151050"></a><a name="p24675975151050"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p52596998151050"><a name="p52596998151050"></a><a name="p52596998151050"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p12429959151120"><a name="p12429959151120"></a><a name="p12429959151120"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p1744019151120"><a name="p1744019151120"></a><a name="p1744019151120"></a>带宽对象，请参见<a href="#table11041789">表4</a>。</p>
    </td>
    </tr>
    <tr id="row7563161315419"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p19564181313543"><a name="p19564181313543"></a><a name="p19564181313543"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p13564413185412"><a name="p13564413185412"></a><a name="p13564413185412"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p95641133547"><a name="p95641133547"></a><a name="p95641133547"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><a name="ul16411048123"></a><a name="ul16411048123"></a><ul id="ul16411048123"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。</li><li>创建弹性公网IP时，给弹性公网IP绑定企业项目ID。</li><li>不指定该参数时，默认值是 0</li></ul>
    <div class="note" id="note16336122416016"><a name="note16336122416016"></a><a name="note16336122416016"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1915862704914"><a name="p1915862704914"></a><a name="p1915862704914"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0126101490.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicip字段说明

    <a name="table4491214"></a>
    <table><thead align="left"><tr id="row21610982"><th class="cellrowborder" valign="top" width="31%" id="mcps1.2.5.1.1"><p id="p5659087"><a name="p5659087"></a><a name="p5659087"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.2"><p id="p55732864"><a name="p55732864"></a><a name="p55732864"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.9%" id="mcps1.2.5.1.3"><p id="p4226242618129"><a name="p4226242618129"></a><a name="p4226242618129"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.1%" id="mcps1.2.5.1.4"><p id="p18068130"><a name="p18068130"></a><a name="p18068130"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row54232412"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.5.1.1 "><p id="p30749271"><a name="p30749271"></a><a name="p30749271"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.2 "><p id="p7663035"><a name="p7663035"></a><a name="p7663035"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.9%" headers="mcps1.2.5.1.3 "><p id="p70444218129"><a name="p70444218129"></a><a name="p70444218129"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.1%" headers="mcps1.2.5.1.4 "><a name="ul29589093174724"></a><a name="ul29589093174724"></a><ul id="ul29589093174724"><li>功能说明：弹性公网IP的类型</li><li>取值范围：<em id="i16850184017499"><a name="i16850184017499"></a><a name="i16850184017499"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="ul585004064911"></a><a name="ul585004064911"></a><ul id="ul585004064911"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li></ul>
    </li><li>约束：<a name="ul9738153015499"></a><a name="ul9738153015499"></a><ul id="ul9738153015499"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"publicip_type"字段未给定时，默认为5_bgp。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row4771536182914"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.5.1.1 "><p id="p1661484872917"><a name="p1661484872917"></a><a name="p1661484872917"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.2 "><p id="p1861404882912"><a name="p1861404882912"></a><a name="p1861404882912"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.9%" headers="mcps1.2.5.1.3 "><p id="p1661413481295"><a name="p1661413481295"></a><a name="p1661413481295"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.1%" headers="mcps1.2.5.1.4 "><a name="ul1842191914615"></a><a name="ul1842191914615"></a><ul id="ul1842191914615"><li>功能说明：弹性公网IP的版本</li><li>取值范围：4、6，分别表示创建ipv4和ipv6</li><li>约束：<a name="ul1190139775"></a><a name="ul1190139775"></a><ul id="ul1190139775"><li>必须是系统具体支持的类型</li><li>不填或空字符串时，默认创建ipv4</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row116305209446"><td class="cellrowborder" valign="top" width="31%" headers="mcps1.2.5.1.1 "><p id="p25480789446"><a name="p25480789446"></a><a name="p25480789446"></a>ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.2 "><p id="p50677729446"><a name="p50677729446"></a><a name="p50677729446"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.9%" headers="mcps1.2.5.1.3 "><p id="p78364279446"><a name="p78364279446"></a><a name="p78364279446"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.1%" headers="mcps1.2.5.1.4 "><a name="ul3888143018611"></a><a name="ul3888143018611"></a><ul id="ul3888143018611"><li>功能说明：希望申请到的弹性公网IP的地址，不指定时由系统自动分配</li><li>约束：必须为IPv4地址格式，且必须在可用地址池范围内</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  bandwidth字段说明

    <a name="table11041789"></a>
    <table><thead align="left"><tr id="row60677888"><th class="cellrowborder" valign="top" width="30.826917308269174%" id="mcps1.2.5.1.1"><p id="p15961928"><a name="p15961928"></a><a name="p15961928"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.10828917108289%" id="mcps1.2.5.1.2"><p id="p17847776"><a name="p17847776"></a><a name="p17847776"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.2.5.1.3"><p id="p3784029918155"><a name="p3784029918155"></a><a name="p3784029918155"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.886911308869113%" id="mcps1.2.5.1.4"><p id="p36383728"><a name="p36383728"></a><a name="p36383728"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row61400865"><td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.1 "><p id="p7414170"><a name="p7414170"></a><a name="p7414170"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.10828917108289%" headers="mcps1.2.5.1.2 "><p id="p63676932"><a name="p63676932"></a><a name="p63676932"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.2.5.1.3 "><p id="p4516535118155"><a name="p4516535118155"></a><a name="p4516535118155"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.886911308869113%" headers="mcps1.2.5.1.4 "><a name="ul518119181073"></a><a name="ul518119181073"></a><ul id="ul518119181073"><li>功能说明：带宽名称</li><li>取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li><li>如果share_type是PER，该参数必须带,如果share_type是WHOLE并且id有值，该参数会忽略。</li></ul>
    </td>
    </tr>
    <tr id="row15772917"><td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.1 "><p id="p2537905"><a name="p2537905"></a><a name="p2537905"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.10828917108289%" headers="mcps1.2.5.1.2 "><p id="p4243749"><a name="p4243749"></a><a name="p4243749"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.2.5.1.3 "><p id="p3451484018155"><a name="p3451484018155"></a><a name="p3451484018155"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.886911308869113%" headers="mcps1.2.5.1.4 "><a name="ul194366475712"></a><a name="ul194366475712"></a><ul id="ul194366475712"><li>功能说明：带宽大小</li><li>取值范围：默认1Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。</li><li>约束：share_type是PER，该参数必须带,如果share_type是WHOLE并且id有值，该参数会忽略。</li><li>注意：调整带宽时的最小单位会根据带宽范围不同存在差异。<a name="ul9790510185"></a><a name="ul9790510185"></a><ul id="ul9790510185"><li>小于等于300Mbit/s：默认最小单位为1Mbit/s。</li><li>300Mbit/s~1000Mbit/s：默认最小单位为50Mbit/s。</li><li>大于1000Mbit/s：默认最小单位为500Mbit/s。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row42186470"><td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.1 "><p id="p61660876"><a name="p61660876"></a><a name="p61660876"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.10828917108289%" headers="mcps1.2.5.1.2 "><p id="p28475059"><a name="p28475059"></a><a name="p28475059"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.2.5.1.3 "><p id="p4423869418155"><a name="p4423869418155"></a><a name="p4423869418155"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.886911308869113%" headers="mcps1.2.5.1.4 "><a name="ul569842518819"></a><a name="ul569842518819"></a><ul id="ul569842518819"><li>功能说明：带宽ID，创建弹性公网IP时可以指定已有的共享带宽</li><li>取值范围：共享（WHOLE类型）带宽ID</li></ul>
    </td>
    </tr>
    <tr id="row33642107"><td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.1 "><p id="p40656116"><a name="p40656116"></a><a name="p40656116"></a>share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.10828917108289%" headers="mcps1.2.5.1.2 "><p id="p4811061"><a name="p4811061"></a><a name="p4811061"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.2.5.1.3 "><p id="p2656447218155"><a name="p2656447218155"></a><a name="p2656447218155"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.886911308869113%" headers="mcps1.2.5.1.4 "><a name="ul2255712095"></a><a name="ul2255712095"></a><ul id="ul2255712095"><li>功能说明：带宽类型</li><li>取值范围：<a name="ul143257017559"></a><a name="ul143257017559"></a><ul id="ul143257017559"><li>PER：独享带宽</li><li>WHOLE：共享带宽</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row17737188172319"><td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.1 "><p id="p27426113172319"><a name="p27426113172319"></a><a name="p27426113172319"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.10828917108289%" headers="mcps1.2.5.1.2 "><p id="p55776100172330"><a name="p55776100172330"></a><a name="p55776100172330"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.2.5.1.3 "><p id="p23864764172319"><a name="p23864764172319"></a><a name="p23864764172319"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.886911308869113%" headers="mcps1.2.5.1.4 "><a name="ul152417331215"></a><a name="ul152417331215"></a><ul id="ul152417331215"><li>功能说明：按流量计费还是按带宽计费。</li><li>取值范围：bandwidth，traffic，不填或者为空时默认是bandwidth。其中IPv6国外默认是bandwidth，国内默认是traffic。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例一（IPv4 EIP独享带宽）

    ```
    POST https://{Endpoint}/v1/{project_id}/publicips
    
    {
        "publicip": {
            "type": "5_bgp",
            "ip_version": 4
        },
        "bandwidth": {
            "name": "bandwidth123",
            "size": 10,
            "share_type": "PER"
        },
        "enterprise_project_id":"b261ac1f-2489-4bc7-b31b-c33c3346a439"
    }
    ```


-   请求样例二（IPv6 EIP共享带宽）

    ```
    POST https://{Endpoint}/v1/{project_id}/publicips
    
    {    
    	"publicip": {        
    		"type": "5_bgp",        
    		"ip_version": 6       
    	},   
    	"bandwidth": {       
    		"name": "bandwidth123",       
    		"size": 5,        
    		"share_type": "WHOLE"    		
    	},         
    	"enterprise_project_id":"0"    	
    }
    ```


## 响应消息<a name="section1412808"></a>

-   响应参数

    **表 5**  响应参数

    <a name="table32663367152049"></a>
    <table><thead align="left"><tr id="row49418185152049"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p43450028152049"><a name="p43450028152049"></a><a name="p43450028152049"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="p64289235152049"><a name="p64289235152049"></a><a name="p64289235152049"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="p40045543152049"><a name="p40045543152049"></a><a name="p40045543152049"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row22463580152049"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p7610714152049"><a name="p7610714152049"></a><a name="p7610714152049"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p4900878152049"><a name="p4900878152049"></a><a name="p4900878152049"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p15970624152049"><a name="p15970624152049"></a><a name="p15970624152049"></a>弹性公网IP对象，请参见<a href="#table44471219">表6</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  publicip字段说明

    <a name="table44471219"></a>
    <table><thead align="left"><tr id="row33860402"><th class="cellrowborder" valign="top" width="38%" id="mcps1.2.4.1.1"><p id="p58338056"><a name="p58338056"></a><a name="p58338056"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24%" id="mcps1.2.4.1.2"><p id="p4133121218330"><a name="p4133121218330"></a><a name="p4133121218330"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="38%" id="mcps1.2.4.1.3"><p id="p34137829"><a name="p34137829"></a><a name="p34137829"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row13700797"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p36022757"><a name="p36022757"></a><a name="p36022757"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p5949386218330"><a name="p5949386218330"></a><a name="p5949386218330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><p id="p25236858"><a name="p25236858"></a><a name="p25236858"></a>弹性公网IP唯一标识</p>
    </td>
    </tr>
    <tr id="row25805135"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p9841225"><a name="p9841225"></a><a name="p9841225"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p5427353718330"><a name="p5427353718330"></a><a name="p5427353718330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><a name="ul052132731516"></a><a name="ul052132731516"></a><ul id="ul052132731516"><li>功能说明：弹性公网IP的状态</li><li>取值范围：<a name="ul10603143175810"></a><a name="ul10603143175810"></a><ul id="ul10603143175810"><li>FREEZED：冻结</li><li>BIND_ERROR：绑定失败</li><li>BINDING：绑定中</li><li>PENDING_DELETE：释放中</li><li>PENDING_CREATE：创建中</li><li>PENDING_UPDATE：更新中</li><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ELB：绑定ELB</li><li>ERROR：异常失败</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row66476022"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p1332417268438"><a name="p1332417268438"></a><a name="p1332417268438"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p3408038918330"><a name="p3408038918330"></a><a name="p3408038918330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><a name="ul61069400416"></a><a name="ul61069400416"></a><ul id="ul61069400416"><li>功能说明：弹性公网IP的类型</li><li>取值范围：<em id="i18107114018414"><a name="i18107114018414"></a><a name="i18107114018414"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="ul13107164012416"></a><a name="ul13107164012416"></a><ul id="ul13107164012416"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li></ul>
    </li><li>约束：<a name="ul1010714409416"></a><a name="ul1010714409416"></a><ul id="ul1010714409416"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"publicip_type"字段未给定时，默认为5_bgp。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row53754023"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p59108624"><a name="p59108624"></a><a name="p59108624"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p904808818330"><a name="p904808818330"></a><a name="p904808818330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><p id="p40237373"><a name="p40237373"></a><a name="p40237373"></a>IPv4时是申请到的弹性公网IP地址，IPv6时是IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="row25891604376"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p174765913710"><a name="p174765913710"></a><a name="p174765913710"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p18476149163714"><a name="p18476149163714"></a><a name="p18476149163714"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><p id="p1447614916377"><a name="p1447614916377"></a><a name="p1447614916377"></a>IPv4时无此字段，IPv6时为申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="row58647356212"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p171101456172118"><a name="p171101456172118"></a><a name="p171101456172118"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p1811012569218"><a name="p1811012569218"></a><a name="p1811012569218"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><p id="p1211011564217"><a name="p1211011564217"></a><a name="p1211011564217"></a>IP版本信息，取值范围是4和6</p>
    <a name="ul13987110227"></a><a name="ul13987110227"></a><ul id="ul13987110227"><li>4：表示IPv4</li><li>6：表示IPv6</li></ul>
    </td>
    </tr>
    <tr id="row26592044"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p6471942"><a name="p6471942"></a><a name="p6471942"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p6180656518330"><a name="p6180656518330"></a><a name="p6180656518330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><p id="p17634333267"><a name="p17634333267"></a><a name="p17634333267"></a>项目ID</p>
    </td>
    </tr>
    <tr id="row43875021"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p64215808"><a name="p64215808"></a><a name="p64215808"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p4027585818330"><a name="p4027585818330"></a><a name="p4027585818330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><p id="p27139175"><a name="p27139175"></a><a name="p27139175"></a>弹性公网IP申请时间（UTC）</p>
    </td>
    </tr>
    <tr id="row42925989"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p54453050"><a name="p54453050"></a><a name="p54453050"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p4111904718330"><a name="p4111904718330"></a><a name="p4111904718330"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><p id="p11161650"><a name="p11161650"></a><a name="p11161650"></a>带宽大小，单位为Mbit/s。</p>
    </td>
    </tr>
    <tr id="row59251766137"><td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.1 "><p id="p4160981130"><a name="p4160981130"></a><a name="p4160981130"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="p201633831312"><a name="p201633831312"></a><a name="p201633831312"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="38%" headers="mcps1.2.4.1.3 "><a name="ul11996131168"></a><a name="ul11996131168"></a><ul id="ul11996131168"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。</li><li>创建弹性公网IP时，给弹性公网IP绑定企业项目ID。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例一（IPv4 EIP独享带宽）

    ```
    {
        "publicip": {
            "id": "f588ccfa-8750-4d7c-bf5d-2ede24414706",
            "status": "PENDING_CREATE",
            "type": "5_bgp",
            "public_ip_address": "161.xx.xx.7",
            "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
            "ip_version": 4,
            "create_time": "2015-07-16 04:10:52",
            "bandwidth_size": 0,
            "enterprise_project_id":"b261ac1f-2489-4bc7-b31b-c33c3346a439"
        }
    }
    ```


-   响应样例二（IPv6 EIP共享带宽）

    ```
    {
      "publicip": {
        "id": "3ff2bf48-b82d-4bf3-88e7-9e55ecdedc34",
        "status": "PENDING_CREATE",
        "type": "5_bgp",
        "public_ip_address": "10.154.79.48",
        "public_ipv6_address": "cdcd:910a:2222:5498::a9a:4f30",
        "tenant_id": "26ae5181a416420998eb2093aaed84d9",
        "create_time": "2019-01-17 11:54:48",
        "bandwidth_size": 0,
        "enterprise_project_id": "0",
        "ip_version": 6
      }
    }
    ```


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

