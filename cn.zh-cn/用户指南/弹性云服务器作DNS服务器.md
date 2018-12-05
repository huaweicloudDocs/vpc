# 弹性云服务器作DNS服务器<a name="SecurityGroup_0013"></a>

-   场景举例：

    如果您将弹性云服务器设置为DNS服务器，则必须确保TCP和UDP数据可通过53端口访问您的DNS服务器。您需要在弹性云服务器所在安全组中添加以下安全组规则。

-   安全组配置方法：

    <a name="table30323767195135"></a>
    <table><thead align="left"><tr id="row15770184195135"><th class="cellrowborder" valign="top" width="28.93%" id="mcps1.1.5.1.1"><p id="p2316559195135"><a name="p2316559195135"></a><a name="p2316559195135"></a>协议</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.27%" id="mcps1.1.5.1.2"><p id="p53423553195135"><a name="p53423553195135"></a><a name="p53423553195135"></a>方向</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.349999999999998%" id="mcps1.1.5.1.3"><p id="p32340552195135"><a name="p32340552195135"></a><a name="p32340552195135"></a>端口范围</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.45%" id="mcps1.1.5.1.4"><p id="p2339084195135"><a name="p2339084195135"></a><a name="p2339084195135"></a>源地址</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row55248116195135"><td class="cellrowborder" valign="top" width="28.93%" headers="mcps1.1.5.1.1 "><p id="p45912425195135"><a name="p45912425195135"></a><a name="p45912425195135"></a>TCP</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.27%" headers="mcps1.1.5.1.2 "><p id="p27918930195135"><a name="p27918930195135"></a><a name="p27918930195135"></a>入方向</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.349999999999998%" headers="mcps1.1.5.1.3 "><p id="p46840856195135"><a name="p46840856195135"></a><a name="p46840856195135"></a>53</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.45%" headers="mcps1.1.5.1.4 "><p id="p36012962195135"><a name="p36012962195135"></a><a name="p36012962195135"></a>0.0.0.0/0</p>
    </td>
    </tr>
    <tr id="row5566305020026"><td class="cellrowborder" valign="top" width="28.93%" headers="mcps1.1.5.1.1 "><p id="p3120540920026"><a name="p3120540920026"></a><a name="p3120540920026"></a>UDP</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.27%" headers="mcps1.1.5.1.2 "><p id="p4461017620026"><a name="p4461017620026"></a><a name="p4461017620026"></a>入方向</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.349999999999998%" headers="mcps1.1.5.1.3 "><p id="p5665449220026"><a name="p5665449220026"></a><a name="p5665449220026"></a>53</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.45%" headers="mcps1.1.5.1.4 "><p id="p2561110020026"><a name="p2561110020026"></a><a name="p2561110020026"></a>0.0.0.0/0</p>
    </td>
    </tr>
    </tbody>
    </table>


