# 创建VPC<a name="vpc_apieg_0001"></a>

## 操作场景<a name="section138381652181710"></a>

本节通过调用VPC创建接口来创建一个VPC。创建VPC的API参数说明及响应信息请参见[创建VPC](vpc-创建VPC.md)。

## 前提条件<a name="section109541355172116"></a>

您需要规划VPC所在的区域信息，并根据区域确定调用API的Endpoint，详细信息请参见[终端节点](终端节点.md)。

当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。Token认证，具体操作请参考[认证鉴权](认证鉴权.md)。

>![](public_sys-resources/icon-note.gif) **说明：**   
>通过IAM服务获取到的Token有效期为24小时，需要使用同一个Token鉴权时，可以先将Token缓存，避免频繁调用。  

## 操作步骤<a name="section7856948"></a>

1.  发送“POST  https://VPC的Endpoint/v1/\{project\_id\}/vpcs”，project\_id为项目ID。
2.  在Request Header中增加“X-Auth-Token”。
3.  在Request Body中传入参数如下：

    ```
    {
        "vpc": {
            "name": "vpc", //虚拟私有云名称
            "cidr": "192.168.0.0/16" //虚拟私有云下可用子网的范围
        }
    }
    ```

4.  查看请求响应结果。
    -   请求成功时，响应参数如下，id就是vpc\_id。

        ```
        {
            "vpc": {
                "id": "b6684a27-b049-407d-90b4-c9551f2390e1",
                "name": "vpc",
                "cidr": "192.168.0.0/16",
                "status": "CREATING",
                "routes": []
            }
        }
        ```

    -   请求异常时，错误码请参见[错误码](错误码.md)。

5.  根据vpc\_id和project\_id可以查询VPC详情，更新或删除VPC。

