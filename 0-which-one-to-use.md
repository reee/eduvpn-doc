# 选择适合自己的链接方式

## 服务器列表：

服务器地址 | 地理位置 | 推荐用于
--- | --- | --- | ---
**tokyo-jp.eduvpn.net** | 日本·东京 | 联通/移动/IPv6（绕美国）
**lax-us.eduvpn.net** | 美国·洛杉矶 | 电信/联通/移动/IPv6
**hk.eduvpn.net** | 中国·香港 | 电信/移动/联通 无IPv6
**de.eduvpn.net** | 德国·纽伦堡 | 移动/联通 无IPv6

## 当前提供的连接方式对比如下：

链接名称 | 路由方式 | 是否支持国内路由穿透 | IPv4/IPv6 | 平台支持 | 补充说明
--- | --- | --- | --- | --- | ---
OpenVPN | 全局路由 | 客户端配置文件指定路由表 | 均支持 | Windows, Mac OS, Linux，OpenWRT/LEDE | **仅开放IPv6连接 适用于教育网用户**
ShadowSocks | Socks5 / HTTP代理 | 默认国内路由穿透 | 均支持 | Windows, Mac OS, Linux, iOS, Android，OpenWRT/LEDE | 默认不支持全局代理，**推荐IPv4/IPv6 桌面端用户使用**
OpenConnect / Anyconnect | 全局路由 | 服务器端默认国内路由穿透 | 仅IPv4 | Windows, Mac OS, Linux, iOS, Android | 支持漫游，即网络切换时保持在线。**推荐移动端用户使用**
IKEv2 | 全局路由 | 路由所有流量 | 仅IPv4 | Windows, Mac OS, Linux, iOS, Android | 支持漫游，即网络切换时保持在线。**推荐MacOS，iOS用户使用** 
SSTP | 全局路由 | 路由所有流量 | 仅IPv4 | 仅Windows | **仅推荐Windows用户作为备用** 

注：PPTP，L2TP不安全，IPsec（IKEv1）目前会被流量识别而导致服务器被阻断，不再提供。

**任何服务器速度/连接问题请邮件  eduvpn at gmail dot com**
