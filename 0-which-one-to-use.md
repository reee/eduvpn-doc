# 选择适合自己的链接方式

## 服务器列表：

当前服务器各种线路基本可以兼顾，所以短期内应该不会更新了。

服务器地址 | 地理位置 | 带宽情况
--- | --- | ---
tokyo-jp.eduvpn.net | 日本 东京 | 100Mbps对等。**推荐通常情况下使用，IPV6连接比lax-us稍慢**
lax-us.eduvpn.net | 美国 洛杉矶 | 100Mbps对等。**推荐用于IPv6连接和电信用户使用，IPV6连接最优**
sg.eduvpn.net | 新加坡 | 100Mbps对等。 **电信走CN2，主要推荐电信用户使用**

注：服务器相关监控，包括负载，带宽占用等，请查看：[munin](https://eduvpn.net/munin)

## 当前提供的连接方式对比如下：

链接名称 | 路由方式 | 是否支持国内路由穿透 | IPv4/IPV6 | 平台支持 | 补充说明
--- | --- | --- | --- | --- | ---
openVPN | 全局路由 | 通过.ovpn指定路由表穿透 | 均支持 | Windows, Mac OS, Linux，openwrt | **仅开放IPv6连接**。
shadowsocks | socks5 / http代理 | 默认国内路由穿透 | 均支持 | Windows, Mac OS, Linux, iOS, Android，openwrt | 默认不支持全局代理，**推荐IPv4/IPv6 桌面端用户使用**。
openconnect / anyconnect | 全局路由 | 服务器端默认国内路由穿透 | 仅IPv4 | Windows, Mac OS, Linux, iOS, Android | 支持漫游，即网络切换时保持在线。**推荐移动端用户使用**。

注1：PPTP，L2TP不安全，IPsec，IKEv2目前会被流量识别而导致服务器被阻断，不再提供。

注2：shadowsocks 默认没有开通，需要自行来邮件申请。我们也暂时不提供这两者运行在openwrt上的教程，请自行谷歌。

**任何服务器速度/连接问题请邮件  eduvpn at gmail dot com**
