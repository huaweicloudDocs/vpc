# 仅允许特定 IP 地址远程连接弹性云服务器<a name="SecurityGroup_0008"></a>

-   场景举例：

    为了防止弹性云服务器被网络攻击，用户可以修改远程登录端口号，并设置安全组规则只允许特定的IP地址远程登录到弹性云服务器。

-   安全组配置方法：

    以仅允许特定IP地址（例如，192.168.20.2）通过SSH协议访问Linux操作系统的弹性云服务器的22端口为例，安全组规则如下所示。

    <a name="table2497622119555"></a>
    <table><thead align="left"><tr id="row407563919555"><th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.1.5.1.1"><p id="p6169135719555"><a name="p6169135719555"></a><a name="p6169135719555"></a>协议</p>
    </th>
    <th class="cellrowborder" valign="top" width="10.891089108910892%" id="mcps1.1.5.1.2"><p id="p3094402719555"><a name="p3094402719555"></a><a name="p3094402719555"></a>方向</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.1.5.1.3"><p id="p2343829819555"><a name="p2343829819555"></a><a name="p2343829819555"></a>端口范围</p>
    </th>
    <th class="cellrowborder" valign="top" width="64.35643564356435%" id="mcps1.1.5.1.4"><p id="p1945401819555"><a name="p1945401819555"></a><a name="p1945401819555"></a>源地址</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3227161019555"><td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.1.5.1.1 "><p id="p6386359419555"><a name="p6386359419555"></a><a name="p6386359419555"></a>SSH（22）</p>
    </td>
    <td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.1.5.1.2 "><p id="p556863519555"><a name="p556863519555"></a><a name="p556863519555"></a>入方向</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.1.5.1.3 "><p id="p4840629219555"><a name="p4840629219555"></a><a name="p4840629219555"></a>22</p>
    </td>
    <td class="cellrowborder" valign="top" width="64.35643564356435%" headers="mcps1.1.5.1.4 "><p id="p2859561419555"><a name="p2859561419555"></a><a name="p2859561419555"></a>IPv4地址、IPv4 CIDR或者另一个安全组的ID。</p>
    <p id="p62410334191747"><a name="p62410334191747"></a><a name="p62410334191747"></a>例如：192.168.20.2</p>
    </td>
    </tr>
    </tbody>
    </table>


