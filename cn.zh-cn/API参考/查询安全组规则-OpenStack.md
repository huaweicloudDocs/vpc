# 查询安全组规则<a name="zh-cn_topic_0060595556"></a>

## 功能介绍<a name="section6306987516218"></a>

查询提交请求的租户有权限操作的所有安全组规则。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section2319473516218"></a>

GET /v2.0/security-group-rules

样例：

```
GET https://{Endpoint}/v2.0/security-group-rules?security_group_id={security_group_id}&remote_group_id={remote_group_id}&direction={direction}&remote_ip_prefix={remote_ip_prefix}&protocol={protocol}&port_range_max={port_range_max}&port_range_min={port_range_min}&ethertype={ethertype}&tenant_id ={tenant_id}
```

分页查询样例：

```
GET https://{Endpoint}/v2.0/networks?limit=2&marker=07adc044-3f21-4eeb-bd57-5e5eb6024b7f&page_reverse=False
```

## 请求消息<a name="section4004032316218"></a>

无。

## 响应消息<a name="section4154959916218"></a>

**表 1**  响应参数

<a name="table5126909016218"></a>
<table><thead align="left"><tr id="row4406312316218"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p130340816218"><a name="p130340816218"></a><a name="p130340816218"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p23005316218"><a name="p23005316218"></a><a name="p23005316218"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p1954037216218"><a name="p1954037216218"></a><a name="p1954037216218"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row25691016218"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p5925871816218"><a name="p5925871816218"></a><a name="p5925871816218"></a>security_group_rules</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p263715271607"><a name="p263715271607"></a><a name="p263715271607"></a>Array of <a href="#table655457801607">Security Group Rule</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p732393116218"><a name="p732393116218"></a><a name="p732393116218"></a>security group rule对象列表。请参见<a href="#table655457801607">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Security Group Rule对象

<a name="table655457801607"></a>
<table><thead align="left"><tr id="row54478641607"><th class="cellrowborder" valign="top" width="26.669999999999998%" id="mcps1.2.4.1.1"><p id="p389969021607"><a name="p389969021607"></a><a name="p389969021607"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.2"><p id="p36789391607"><a name="p36789391607"></a><a name="p36789391607"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="p433861031607"><a name="p433861031607"></a><a name="p433861031607"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row134774871607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p269083981607"><a name="p269083981607"></a><a name="p269083981607"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p630670281607"><a name="p630670281607"></a><a name="p630670281607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p334792201607"><a name="p334792201607"></a><a name="p334792201607"></a>安全组规则id</p>
<p id="p529374054010"><a name="p529374054010"></a><a name="p529374054010"></a>使用说明：查询安全组规则非必选</p>
</td>
</tr>
<tr id="row250554771607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p254411021607"><a name="p254411021607"></a><a name="p254411021607"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p505368621607"><a name="p505368621607"></a><a name="p505368621607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p480145951607"><a name="p480145951607"></a><a name="p480145951607"></a>安全组规则描述</p>
</td>
</tr>
<tr id="row569401671607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p115724181607"><a name="p115724181607"></a><a name="p115724181607"></a>security_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p615991711607"><a name="p615991711607"></a><a name="p615991711607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p587796621607"><a name="p587796621607"></a><a name="p587796621607"></a>所属安全组id</p>
</td>
</tr>
<tr id="row654332091607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p113008931607"><a name="p113008931607"></a><a name="p113008931607"></a>remote_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p170542961607"><a name="p170542961607"></a><a name="p170542961607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p141218971607"><a name="p141218971607"></a><a name="p141218971607"></a>所属安全组的对端id</p>
</td>
</tr>
<tr id="row9932071607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p657989401607"><a name="p657989401607"></a><a name="p657989401607"></a>direction</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p507988391607"><a name="p507988391607"></a><a name="p507988391607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p570991491607"><a name="p570991491607"></a><a name="p570991491607"></a>规则方向</p>
</td>
</tr>
<tr id="row97529031607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p478834691607"><a name="p478834691607"></a><a name="p478834691607"></a>remote_ip_prefix</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p622759951607"><a name="p622759951607"></a><a name="p622759951607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p146708701607"><a name="p146708701607"></a><a name="p146708701607"></a>对端ip网段</p>
</td>
</tr>
<tr id="row315033981607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p163656291607"><a name="p163656291607"></a><a name="p163656291607"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p628340441607"><a name="p628340441607"></a><a name="p628340441607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p99902671607"><a name="p99902671607"></a><a name="p99902671607"></a>协议类型或直接指定IP协议号</p>
</td>
</tr>
<tr id="row551583771607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p97886331607"><a name="p97886331607"></a><a name="p97886331607"></a>port_range_max</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p343603851607"><a name="p343603851607"></a><a name="p343603851607"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p188144701607"><a name="p188144701607"></a><a name="p188144701607"></a>最大端口，当协议类型为ICMP时，该值表示ICMP的code</p>
</td>
</tr>
<tr id="row456604071607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p630384091607"><a name="p630384091607"></a><a name="p630384091607"></a>port_range_min</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p337362901607"><a name="p337362901607"></a><a name="p337362901607"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p258562691607"><a name="p258562691607"></a><a name="p258562691607"></a>最小端口，当协议类型为ICMP时，该值表示ICMP的type。</p>
<p id="p5690808615417"><a name="p5690808615417"></a><a name="p5690808615417"></a>protocol为tcp和udp时，port_range_max和port_range_min必须同时输入，且port_range_max应大于等于port_range_min。</p>
<p id="p4241072615417"><a name="p4241072615417"></a><a name="p4241072615417"></a>protocol为icmp时，指定ICMP code（port_range_max）时，必须同时指定ICMP type（port_range_min）。</p>
</td>
</tr>
<tr id="row360773491607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p364292801607"><a name="p364292801607"></a><a name="p364292801607"></a>ethertype</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p339523071607"><a name="p339523071607"></a><a name="p339523071607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p34728681607"><a name="p34728681607"></a><a name="p34728681607"></a>网络类型</p>
<p id="p568898621607"><a name="p568898621607"></a><a name="p568898621607"></a>仅支持IPv4</p>
</td>
</tr>
<tr id="row532124261607"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p593368391607"><a name="p593368391607"></a><a name="p593368391607"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p130282191607"><a name="p130282191607"></a><a name="p130282191607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row11992111863317"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p169261732143314"><a name="p169261732143314"></a><a name="p169261732143314"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p69311132153317"><a name="p69311132153317"></a><a name="p69311132153317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p13646103310"><a name="p13646103310"></a><a name="p13646103310"></a>项目ID</p>
</td>
</tr>
<tr id="row10903153923318"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p6634195714335"><a name="p6634195714335"></a><a name="p6634195714335"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p12638157153319"><a name="p12638157153319"></a><a name="p12638157153319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1364635713332"><a name="p1364635713332"></a><a name="p1364635713332"></a>资源创建时间，UTC时间</p>
<p id="p65980291419"><a name="p65980291419"></a><a name="p65980291419"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
<tr id="row1797311427338"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.2.4.1.1 "><p id="p1725445103416"><a name="p1725445103416"></a><a name="p1725445103416"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="p192601514345"><a name="p192601514345"></a><a name="p192601514345"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1127018513343"><a name="p1127018513343"></a><a name="p1127018513343"></a>资源更新时间，UTC时间</p>
<p id="p19850105451210"><a name="p19850105451210"></a><a name="p19850105451210"></a>格式：yyyy-MM-ddTHH:mm:ss</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section2229785216218"></a>

