# 选择适合自己的链接方式

## 服务器列表：

为了保证在较低成本情况下提供最优服务，服务器列表可能随时会更新，请注意经常前来查看。

服务器地址 | 地理位置 | 机房 | 带宽情况 
--- | --- | --- | ---
tokyo-jp.eduvpn.net | 日本 东京 | Sakura东京机房 | 100Mbps对等。**正常情况下连接速度优秀！**
fremont-us.eduvpn.net | 美国 费利蒙 | Linode 东京机房 | 40Gbps In，125Mbps Out。**IPv6连接速度优秀。**
hk.eduvpn.net | 香港 | Gigsgigscloud 香港机房 | 限速8mbps，不支持IPV6，仅供IPV4使用。**IPv4延迟最低但是带宽小。**

注：服务器相关监控，包括负载，带宽占用等，请查看：[munin](https://eduvpn.net/munin)

## 当前提供的连接方式对比如下：

链接名称 | 路由方式 | 是否支持国内路由穿透 | IPv4/IPV6 | 平台支持 | 补充说明
--- | --- | --- | --- | --- | ---
openVPN | 全局路由 | 通过.ovpn指定路由表穿透 | 均支持 | Windows, Mac OS, Linux，openwrt | **仅供IPv6用户使用**。
shadowvpn | 全局路由 | 默认国内路由穿透 | 仅IPv6 | Linux，openwrt | **账号要求自行申请，推荐高端IPv4用户使用**。
shadowsocks | socks5 / http代理 | 默认国内路由穿透 | 均支持 | Windows, Mac OS, Linux, iOS, Android，openwrt | 桌面端无法全局代理，**推荐IPv4/IPv6 桌面端用户使用**。
openconnect / anyconnect | 全局路由 | 服务器端默认国内路由穿透 | 仅IPv4 | Windows, Mac OS, Linux, iOS, Android | 支持漫游，网络切换时可以保持在线。**推荐移动端用户使用**。

注：PPTP，L2TP不安全，IPsec，IKEv2目前会被流量识别而导致服务器被阻断，不再提供。

