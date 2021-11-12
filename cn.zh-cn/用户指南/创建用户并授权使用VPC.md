# 创建用户并授权使用VPC<a name="permission_0003"></a>

如果您需要对您所拥有的VPC进行精细的权限管理，您可以使用统一身份认证服务（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云帐号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用VPC资源。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将VPC资源委托给更专业、高效的其他华为云帐号或者云服务，这些帐号或者云服务可以根据权限进行代运维。

如果华为云帐号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用VPC服务的其他功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#fig1447123814172)所示。

## 前提条件<a name="section6808937111712"></a>

给用户组授权之前，请您了解用户组可以添加的VPC系统权限，并结合实际需求进行选择，VPC支持的系统权限，请参见：[VPC系统策略](https://support.huaweicloud.com/productdesc-vpc/overview_permission.html)。若您需要对除VPC之外的其他服务授权，IAM支持服务的所有策略请参见[权限策略](https://support.huaweicloud.com/usermanual-permissions/iam_01_0001.html)。

## 示例流程<a name="section197617372174"></a>

**图 1**  给用户授权VPC权限流程<a name="fig1447123814172"></a>  
![](figures/给用户授权VPC权限流程.png "给用户授权VPC权限流程")

1.  <a name="li8447183891715"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/iam_03_0001.html)

    在IAM控制台创建用户组，并授予VPC只读权限“VPC ReadOnlyAccess”。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/iam_02_0001.html)

    在IAM控制台创建用户，并将其加入[1.创建用户组并授权](#li8447183891715)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，切换至授权区域，验证权限：

    -   在“服务列表”中选择虚拟私有云，进入VPC主界面，单击右上角“创建虚拟私有云”，如果无法创建虚拟私有云（假设当前权限仅包含VPC ReadOnlyAccess），表示“VPC ReadOnlyAccess”已生效。
    -   在“服务列表”中选择除虚拟私有云外（假设当前策略仅包含ECS Viewer）的任一服务，若提示权限不足，表示“VPC ReadOnlyAccess”已生效。