请求样例

```
GET https://{Endpoint}/v2.0/security-group-rules
```

响应样例

```
{
    "security_group_rules": [
        {
            "remote_group_id": "1d8b19c7-7c56-48f7-a99b-4b40eb390967", 
            "direction": "ingress", 
            "remote_ip_prefix": null, 
            "protocol": null, 
            "tenant_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "port_range_max": null, 
            "security_group_id": "1d8b19c7-7c56-48f7-a99b-4b40eb390967", 
            "port_range_min": null, 
            "ethertype": "IPv6", 
            "description": null, 
            "id": "07adc044-3f21-4eeb-bd57-5e5eb6024b7f",
            "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "created_at": "2018-09-20T02:15:34",
            "updated_at": "2018-09-20T02:15:34"
        }, 
        {
            "remote_group_id": null, 
            "direction": "egress", 
            "remote_ip_prefix": null, 
            "protocol": null, 
            "tenant_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "port_range_max": null, 
            "security_group_id": "328fb454-a2ee-4a11-bdb1-ee19bbdfde43", 
            "port_range_min": null, 
            "ethertype": "IPv6", 
            "description": null, 
            "id": "09358f83-f4a5-4386-9563-a1e3c373d655",
            "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "created_at": "2018-09-20T02:15:34",
            "updated_at": "2018-09-20T02:15:34"
        }, 
        {
            "remote_group_id": "4c763030-366e-428c-be2b-d48f6baf5297", 
            "direction": "ingress", 
            "remote_ip_prefix": null, 
            "protocol": null, 
            "tenant_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "port_range_max": null, 
            "security_group_id": "4c763030-366e-428c-be2b-d48f6baf5297", 
            "port_range_min": null, 
            "ethertype": "IPv6", 
            "description": null, 
            "id": "219a6f56-1069-458b-bec0-df9270e7a074",
            "project_id": "6c9298ec8c874f7f99688489ab65f90e", 
            "created_at": "2018-09-20T02:15:34",
            "updated_at": "2018-09-20T02:15:34"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

