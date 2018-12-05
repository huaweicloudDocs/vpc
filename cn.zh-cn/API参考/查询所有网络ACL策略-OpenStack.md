# 查询所有网络ACL策略<a name="ZH-CN_TOPIC_0060574382"></a>

## 功能介绍<a name="section836818132340"></a>

查询提交请求的租户有权限操作的所有网络ACL策略信息。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section20177217132340"></a>

GET /v2.0/fwaas/firewall\_policies

## 请求消息<a name="section49464339132340"></a>

无。

## 响应消息<a name="section60203718132340"></a>

**表 1**  响应参数

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
<td class="cellrowborder" valign="top" width="17.78%" headers="mcps1.2.4.1.2 "><p id="p39042021132340"><a name="p39042021132340"></a><a name="p39042021132340"></a>List(firewall policy)</p>
</td>
<td class="cellrowborder" valign="top" width="58.89%" headers="mcps1.2.4.1.3 "><p id="p50197883132340"><a name="p50197883132340"></a><a name="p50197883132340"></a>firewall policy对象列表，参见<a href="网络ACL简介-OpenStack.md#table17002720121127">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section35216218132340"></a>

请求样例

```
GET /v2.0/fwaas/firewall_policies
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

