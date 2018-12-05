# SSH远程连接Linux弹性云服务器<a name="SecurityGroup_0009"></a>

-   场景举例：

    创建好Linux弹性云服务器后，为了通过SSH远程连接到弹性云服务器，您可以添加安全组规则。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >默认安全组中已经配置了该条规则，如您使用默认安全组，无需重复配置。  

-   安全组配置方法：

    <a name="table46033413216"></a>
    <table><thead align="left"><tr id="row566213473212"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.5.1.1"><p id="p146625493212"><a name="p146625493212"></a><a name="p146625493212"></a>协议</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.1.5.1.2"><p id="p26621548329"><a name="p26621548329"></a><a name="p26621548329"></a>方向</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.5.1.3"><p id="p176659413329"><a name="p176659413329"></a><a name="p176659413329"></a>端口范围</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.1.5.1.4"><p id="p76655483218"><a name="p76655483218"></a><a name="p76655483218"></a>源地址</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row156650473218"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.5.1.1 "><p id="p10666174203214"><a name="p10666174203214"></a><a name="p10666174203214"></a>SSH（22）</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.1.5.1.2 "><p id="p1566654143218"><a name="p1566654143218"></a><a name="p1566654143218"></a>入方向</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.5.1.3 "><p id="p1266684163219"><a name="p1266684163219"></a><a name="p1266684163219"></a>22</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.1.5.1.4 "><p id="p26661844324"><a name="p26661844324"></a><a name="p26661844324"></a>0.0.0.0/0</p>
    </td>
    </tr>
    </tbody>
    </table>


