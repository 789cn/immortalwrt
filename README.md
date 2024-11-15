# immortalwrt
自用immortalwrt

后台 10.0.0.1 密码 空

安装的插件
```
luci-i18n-firewall-zh-cn      #防火墙汉化
luci-i18n-filebrowser-zh-cn   #网页文件管理
luci-app-argon-config         #主题
luci-i18n-argon-config-zh-cn  #主题
luci-i18n-opkg-zh-cn       #软件包汉化
luci-i18n-ttyd-zh-cn       #内置SHH
luci-i18n-passwall-zh-cn   #科学
luci-app-openclash         #科学
luci-i18n-homeproxy-zh-cn  #科学中文
luci-app-autoreboot        #重启
luci-app-diskman           #磁盘管理
luci-app-nlbwmon           #流量监控
luci-app-vlmcsd            #KMS 微软系统激活
luci-app-wol               #网络唤醒
luci-app-samba4            #文件共享
luci-app-ddns-go           #ddns转发
luci-i18n-ddns-go-zh-cn    #汉化
luci-app-netdata           #实时监控
luci-app-upnp              #RT
luci-app-cpulimit          #CPU频率设置
luci-app-socat             #端口转发
luci-app-wireguard         #VPN回家-没防火墙的好用
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
