# 管理弹性公网IP地址标签<a name="zh-cn_topic_0068145818"></a>

## 操作场景<a name="section51463883214456"></a>

为弹性公网IP地址添加标签，可以方便用户识别和管理拥有的弹性公网IP地址。您可以在申请弹性公网IP地址时增加标签，或者在已经创建的弹性公网IP地址详情页添加标签，最多可以给弹性公网IP地址添加10个标签。

标签共由两部分组成：“键”和“值”，其中，“键”和“值”的命名规则如[表1](#ted9687ca14074ef785241145365a6175)所示。

**表 1**  弹性公网IP地址标签命名规则

<a name="ted9687ca14074ef785241145365a6175"></a>
<table><thead align="left"><tr id="rd57708e01e6443a9805ca72f554fae7f"><th class="cellrowborder" valign="top" width="18.54%" id="mcps1.2.4.1.1"><p id="abc7708d69440476086850b219c70efa8"><a name="abc7708d69440476086850b219c70efa8"></a><a name="abc7708d69440476086850b219c70efa8"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="53.39%" id="mcps1.2.4.1.2"><p id="a0df2f83c3277432ab05b525e4ffb1c2c"><a name="a0df2f83c3277432ab05b525e4ffb1c2c"></a><a name="a0df2f83c3277432ab05b525e4ffb1c2c"></a>规则</p>
</th>
<th class="cellrowborder" valign="top" width="28.07%" id="mcps1.2.4.1.3"><p id="a902e732241f94e96b0b1b718cf7ed639"><a name="a902e732241f94e96b0b1b718cf7ed639"></a><a name="a902e732241f94e96b0b1b718cf7ed639"></a>样例</p>
</th>
</tr>
</thead>
<tbody><tr id="r95612b479088487b99e620f90b71f798"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="a7694a48138124d1daf3804556a27bfd6"><a name="a7694a48138124d1daf3804556a27bfd6"></a><a name="a7694a48138124d1daf3804556a27bfd6"></a>键</p>
</td>
<td class="cellrowborder" valign="top" width="53.39%" headers="mcps1.2.4.1.2 "><a name="uac40e19ce4ac49d0913d48b334564c45"></a><a name="uac40e19ce4ac49d0913d48b334564c45"></a><ul id="uac40e19ce4ac49d0913d48b334564c45"><li>不能为空。</li><li>对于同一弹性公网IP地址键值唯一。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.3 "><p id="a1a10de6d67c04555a3508a8cdc3500e7"><a name="a1a10de6d67c04555a3508a8cdc3500e7"></a><a name="a1a10de6d67c04555a3508a8cdc3500e7"></a>Ipv4_key1</p>
</td>
</tr>
<tr id="r32a79d8bde844fda8a6254383317e58f"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="a1ebd1dda592448d49631c7f099519113"><a name="a1ebd1dda592448d49631c7f099519113"></a><a name="a1ebd1dda592448d49631c7f099519113"></a>值</p>
</td>
<td class="cellrowborder" valign="top" width="53.39%" headers="mcps1.2.4.1.2 "><a name="uaf17b1ea9b9a4e58b95cafefa2898283"></a><a name="uaf17b1ea9b9a4e58b95cafefa2898283"></a><ul id="uaf17b1ea9b9a4e58b95cafefa2898283"><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="28.07%" headers="mcps1.2.4.1.3 "><p id="a21a035aeb72143f5ab0fd45a08248d08"><a name="a21a035aeb72143f5ab0fd45a08248d08"></a><a name="a21a035aeb72143f5ab0fd45a08248d08"></a>192.168.12.10</p>
</td>
</tr>
</tbody>
</table>

## 操作步骤<a name="section4374728222113"></a>

**在弹性公网IP列表页，按标签的键或值搜索目标弹性公网IP地址。**

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，选择“网络 \> 弹性公网IP”。
4.  单击弹性公网IP地址列表右上角的“标签搜索”，展开查询页。
5.  输入待查询弹性公网IP地址的标签值。

    键和值均不能为空，当键和值全匹配时，系统可以自动查询到目标弹性公网IP地址。

6.  单击“+”，添加输入的标签值。

    系统支持添加多个标签值，并取各个标签值的交集，对目标弹性公网IP地址进行搜索。

7.  单击“搜索”。

    系统根据标签的键和值搜索目标弹性公网IP地址。


**在弹性公网IP地址的标签页，执行标签的增、删、改、查操作。**

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region.png)，选择区域和项目。
3.  在系统首页，选择“网络 \> 弹性公网IP”。
4.  在弹性公网IP地址列表中，单击待管理标签的弹性公网IP地址名称。
5.  在弹性公网IP地址详情页面，选择“标签”页签，对弹性公网IP地址的标签执行增、删、改、查。
    -   查看

        在“标签”页，可以查看当前弹性公网IP地址的标签详情，包括标签个数，以及每个标签的键和值。

    -   添加

        单击左上角的“添加标签”，在弹出的“添加标签”窗口，输入新添加标签的键和值，并单击“确定”。

    -   修改

        单击标签所在行“操作”列下的“编辑”，在弹出的“编辑标签”窗口，输入修改后标签的键和值，并单击“确定”。

    -   删除

        单击标签所在行“操作”列下的“删除”，如果确认删除，在弹出的“删除标签”窗口，单击“是”。



