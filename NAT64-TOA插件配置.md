# NAT64 TOA插件配置<a name="vpc_toa"></a>

## 操作场景<a name="section873033016354"></a>

用户使用IPv6地址通信需要获取来访者的真实IPv6地址。TOA内核模块主要用来获取经NAT64转化过的来访者真实IPv6地址，该插件安装在后端服务器。

当用户需要在操作系统中编译NAT64 TOA内核模块时，可参考本文档进行配置。本操作当前仅支持华北-北京四区域。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   TOA不支持UDP协议。  
>-   TOA模块在以下操作系统中验证可以正常工作，其他内核版本安装方法类似。  
>    -   CentOS 7/7.2 \(Kernel version 3.10.0\)  
>    -   Ubuntu 14.04.3\(Kernel version 3.12.0\)  
>    -   Ubuntu 16.04.3 \(Kernel version 4.4.0\)  

## 前提条件<a name="section730623513357"></a>

-   编译内核模块开发环境需与当前内核版本开发环境一致。
-   确保虚拟机可以访问开放源。
-   如果是非root用户，需拥有sudo权限。

## 操作步骤<a name="section1566101825018"></a>

**编译并加载TOA模块**

以下操作步骤是针对Linux内核版本为3.0以上的操作系统。

1.  准备编译环境。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >安装内核模块开发包的过程中，如果源里面找不到对应内核版本的安装包，需要自行去网上下载需要的安装包。  

    以下是不同Linux发行版本的操作说明，请根据环境选择对应的方案。

    -   CentOS环境下的操作步骤。
        1.  执行如下命令，安装gcc编译器。

            **sudo yum install gcc**

        2.  执行如下命令，安装make工具。

            **sudo yum install make**

        3.  执行如下命令，安装内核模块开发包，开发包头文件与库的版本需要与内核版本一致。

            **sudo yum install kernel-devel-\`uname -r\`**

            >![](public_sys-resources/icon-note.gif) **说明：**   
            >如果自带源里没有对应的内核开发包，可以到如下地址中去下载对应的rpm包。  
            >地址：https://mirror.netcologne.de/oracle-linux-repos/ol7\_latest/getPackage/  
            >以3.10.0-693.11.1.el7.x86\_64为例，下载后执行以下命令安装：  
            >**rpm -ivh**  kernel-devel-3.10.0-693.11.1.el7.x86\_64.rpm。  


    -   Ubuntu、Debian环境下的操作步骤。
        1.  执行如下命令，安装gcc编译器。

            **sudo apt-get install gcc**

        1.  执行如下命令，安装make工具。

            **sudo apt-get install make**

        1.  执行如下命令，安装内核模块开发包，开发包头文件与库的版本需要与内核版本一致。

            **sudo apt-get install linux-headers-\`uname -r\`**

    -   SUSE环境下的操作步骤。
        1.  执行如下命令，安装gcc编译器。

            **sudo zypper install gcc**

        2.  执行如下命令，安装make工具。

            **sudo zypper install make**

        3.  执行如下命令，安装内核模块开发包，开发包头文件与库的版本需要与内核版本一致。

            **sudo zypper install enel-default-devel**

    -   CoreOS环境下的操作步骤。

        CoreOS环境下在容器内进行内核模块的编译时，需要先启动一个用于内核模块开发的容器，然后再进行编译。

        详细过程参见CoreOS官方文档，获取方式如下链接所示。

        <u>[https://coreos.com/os/docs/latest/kernel-modules.html](https://coreos.com/os/docs/latest/kernel-modules.html)</u>

2.  编译内核模块。
    1.  使用git工具，执行如下命令，下载TOA内核模块源代码。

        **git clone https://github.com/huaweicloud/elb-toa**

        **git checkout IPv6**

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >如果未安装git工具，请进入以下链接下载TOA模块源代码。  
        >[https://github.com/huaweicloud/elb-toa/tree/IPv6](https://github.com/huaweicloud/elb-toa/tree/IPv6)  

    2.  执行如下命令，进入源码目录，编译模块。

        **cd src**

        **make**

        编译过程未提示warning或者error，说明编译成功，检查当前目录下是否已经生成toa.ko文件。

3.  <a name="li84761520171217"></a>加载内核模块。
    1.  执行如下命令，加载内核模块。

        **sudo insmod toa.ko**

    2.  执行如下命令，验证模块加载情况，查看内核输出信息。

        **dmesg | grep TOA**

        若提示信息包含“TOA: toa loaded”，说明内核模块加载成功。

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >CoreOS在容器中编译完内核模块后，需要将内核模块复制到宿主系统，然后在宿主系统中加载内核模块。由于编译内核模块的容器和宿主系统共享/lib/modules目录，可以在容器中将内核模块复制到该目录下，以供宿主系统使用。  


4.  自动加载内核模块。

    为了使TOA内核模块在系统启动时生效，可以将加载TOA内核模块的命令加到客户的启动脚本中。

    自动加载内核模块的方法有以下两种方法：

    -   客户可以根据自身需求，在自定义的启动脚本中添加加载TOA内核模块的命令。
    -   参考以下操作步骤配置启动脚本。
        1.  在“/etc/sysconfig/modules/”目录下新建toa.modules文件。该文件包含了TOA内核模块的加载脚本。

            toa.modules文件内容，请参考如下示例：

            **\#!/bin/sh**

            **/sbin/modinfo -F filename /root/toa/toa.ko \> /dev/null 2\>&1**

            **if \[ $? -eq 0 \]; then**

            **/sbin/insmod /root/toa/toa.ko**

            **fi**

            其中“/root/toa/toa.ko”为TOA内核模块文件的路径，客户需要将其替换为自己编译的TOA内核模块路径。

        2.  执行以下命令，为toa.modules启动脚本添加可执行权限。

            **sudo** **chmod +x /etc/sysconfig/modules/toa.modules**

            >![](public_sys-resources/icon-note.gif) **说明：**   
            >客户升级内核后，会导致现有TOA内核模块不匹配，因此需要重新编译TOA内核模块。  


5.  安装多节点。

    如果要在相同的客户操作系统中加载此内核模块，可以将toa.ko文件拷贝到需要加载此模块的虚拟机中，然后参照[3](#li84761520171217)加载内核模块。

    内核模块加载成功以后，应用程序可以正常获取访问者的真实源IPv6地址。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >节点的操作系统发行版与内核版本必须相同。  


**后端服务器适配**

使用NAT64的TOA源地址透传功能，后端服务器应用程序源码应该做以下适配（以下为C语言示例）：

1.  定义用来保存地址的数据结构。

    **struct toa\_nat64\_peer uaddr**

2.  调用函数，获得IPv6地址。

    **getsockopt\(connfd, IPPROTO\_IP, TOA\_SO\_GET\_LOOKUP, &uaddr, &len\)**

    其中

    connfd：服务器端提供服务连接的socket fd

    IPPROTO\_IP：固定

    len：sizeof\(struct toa\_nat64\_peer\)

    TOA\_SO\_GET\_LOOKUP：常量值4096

    uaddr：用来保存NAT64 TOA数据结构的变量

3.  输出地址并保存。

    **uaddr.saddr**

4.  参考代码示例：

    ```
    //定义保存nat64 toa信息的数据结构和变量
    enum {
        TOA_BASE_CTL            = 4096,
        TOA_SO_SET_MAX          = TOA_BASE_CTL,
        TOA_SO_GET_LOOKUP       = TOA_BASE_CTL,
        TOA_SO_GET_MAX          = TOA_SO_GET_LOOKUP,
    };
     
    struct toa_nat64_peer {
        struct in6_addr saddr;
        uint16_t sport;
    };
    struct toa_nat64_peer uaddr;
    ……
    //获取服务端的socket
    sockaddr.sin_family = AF_INET;
    sockaddr.sin_addr.s_addr = htonl(INADDR_ANY);
    sockaddr.sin_port = htons(PORT);
    listenfd = socket(AF_INET,SOCK_STREAM,0);
    bind(listenfd, (struct sockaddr *)&sockaddr, sizeof(sockaddr))
    ……
    //监听对应的socket
    connfd = accept(listenfd, (struct sockaddr*)&caddr, &length);
     
    //获取对应nat64 toa的信息
    char from[40];
    int len = sizeof(struct toa_nat64_peer);
    if (getsockopt(connfd, IPPROTO_IP, TOA_SO_GET_LOOKUP, &uaddr, &len) == 0) {
    inet_ntop(AF_INET6, &uaddr.saddr, from, sizeof(from));
    //获取源IP和源port的信息
    printf("real client [%s]:%d\n", from, ntohs(uaddr.sport));
    }
    ```


