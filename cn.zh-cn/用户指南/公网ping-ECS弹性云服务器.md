# 公网ping ECS弹性云服务器<a name="SecurityGroup_0011"></a>

-   场景举例：

    创建好弹性云服务器后，为了使用ping程序测试弹性云服务器之间的通讯状况，您需要添加安全组规则。

-   安全组配置方法：

    <a name="table810055173719"></a>
    <table><thead align="left"><tr id="row0160051103719"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.5.1.1"><p id="p141601751113715"><a name="p141601751113715"></a><a name="p141601751113715"></a>协议</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.1.5.1.2"><p id="p2160251153718"><a name="p2160251153718"></a><a name="p2160251153718"></a>方向</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.5.1.3"><p id="p14160165111379"><a name="p14160165111379"></a><a name="p14160165111379"></a>端口范围</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.1.5.1.4"><p id="p161601651183720"><a name="p161601651183720"></a><a name="p161601651183720"></a>源地址</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1216175110371"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.5.1.1 "><p id="p816119517376"><a name="p816119517376"></a><a name="p816119517376"></a>ICMP</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.1.5.1.2 "><p id="p5161175117373"><a name="p5161175117373"></a><a name="p5161175117373"></a>入方向</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.5.1.3 "><p id="p11161205112375"><a name="p11161205112375"></a><a name="p11161205112375"></a>All</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.1.5.1.4 "><p id="p1316155143713"><a name="p1316155143713"></a><a name="p1316155143713"></a>0.0.0.0/0</p>
    </td>
    </tr>
    </tbody>
    </table>


