# immortalwrt
自用immortalwrt

后台 10.0.0.1 密码 空

安装的插件
```
ImmortalWrt 插件的中文解释及功能概述：

基础功能插件
luci-i18n-diskman-zh-cn
磁盘管理插件的中文本地化语言包，用于管理硬盘、挂载点、分区等。

luci-i18n-firewall-zh-cn
防火墙管理插件的中文本地化语言包，用于配置防火墙规则。

luci-i18n-filebrowser-zh-cn
文件管理器插件的中文本地化语言包，用于浏览和管理路由器上的文件。

luci-i18n-opkg-zh-cn
软件包管理插件的中文本地化语言包，用于通过 OpenWrt 的 opkg 系统安装或管理软件包。

luci-i18n-ttyd-zh-cn
TTYD 终端管理插件的中文本地化语言包，允许通过浏览器访问终端界面。

openssh-sftp-server
OpenSSH 的 SFTP 服务模块，提供文件传输功能，类似 FTP，但更安全。

科学上网与代理相关插件
luci-i18n-passwall-zh-cn
Passwall 插件的中文本地化语言包，Passwall 是一个综合性的科学上网插件，支持多种协议和代理方式。

luci-app-openclash
OpenClash 插件，用于配置和管理 Clash 的 GUI 界面，主要用于科学上网。

luci-i18n-homeproxy-zh-cn
HomeProxy 插件的中文本地化语言包，主要用于搭建家庭代理服务。

美化与界面管理插件
luci-app-argon-config
Argon 主题的配置插件，用于调整 Argon 的外观和样式。

luci-i18n-argon-config-zh-cn
Argon 配置插件的中文本地化语言包。

功能增强与工具插件
luci-app-autoreboot
自动重启插件，支持定时任务重启路由器。

luci-app-vlmcsd
用于搭建 KMS 激活服务器的插件，适用于 Windows 和 Office 的激活。

luci-app-wol
网络唤醒 (Wake-on-LAN) 插件，用于远程唤醒局域网内的设备。

luci-app-ddns-go
Go 版动态域名服务（DDNS）插件，用于动态更新域名的 IP 地址。

luci-i18n-ddns-go-zh-cn
DDNS Go 插件的中文本地化语言包。

luci-app-netdata
Netdata 插件，用于实时监控路由器性能指标（CPU、内存、流量等）。

luci-app-upnp
通用即插即用 (UPnP) 服务插件，用于动态开启端口转发，提升兼容性和便利性。

luci-i18n-samba4-zh-cn
Samba 4 插件的中文本地化语言包，用于搭建文件共享服务。

每个插件的具体用途和安装场景可以根据您的需求调整。如果需要某些插件的安装方法或详细配置指导，可以随时询问！
```

如何安装docker
确定软件包是有足够的空间的，如果你安装的是我扩容之后的固件，自然没问题。docker和相关组件可能占用1g
```
luci-i18n-dockerman-zh-cn
```
上述名称是docker的名称。我们可以在软件包那里先更新列表，然后搜索该组件，并安装即可。比较大，需要好几分钟。

另外一个方法是采用命令行安装。
```
opkg update 
opkg install luci-i18n-dockerman-zh-cn
```
安装成功后，会出现在左侧菜单栏。首次使用建议重启一次路由器。
