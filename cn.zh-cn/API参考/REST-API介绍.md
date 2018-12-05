# REST API介绍<a name="ZH-CN_TOPIC_0132456728"></a>

第三方应用对公有云API的访问需经过签名认证。

公有云API符合RESTful API的设计理论。

REST从资源的角度来观察整个网络，提供创建、查询、更新、删掉等方法访问服务的资源。

REST API请求/响应对可以分为如下部分：

-   请求URI
-   请求消息头
-   请求消息体
-   响应消息头
-   响应消息体

## 请求URI<a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_section697653216219"></a>

请求URI由如下部分组成：

**\{URI-scheme\}://\{Endpoint\}/\{resource-path\}?\{query-string\}**

尽管请求URI包含在请求消息头中，但大多数语言或框架都要求您从请求消息中单独传递它，所有我们在此单独拿出来强调。

**表 1**  URI中的参数说明

<a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_table4443194632512"></a>
<table><thead align="left"><tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row1944414616258"><th class="cellrowborder" valign="top" width="26%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1644484692510"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1644484692510"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1644484692510"></a><strong id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b2015193132620"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b2015193132620"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b2015193132620"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="74%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p174441146142511"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p174441146142511"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p174441146142511"></a><strong id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b131565362615"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b131565362615"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b131565362615"></a>描述</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row10444144620259"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p154446465251"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p154446465251"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p154446465251"></a>URI-scheme</p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p8444144692517"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p8444144692517"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p8444144692517"></a>表示用于传输请求的协议。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row444414692513"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p7444194610257"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p7444194610257"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p7444194610257"></a>Endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p244474613259"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p244474613259"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p244474613259"></a>指定承载REST服务端点的服务器域名或IP，从<a href="http://developer.huaweicloud.com/dev/endpoint" target="_blank" rel="noopener noreferrer">地区和终端节点</a>获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row1744454612520"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p14442468257"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p14442468257"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p14442468257"></a>resource-path</p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1844412467258"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1844412467258"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1844412467258"></a>资源路径，也即API访问路径。从具体接口的URI模块获取，例如“v3/auth/tokens”。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row184441346152515"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p4444154692516"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p4444154692516"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p4444154692516"></a>query-string</p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1444414622514"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1444414622514"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1444414622514"></a>可选参数，例如API版本或资源选择标准。</p>
</td>
</tr>
</tbody>
</table>

## 请求方法<a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_section5296154118345"></a>

HTTP方法（也称为操作或动词），它告诉服务你正在请求什么类型的操作。

**表 2**  HTTP方法

<a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_table1961229113819"></a>
<table><thead align="left"><tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row86141913816"><th class="cellrowborder" valign="top" width="30%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p186147910387"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p186147910387"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p186147910387"></a><strong id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b1093312238395"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b1093312238395"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b1093312238395"></a>方法</strong></p>
</th>
<th class="cellrowborder" valign="top" width="70%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p166141293387"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p166141293387"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p166141293387"></a><strong id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b169341023133919"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b169341023133919"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b169341023133919"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row146141194381"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p12831539123914"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p12831539123914"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p12831539123914"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p2831123916397"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p2831123916397"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p2831123916397"></a>请求服务器返回指定资源。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row161429103817"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p3831239183912"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p3831239183912"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p3831239183912"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p178311939193911"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p178311939193911"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p178311939193911"></a>请求服务器更新指定资源。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row56141190384"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p68311239113912"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p68311239113912"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p68311239113912"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1583133918391"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1583133918391"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1583133918391"></a>请求服务器新增资源或执行特殊操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row861411903812"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1183153943916"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1183153943916"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1183153943916"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p6831163914392"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p6831163914392"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p6831163914392"></a>请求服务器删除指定资源，如删除对象等。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row5614119183810"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p78314395393"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p78314395393"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p78314395393"></a>HEAD</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p38311239153920"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p38311239153920"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p38311239153920"></a>请求服务器资源头部。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_row2614199163812"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1483143915390"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1483143915390"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p1483143915390"></a>PATCH</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p17831173918394"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p17831173918394"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p17831173918394"></a>请求服务器更新资源的部分内容。</p>
<p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p9831123911390"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p9831123911390"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_p9831123911390"></a>当资源不存在的时候，PATCH可能会去创建一个新的资源。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息头<a name="zh-cn_topic_0121682347_section479119143310"></a>

