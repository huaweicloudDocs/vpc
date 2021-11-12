# 移除网络ACL规则<a name="vpc_firewall_0012"></a>

## 功能介绍<a name="section9946367132633"></a>

从某一网络ACL策略中移除一条网络ACL规则。

## 调试<a name="section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=NeutronRemoveFirewallRule)中直接运行调试该接口。

## URI<a name="section17986671132633"></a>

PUT /v2.0/fwaas/firewall\_policies/\{firewall\_policy\_id\}/remove\_rule

## 请求消息<a name="section27028167132633"></a>

**表 1**  请求参数

<a name="table48893916132633"></a>
<table><thead align="left"><tr id="row19661564132633"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="p4257277132633"><a name="p4257277132633"></a><a name="p4257277132633"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p2994165132633"><a name="p2994165132633"></a><a name="p2994165132633"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p47550467132633"><a name="p47550467132633"></a><a name="p47550467132633"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p38031689132633"><a name="p38031689132633"></a><a name="p38031689132633"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row26905318132633"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p23736314132633"><a name="p23736314132633"></a><a name="p23736314132633"></a>firewall_rule_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p25366437132633"><a name="p25366437132633"></a><a name="p25366437132633"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p36656390132633"><a name="p36656390132633"></a><a name="p36656390132633"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p48236351132633"><a name="p48236351132633"></a><a name="p48236351132633"></a><span id="text1243515538481"><a name="text1243515538481"></a><a name="text1243515538481"></a>网络ACL</span><span id="text6435105344819"><a name="text6435105344819"></a><a name="text6435105344819"></a></span>规则唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section14889742132633"></a>

**表 2**  响应参数

<a name="table7711269132633"></a>
<table><thead align="left"><tr id="row40961108132633"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.4.1.1"><p id="p53016887132633"><a name="p53016887132633"></a><a name="p53016887132633"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.61%" id="mcps1.2.4.1.2"><p id="p45522129132633"><a name="p45522129132633"></a><a name="p45522129132633"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.22%" id="mcps1.2.4.1.3"><p id="p31582377132633"><a name="p31582377132633"></a><a name="p31582377132633"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18215720132633"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p64319710132633"><a name="p64319710132633"></a><a name="p64319710132633"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p20101354132633"><a name="p20101354132633"></a><a name="p20101354132633"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p41635977132633"><a name="p41635977132633"></a><a name="p41635977132633"></a>对policy的描述信息</p>
</td>
</tr>
<tr id="row7244977132633"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p35103306132633"><a name="p35103306132633"></a><a name="p35103306132633"></a>audited</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p14021835132633"><a name="p14021835132633"></a><a name="p14021835132633"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p34631936132633"><a name="p34631936132633"></a><a name="p34631936132633"></a>每次policy或者它相关的rule有变动，该参数将会被置为False</p>
</td>
</tr>
<tr id="row21094728132633"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p50715789132633"><a name="p50715789132633"></a><a name="p50715789132633"></a>firewall_rules</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p56483400132633"><a name="p56483400132633"></a><a name="p56483400132633"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p3804581132633"><a name="p3804581132633"></a><a name="p3804581132633"></a>与当前policy相关联的rule的ID列表</p>
</td>
</tr>
<tr id="row27264529132633"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p47093833132633"><a name="p47093833132633"></a><a name="p47093833132633"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p45736328132633"><a name="p45736328132633"></a><a name="p45736328132633"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p46737820132633"><a name="p46737820132633"></a><a name="p46737820132633"></a>policy ID</p>
</td>
</tr>
<tr id="row46882287132633"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p28861411132633"><a name="p28861411132633"></a><a name="p28861411132633"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p36587630132633"><a name="p36587630132633"></a><a name="p36587630132633"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p14824904132633"><a name="p14824904132633"></a><a name="p14824904132633"></a>Policy名称</p>
</td>
</tr>
<tr id="row64601479132633"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p61245310132633"><a name="p61245310132633"></a><a name="p61245310132633"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p21782173132633"><a name="p21782173132633"></a><a name="p21782173132633"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p9188558132633"><a name="p9188558132633"></a><a name="p9188558132633"></a>如果为True，该policy对于其他项目<span id="text983811810491"><a name="text983811810491"></a><a name="text983811810491"></a>网络ACL</span><span id="text783878124916"><a name="text783878124916"></a><a name="text783878124916"></a></span>策略可见， 默认不可见</p>
</td>
</tr>
<tr id="row31674173132633"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p49506560132633"><a name="p49506560132633"></a><a name="p49506560132633"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p50877818132633"><a name="p50877818132633"></a><a name="p50877818132633"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row9718201825319"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p12424739135216"><a name="p12424739135216"></a><a name="p12424739135216"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="25.61%" headers="mcps1.2.4.1.2 "><p id="p1433100105317"><a name="p1433100105317"></a><a name="p1433100105317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.22%" headers="mcps1.2.4.1.3 "><p id="p83360145317"><a name="p83360145317"></a><a name="p83360145317"></a>项目ID</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section48445237132633"></a>

请求样例

```
PUT https://{Endpoint}/v2.0/fwaas/firewall_policies/afc52ce9-5305-4ec9-9feb-44feb8330341/remove_rule 

{
    "firewall_rule_id": "0f82b221-8cd6-44bd-9dfc-0e118fa7b6b1"
}
```

响应样例

```
{
    "description": "", 
    "firewall_rules": [
        "b8243448-cb3c-496e-851c-dadade4c161b"
    ], 
    "tenant_id": "23c8a121505047b6869edf39f3062712", 
    "public": false, 
    "id": "afc52ce9-5305-4ec9-9feb-44feb8330341", 
    "audited": false, 
    "name": "test-policy",
    "project_id": "23c8a121505047b6869edf39f3062712"
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

