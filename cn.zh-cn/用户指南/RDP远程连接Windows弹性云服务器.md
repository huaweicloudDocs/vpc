# RDP远程连接Windows弹性云服务器<a name="SecurityGroup_0010"></a>

-   场景举例：

    创建好Windows弹性云服务器后，为了通过RDP远程连接弹性云服务器，您可以添加安全组规则。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >默认安全组中已经配置了该条规则，如您使用默认安全组，无需重复配置。  

-   安全组配置方法：

    <a name="table129650323711"></a>
    <table><thead align="left"><tr id="row145116433715"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.5.1.1"><p id="p165113443717"><a name="p165113443717"></a><a name="p165113443717"></a>协议</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.1.5.1.2"><p id="p155113453713"><a name="p155113453713"></a><a name="p155113453713"></a>方向</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.5.1.3"><p id="p155214163719"><a name="p155214163719"></a><a name="p155214163719"></a>端口范围</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.1.5.1.4"><p id="p952142371"><a name="p952142371"></a><a name="p952142371"></a>源地址</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row18528416375"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.5.1.1 "><p id="p452446375"><a name="p452446375"></a><a name="p452446375"></a>RDP（3389）</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.1.5.1.2 "><p id="p8521445370"><a name="p8521445370"></a><a name="p8521445370"></a>入方向</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.5.1.3 "><p id="p125215413371"><a name="p125215413371"></a><a name="p125215413371"></a>3389</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.1.5.1.4 "><p id="p155219414376"><a name="p155219414376"></a><a name="p155219414376"></a>0.0.0.0/0</p>
    </td>
    </tr>
    </tbody>
    </table>