可选的附加请求头字段，如指定的URI和HTTP方法所要求的字段。详细的公共请求消息头字段请参见[表3](#zh-cn_topic_0121682347_table1986821153312)。

**表 3**  公共请求消息头

<a name="zh-cn_topic_0121682347_table1986821153312"></a>
<table><thead align="left"><tr id="zh-cn_topic_0121682347_row1286841153311"><th class="cellrowborder" valign="top" width="19.74%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0121682347_p178680183310"><a name="zh-cn_topic_0121682347_p178680183310"></a><a name="zh-cn_topic_0121682347_p178680183310"></a><strong id="zh-cn_topic_0121682347_b68682163320"><a name="zh-cn_topic_0121682347_b68682163320"></a><a name="zh-cn_topic_0121682347_b68682163320"></a>名称</strong></p>
</th>
<th class="cellrowborder" valign="top" width="26.490000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0121682347_p78688118335"><a name="zh-cn_topic_0121682347_p78688118335"></a><a name="zh-cn_topic_0121682347_p78688118335"></a><strong id="zh-cn_topic_0121682347_b148681111333"><a name="zh-cn_topic_0121682347_b148681111333"></a><a name="zh-cn_topic_0121682347_b148681111333"></a>描述</strong></p>
</th>
<th class="cellrowborder" valign="top" width="20.119999999999997%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0121682347_p58686123316"><a name="zh-cn_topic_0121682347_p58686123316"></a><a name="zh-cn_topic_0121682347_p58686123316"></a><strong id="zh-cn_topic_0121682347_b98684111338"><a name="zh-cn_topic_0121682347_b98684111338"></a><a name="zh-cn_topic_0121682347_b98684111338"></a>是否必选</strong></p>
</th>
<th class="cellrowborder" valign="top" width="33.650000000000006%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0121682347_p48681314333"><a name="zh-cn_topic_0121682347_p48681314333"></a><a name="zh-cn_topic_0121682347_p48681314333"></a><strong id="zh-cn_topic_0121682347_b48688114333"><a name="zh-cn_topic_0121682347_b48688114333"></a><a name="zh-cn_topic_0121682347_b48688114333"></a>示例</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0121682347_row1286812113317"><td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0121682347_p18685112332"><a name="zh-cn_topic_0121682347_p18685112332"></a><a name="zh-cn_topic_0121682347_p18685112332"></a>X-Sdk-Date</p>
</td>
<td class="cellrowborder" valign="top" width="26.490000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0121682347_p158681113337"><a name="zh-cn_topic_0121682347_p158681113337"></a><a name="zh-cn_topic_0121682347_p158681113337"></a>请求的发生时间，格式为YYYYMMDD'T'HHMMSS'Z'。</p>
<p id="zh-cn_topic_0121682347_p1286816117332"><a name="zh-cn_topic_0121682347_p1286816117332"></a><a name="zh-cn_topic_0121682347_p1286816117332"></a>取值为当前系统的GMT时间。</p>
</td>
<td class="cellrowborder" valign="top" width="20.119999999999997%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0121682347_p48681111339"><a name="zh-cn_topic_0121682347_p48681111339"></a><a name="zh-cn_topic_0121682347_p48681111339"></a>否</p>
<p id="zh-cn_topic_0121682347_p1886851113314"><a name="zh-cn_topic_0121682347_p1886851113314"></a><a name="zh-cn_topic_0121682347_p1886851113314"></a>使用AK/SK认证时该字段必选。</p>
</td>
<td class="cellrowborder" valign="top" width="33.650000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0121682347_p7868131153315"><a name="zh-cn_topic_0121682347_p7868131153315"></a><a name="zh-cn_topic_0121682347_p7868131153315"></a>20150907T101459Z</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_row1486813163318"><td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0121682347_p586816117339"><a name="zh-cn_topic_0121682347_p586816117339"></a><a name="zh-cn_topic_0121682347_p586816117339"></a>Authorization</p>
</td>
<td class="cellrowborder" valign="top" width="26.490000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0121682347_p1986841143311"><a name="zh-cn_topic_0121682347_p1986841143311"></a><a name="zh-cn_topic_0121682347_p1986841143311"></a>签名认证信息。</p>
<p id="zh-cn_topic_0121682347_p986831133320"><a name="zh-cn_topic_0121682347_p986831133320"></a><a name="zh-cn_topic_0121682347_p986831133320"></a>该值来源于请求签名结果。</p>
</td>
<td class="cellrowborder" valign="top" width="20.119999999999997%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0121682347_p48686133312"><a name="zh-cn_topic_0121682347_p48686133312"></a><a name="zh-cn_topic_0121682347_p48686133312"></a>否</p>
<p id="zh-cn_topic_0121682347_p186814103317"><a name="zh-cn_topic_0121682347_p186814103317"></a><a name="zh-cn_topic_0121682347_p186814103317"></a>使用AK/SK认证时该字段必选。</p>
</td>
<td class="cellrowborder" valign="top" width="33.650000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0121682347_p10868121143318"><a name="zh-cn_topic_0121682347_p10868121143318"></a><a name="zh-cn_topic_0121682347_p10868121143318"></a>SDK-HMAC-SHA256 Credential=ZIRRKMTWPTQFQI1WKNKB/20150907//ec2/sdk_request, SignedHeaders=content-type;host;x-sdk-date, Signature=55741b610f3c9fa3ae40b5a8021ebf7ebc2a28a603fc62d25cb3bfe6608e1994</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_row1286861153311"><td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0121682347_p2086813163316"><a name="zh-cn_topic_0121682347_p2086813163316"></a><a name="zh-cn_topic_0121682347_p2086813163316"></a>Host</p>
</td>
<td class="cellrowborder" valign="top" width="26.490000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0121682347_p58681814333"><a name="zh-cn_topic_0121682347_p58681814333"></a><a name="zh-cn_topic_0121682347_p58681814333"></a>请求的服务器信息，从服务API的URL中获取。值为hostname[:port]。端口缺省时使用默认的端口，https的默认端口为443。</p>
</td>
<td class="cellrowborder" valign="top" width="20.119999999999997%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0121682347_p886815123319"><a name="zh-cn_topic_0121682347_p886815123319"></a><a name="zh-cn_topic_0121682347_p886815123319"></a>否</p>
<p id="zh-cn_topic_0121682347_p386811116333"><a name="zh-cn_topic_0121682347_p386811116333"></a><a name="zh-cn_topic_0121682347_p386811116333"></a>使用AK/SK认证时该字段必选。</p>
</td>
<td class="cellrowborder" valign="top" width="33.650000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0121682347_p486814118330"><a name="zh-cn_topic_0121682347_p486814118330"></a><a name="zh-cn_topic_0121682347_p486814118330"></a>code.test.com</p>
<p id="zh-cn_topic_0121682347_p5868161163317"><a name="zh-cn_topic_0121682347_p5868161163317"></a><a name="zh-cn_topic_0121682347_p5868161163317"></a>or</p>
<p id="zh-cn_topic_0121682347_p786841123315"><a name="zh-cn_topic_0121682347_p786841123315"></a><a name="zh-cn_topic_0121682347_p786841123315"></a>code.test.com:443</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_row386818143313"><td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0121682347_p118689123320"><a name="zh-cn_topic_0121682347_p118689123320"></a><a name="zh-cn_topic_0121682347_p118689123320"></a>Content-Type</p>
</td>
<td class="cellrowborder" valign="top" width="26.490000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0121682347_p1486815116337"><a name="zh-cn_topic_0121682347_p1486815116337"></a><a name="zh-cn_topic_0121682347_p1486815116337"></a>发送的实体的MIME类型。推荐用户默认使用application/json，如果API是对象、镜像上传等接口，媒体类型可按照流类型的不同进行确定。</p>
</td>
<td class="cellrowborder" valign="top" width="20.119999999999997%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0121682347_p1086812114335"><a name="zh-cn_topic_0121682347_p1086812114335"></a><a name="zh-cn_topic_0121682347_p1086812114335"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.650000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0121682347_p1186841163310"><a name="zh-cn_topic_0121682347_p1186841163310"></a><a name="zh-cn_topic_0121682347_p1186841163310"></a>application/json</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_row11868419337"><td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0121682347_p178687119330"><a name="zh-cn_topic_0121682347_p178687119330"></a><a name="zh-cn_topic_0121682347_p178687119330"></a>Content-Length</p>
</td>
<td class="cellrowborder" valign="top" width="26.490000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0121682347_p178681813332"><a name="zh-cn_topic_0121682347_p178681813332"></a><a name="zh-cn_topic_0121682347_p178681813332"></a>请求body长度，单位为Byte。</p>
</td>
<td class="cellrowborder" valign="top" width="20.119999999999997%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0121682347_p18687183316"><a name="zh-cn_topic_0121682347_p18687183316"></a><a name="zh-cn_topic_0121682347_p18687183316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="33.650000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0121682347_p148689110334"><a name="zh-cn_topic_0121682347_p148689110334"></a><a name="zh-cn_topic_0121682347_p148689110334"></a>3495</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_row2868171143313"><td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0121682347_p586815118338"><a name="zh-cn_topic_0121682347_p586815118338"></a><a name="zh-cn_topic_0121682347_p586815118338"></a>X-Project-Id</p>
</td>
<td class="cellrowborder" valign="top" width="26.490000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0121682347_p1586811163312"><a name="zh-cn_topic_0121682347_p1586811163312"></a><a name="zh-cn_topic_0121682347_p1586811163312"></a>project id，项目编号。请参考<a href="获取项目ID.md#ZH-CN_TOPIC_0132670200">获取项目ID</a>章节获取项目编号。</p>
<p id="zh-cn_topic_0121682347_p178681018333"><a name="zh-cn_topic_0121682347_p178681018333"></a><a name="zh-cn_topic_0121682347_p178681018333"></a>如果是DeC的请求或者多project的请求则必须传入project id。</p>
</td>
<td class="cellrowborder" valign="top" width="20.119999999999997%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0121682347_p886812110335"><a name="zh-cn_topic_0121682347_p886812110335"></a><a name="zh-cn_topic_0121682347_p886812110335"></a>否</p>
<p id="zh-cn_topic_0121682347_p128682103311"><a name="zh-cn_topic_0121682347_p128682103311"></a><a name="zh-cn_topic_0121682347_p128682103311"></a>如果是专属云场景采用AK/SK 认证方式的接口请求或者多project场景采用AK/SK认证的接口请求则该字段必选。</p>
</td>
<td class="cellrowborder" valign="top" width="33.650000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0121682347_p198684143315"><a name="zh-cn_topic_0121682347_p198684143315"></a><a name="zh-cn_topic_0121682347_p198684143315"></a>e9993fc787d94b6c886cbaa340f9c0f4</p>
</td>
</tr>
<tr id="zh-cn_topic_0121682347_row188688113337"><td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0121682347_p198684111335"><a name="zh-cn_topic_0121682347_p198684111335"></a><a name="zh-cn_topic_0121682347_p198684111335"></a>X-Auth-Token</p>
</td>
<td class="cellrowborder" valign="top" width="26.490000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0121682347_p1086851153317"><a name="zh-cn_topic_0121682347_p1086851153317"></a><a name="zh-cn_topic_0121682347_p1086851153317"></a>用户Token。</p>
<p id="zh-cn_topic_0121682347_p15868417337"><a name="zh-cn_topic_0121682347_p15868417337"></a><a name="zh-cn_topic_0121682347_p15868417337"></a>获取Token，请参考《统一身份认证服务API参考》的“获取用户Token”章节。请求响应成功后在响应消息头中包含的“X-Subject-Token”的值即为Token值。</p>
</td>
<td class="cellrowborder" valign="top" width="20.119999999999997%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0121682347_p4868514338"><a name="zh-cn_topic_0121682347_p4868514338"></a><a name="zh-cn_topic_0121682347_p4868514338"></a>否</p>
<p id="zh-cn_topic_0121682347_p986818114339"><a name="zh-cn_topic_0121682347_p986818114339"></a><a name="zh-cn_topic_0121682347_p986818114339"></a>使用Token认证时该字段必选。</p>
</td>
<td class="cellrowborder" valign="top" width="33.650000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0121682347_p168689113318"><a name="zh-cn_topic_0121682347_p168689113318"></a><a name="zh-cn_topic_0121682347_p168689113318"></a>注：以下仅为Token示例片段MIIPAgYJKoZIhvcNAQcCoIIO8zCCDu8CAQExDTALBglghkgBZQMEAgEwgg1QBgkqhkiG9w0BBwGggg1BBIINPXsidG9rZ</p>
</td>
</tr>
</tbody>
</table>

## 请求消息体<a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_section1437471411"></a>

该部分可选。请求消息体通常以结构化格式（如JSON或XML）发出，与请求消息头中Content-Type对应，传递除请求消息头之外的内容。

若请求消息体中的参数支持中文，则中文字符必须为UTF-8编码。

## 响应消息头<a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_section61333484715"></a>

响应消息头包含如下两部分：

-   一个HTTP状态代码，从2xx成功代码到4xx或5xx错误代码，或者可以返回服务定义的状态码。
-   附加响应头字段，如Content-Type响应消息头。

    详细的公共响应消息头字段请参考[表4](#zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_table3877208613139)。

    **表 4**  公共响应消息头

    <a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_table3877208613139"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_row3771309013139"><th class="cellrowborder" valign="top" width="19.15%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p4531764513139"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p4531764513139"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p4531764513139"></a><strong id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b1355613001117"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b1355613001117"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b1355613001117"></a>名称</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="49.830000000000005%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p4685062813139"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p4685062813139"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p4685062813139"></a><strong id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b555911300112"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b555911300112"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b555911300112"></a>描述</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="31.019999999999996%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p5162099210429"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p5162099210429"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p5162099210429"></a><strong id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b55591930171112"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b55591930171112"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_b55591930171112"></a>示例</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_row1900247113139"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p6280518613139"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p6280518613139"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p6280518613139"></a>Content-Length</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.830000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p4985309313517"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p4985309313517"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p4985309313517"></a>响应消息体的字节长度，单位为Byte。</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.019999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p2055083910429"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p2055083910429"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p2055083910429"></a>--</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_row1673548413139"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p1339693313139"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p1339693313139"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p1339693313139"></a>Date</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.830000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p1140975013139"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p1140975013139"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p1140975013139"></a>系统响应的GMT时间。</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.019999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p59381193104213"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p59381193104213"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p59381193104213"></a>Wed, 27 Dec 2016 06:49:46 GMT</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_row2720466144725"><td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p19031219144725"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p19031219144725"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p19031219144725"></a>Content-Type</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.830000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p65133809144725"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p65133809144725"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p65133809144725"></a>响应消息体的MIME类型。</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.019999999999996%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p21477025104246"><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p21477025104246"></a><a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_zh-cn_topic_0020536997_p21477025104246"></a>application/json</p>
    </td>
    </tr>
    </tbody>
    </table>


## 响应消息体<a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_section2045571671419"></a>

该部分可选。响应消息体通常以结构化格式（如JSON或XML）返回，与响应消息头中Content-Type对应，传递除响应消息头之外的内容。

## 发送请求<a name="zh-cn_topic_0121682347_zh-cn_topic_0113746487_section162124161515"></a>

共有三种方式可以基于已构建好的请求消息发起请求，分别为：

-   cURL

    cURL是一个命令行工具，用来执行各种URL操作和信息传输。cURL充当的是HTTP客户端，可以发送HTTP请求给服务端，并接收响应消息。cURL适用于接口调试。关于cURL详细信息请参见[https://curl.haxx.se/](https://curl.haxx.se/)。

-   编码

    通过编码调用接口，组装请求消息，并发送处理请求消息。

-   REST客户端

    Mozilla、Google都为REST提供了图形化的浏览器插件，发送处理请求消息。针对Firefox，请参见[FirefoxREST Client](https://addons.mozilla.org/en-US/firefox/addon/restclient/)；针对Chrome，请参见[Postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop)。


