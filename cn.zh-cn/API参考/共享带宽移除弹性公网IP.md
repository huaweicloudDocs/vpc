# 共享带宽移除弹性公网IP<a name="ZH-CN_TOPIC_0201534216"></a>

## 功能介绍<a name="section16581154"></a>

共享带宽移除弹性公网IP。

## URI<a name="section15012662"></a>

POST /v2.0/\{project\_id\}/bandwidths/\{bandwidth\_id\}/remove

参数说明请参见[表1](#table25281875)。

**表 1**  参数说明

<a name="table25281875"></a>
<table><thead align="left"><tr id="row26712487"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p16227847"><a name="p16227847"></a><a name="p16227847"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p39387211"><a name="p39387211"></a><a name="p39387211"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p36247516"><a name="p36247516"></a><a name="p36247516"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row50367649"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p53247746"><a name="p53247746"></a><a name="p53247746"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p18100201"><a name="p18100201"></a><a name="p18100201"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row41709209"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p23002745"><a name="p23002745"></a><a name="p23002745"></a>bandwidth_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p51283066"><a name="p51283066"></a><a name="p51283066"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p60287683"><a name="p60287683"></a><a name="p60287683"></a>带宽唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section896237"></a>

-   请求参数

    **表 2**  请求参数

    <a name="table3057854815556"></a>
    <table><thead align="left"><tr id="row6286666315556"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="p5903494715556"><a name="p5903494715556"></a><a name="p5903494715556"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="p1710139915556"><a name="p1710139915556"></a><a name="p1710139915556"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="p4303610815556"><a name="p4303610815556"></a><a name="p4303610815556"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.18%" id="mcps1.2.5.1.4"><p id="p6337274615556"><a name="p6337274615556"></a><a name="p6337274615556"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3291877615556"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="p4917516615556"><a name="p4917516615556"></a><a name="p4917516615556"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="p2376550915556"><a name="p2376550915556"></a><a name="p2376550915556"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="p4595806815556"><a name="p4595806815556"></a><a name="p4595806815556"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="p1610901815556"><a name="p1610901815556"></a><a name="p1610901815556"></a>带宽对象，请参见<a href="#table31854691">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  bandwidth字段说明

    <a name="table31854691"></a>
    <table><thead align="left"><tr id="row6882862"><th class="cellrowborder" valign="top" width="13.350000000000001%" id="mcps1.2.5.1.1"><p id="p20640979"><a name="p20640979"></a><a name="p20640979"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.91%" id="mcps1.2.5.1.2"><p id="p61306625"><a name="p61306625"></a><a name="p61306625"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.91%" id="mcps1.2.5.1.3"><p id="p5200653172316"><a name="p5200653172316"></a><a name="p5200653172316"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.830000000000005%" id="mcps1.2.5.1.4"><p id="p66889567"><a name="p66889567"></a><a name="p66889567"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row49345813"><td class="cellrowborder" valign="top" width="13.350000000000001%" headers="mcps1.2.5.1.1 "><p id="p37587916"><a name="p37587916"></a><a name="p37587916"></a>publicip_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.2 "><p id="p24722347"><a name="p24722347"></a><a name="p24722347"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.3 "><p id="p18599757172316"><a name="p18599757172316"></a><a name="p18599757172316"></a>Array of <a href="#table30936422">publicip_info</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.830000000000005%" headers="mcps1.2.5.1.4 "><a name="ul290995117818"></a><a name="ul290995117818"></a><ul id="ul290995117818"><li>功能说明：要从共享带宽中移除的弹性公网IP信息，请参见<a href="#table30936422">表4</a>。</li><li>约束：WHOLE类型的带宽支持多个弹性公网IP，跟租户的配额相关，默认一个共享带宽的配额为20。</li></ul>
    </td>
    </tr>
    <tr id="row193703372412"><td class="cellrowborder" valign="top" width="13.350000000000001%" headers="mcps1.2.5.1.1 "><p id="p183711037154117"><a name="p183711037154117"></a><a name="p183711037154117"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.2 "><p id="p17371237114118"><a name="p17371237114118"></a><a name="p17371237114118"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.3 "><p id="p15371143714413"><a name="p15371143714413"></a><a name="p15371143714413"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.830000000000005%" headers="mcps1.2.5.1.4 "><p id="p877125719190"><a name="p877125719190"></a><a name="p877125719190"></a>弹性公网IP从共享带宽移除后，会为此弹性公网IP创建独占带宽进行计费。</p>
    <p id="p29217211425"><a name="p29217211425"></a><a name="p29217211425"></a>此参数表示弹性公网IP从共享带宽移除后，使用的独占带宽的计费类型。</p>
    <p id="p179232117423"><a name="p179232117423"></a><a name="p179232117423"></a>（bandwidth/traffic）</p>
    </td>
    </tr>
    <tr id="row1125210414413"><td class="cellrowborder" valign="top" width="13.350000000000001%" headers="mcps1.2.5.1.1 "><p id="p1425214412410"><a name="p1425214412410"></a><a name="p1425214412410"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.2 "><p id="p1525210418416"><a name="p1525210418416"></a><a name="p1525210418416"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.3 "><p id="p7252164114118"><a name="p7252164114118"></a><a name="p7252164114118"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.830000000000005%" headers="mcps1.2.5.1.4 "><p id="p42481825142019"><a name="p42481825142019"></a><a name="p42481825142019"></a>弹性公网IP从共享带宽移除后，会为此弹性公网IP创建独占带宽进行计费。</p>
    <p id="p16249725152011"><a name="p16249725152011"></a><a name="p16249725152011"></a>此参数表示弹性公网IP从共享带宽移除后，使用的独占带宽的带宽大小。（M）</p>
    <p id="p721494415220"><a name="p721494415220"></a><a name="p721494415220"></a>取值范围：默认为1Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  publicip\_info对象

    <a name="table30936422"></a>
    <table><thead align="left"><tr id="row17161430"><th class="cellrowborder" valign="top" width="13.3%" id="mcps1.2.5.1.1"><p id="p47898561"><a name="p47898561"></a><a name="p47898561"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.02%" id="mcps1.2.5.1.2"><p id="p157089251981"><a name="p157089251981"></a><a name="p157089251981"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.96%" id="mcps1.2.5.1.3"><p id="p2828296517154"><a name="p2828296517154"></a><a name="p2828296517154"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.72%" id="mcps1.2.5.1.4"><p id="p58761073"><a name="p58761073"></a><a name="p58761073"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row62026502"><td class="cellrowborder" valign="top" width="13.3%" headers="mcps1.2.5.1.1 "><p id="p58090788"><a name="p58090788"></a><a name="p58090788"></a>publicip_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.02%" headers="mcps1.2.5.1.2 "><p id="p10708102514810"><a name="p10708102514810"></a><a name="p10708102514810"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.2.5.1.3 "><p id="p921881117154"><a name="p921881117154"></a><a name="p921881117154"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.72%" headers="mcps1.2.5.1.4 "><p id="p476380"><a name="p476380"></a><a name="p476380"></a>带宽对应的弹性公网IP的唯一标识</p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    POST https://{Endpoint}/v2.0/{project_id}/bandwidths/{bandwidth_id}/remove
    
    {
        "bandwidth": {
            "publicip_info": [
                {
                    "publicip_id": "d91b0028-6f6b-4478-808a-297b75b6812a"
     
                },
                {
                    "publicip_id": "1d184b2c-4ec9-49b5-a3f9-27600a76ba3f"
                }
            ],
            "charge_mode": "traffic",
            "size": 22
        }
    }
    ```


## 响应消息<a name="section8066134"></a>

-   响应参数

    无

-   响应样例

    无


## 状态码<a name="section31981619"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参考[错误码](错误码.md)。

