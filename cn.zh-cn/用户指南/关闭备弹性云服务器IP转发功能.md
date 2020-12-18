# 关闭备弹性云服务器IP转发功能<a name="vpc_vip_0007"></a>

**Linux系统**

1.  登录弹性云服务器执行如下命令，查看IP转发功能是否已开启。

    cat /proc/sys/net/ipv4/ip\_forward

    回显结果：1为开启，0为关闭，默认为0。

    -   回显为1，执行[2](#zh-cn_topic_0206027322_zh-cn_topic_0095139658_li1473585332417)和[3](#zh-cn_topic_0206027322_zh-cn_topic_0095139658_li88984711254)关闭IP转发功能。
    -   回显为0，操作完成。

2.  <a name="zh-cn_topic_0206027322_zh-cn_topic_0095139658_li1473585332417"></a>使用vi打开“/etc/sysctl.conf”文件，修改net.ipv4.ip\_forward = 0，按“:wq”保存退出。或使用sed命令修改，参考命令如下：

    sed -i '/net.ipv4.ip\_forward/s/1/0/g' /etc/sysctl.conf

3.  <a name="zh-cn_topic_0206027322_zh-cn_topic_0095139658_li88984711254"></a>执行如下命令，使修改生效。

    sysctl -p /etc/sysctl.conf


**Windows系统**

1.  在Windows系统的“开始 \> 命令提示符”执行如下命令。

    ipconfig /all

    回显结果中：“IP 路由已启用”为 “否”， 则IP转发功能已关闭。

2.  按“Windows+R”打开运行窗口，输入regedit，进入注册表编辑器。
3.  编辑HKEY\_LOCAL\_MACHINE\\SYSTEM\\CurrentControlSet\\Services\\Tcpip\\Parameters下的IPEnableRouter值为0。
    -   指定值为 0：关闭 IP 转发。
    -   指定值为 1：启用 IP 转发。


