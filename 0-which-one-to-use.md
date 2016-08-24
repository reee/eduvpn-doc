# 选择适合自己的链接方式

## 服务器列表：

服务器地址 | 地理位置 | 推荐用于
--- | --- | --- | ---
tokyo-jp.eduvpn.net | 日本 东京 | 联通/移动/IPv6（绕美国）
lax-us.eduvpn.net | 美国 洛杉矶 | 电信/联通/移动/IPv6
sg.eduvpn.net | 新加坡 | 电信/移动/联通/IPv6（绕美国）
hk.eduvpn.net | 香港 | 电信/移动/联通 无IPv6

注1：服务器相关监控，包括负载，带宽占用等，请查看：[munin](https://eduvpn.net/munin)

## 当前提供的连接方式对比如下：

链接名称 | 路由方式 | 是否支持国内路由穿透 | IPv4/IPV6 | 平台支持 | 补充说明
--- | --- | --- | --- | --- | ---
openVPN | 全局路由 | 客户端配置文件指定路由表 | 均支持 | Windows, Mac OS, Linux，openwrt | **仅开放IPv6连接**。
shadowsocks | socks5 / http代理 | 默认国内路由穿透 | 均支持 | Windows, Mac OS, Linux, iOS, Android，openwrt | 默认不支持全局代理，**推荐IPv4/IPv6 桌面端用户使用**。
openconnect / Anyconnect | 全局路由 | 服务器端默认国内路由穿透 | 仅IPv4 | Windows, Mac OS, Linux, iOS, Android | 支持漫游，即网络切换时保持在线。**推荐移动端用户使用**。

注：PPTP，L2TP不安全，IPsec，IKEv2目前会被流量识别而导致服务器被阻断，不再提供。

**任何服务器速度/连接问题请邮件  eduvpn at gmail dot com**
