# 选择适合自己的链接方式
## 当前提供的连接方式对比如下：

链接名称 | 路由方式 | 是否支持国内路由穿透 | 是否支持IPV6 | 平台支持 | 补充说明
--- | --- | --- | --- | --- | ---
openVPN | 全局路由 | 通过.ovpn指定路由表穿透 | 支持 | Windows, Mac OS, Linux, iOS, Android | IPV4已经全面瘫痪，IPV6也有被墙的迹象，**推荐IPV6用户使用**。
shadowsocks | 在本地提供一个socks5 / http代理 | 最新版直接支持国内路由穿透 | 支持 | Windows, Mac OS, Linux, iOS, Android | 目前效率最高的连接方式，但是不支持全局代理，**推荐IPV4桌面端用户使用**。
openconnect / anyconnect | 全局路由 | 由服务器指定国内路由穿透（已配置） | 不支持 | Windows, Mac OS, Linux, iOS, Android | 支持漫游，即从一个网络切换到另外一个网络可以保持在线。**推荐移动端用户使用**。
IKEv2 | 全局路由 | 暂不支持 | | Windows, Mac OS, Linux, iOS, Android, Windows Phone | 因为被大量企业使用，所以是目前最不容易受照顾的协议，**推荐用作后备，Windows Phone用户目前只能使用IKEv2**。
PPTP | 全局路由 | 客户端指定路由表 | 不支持 | Windows, Mac OS, Linux, iOS, Android | 不安全，已经被墙照顾，不推荐使用。

注：基于openwrt的路由器目前比较成熟的方案为shadowsocks，在路由器上使用shadowsocks可以让该路由下所有设备同时享受VPN效果，**推荐倒腾党采用**。

## 目前服务器列表如下：

服务器地址 | 地理位置 | 机房 | 带宽情况 
--- | --- | --- | ---
tokyo-jp.eduvpn.net | 日本 东京 | Sakura东京机房 | 100Mbps对等。
fremont-us.eduvpn.net | 美国 费利蒙 | Linode 东京机房 | 40Gbps In，125Mbps Out。
sgp.eduvpn.net | 新加坡 | DigitalOcean 新加坡机房 | 1Gbps对等。

注：服务器相关监控，包括负载，带宽占用等，请查看：[munin](https://eduvpn.net/munin)
