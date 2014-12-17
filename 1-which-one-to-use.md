# 选择适合自己的链接方式

 *  **教育网用户，具有ipv6访问权限**：，建议使用openvpn（ipv6/全局代理/黑名单模式，即只有指定的流量不通过我们的服务器），或者shadowsocks （ipv6，提供一个本地的socks/http代理）。
 * **普通桌面端用户，包括Windows，Mac OS，Linux**：推荐使用shadowsocks，Windows下还可以使用由思科提供的anyconnect客户端（Mac下理论也可以，没有测试）。Linux下可以使用openconnect连接到ocserv。
 * **移动端用户，包括Android，iOS**：强烈建议使用过anyconnect/openconnect连接，主要特点是连接方便，而且即使切换网络也可以保持在线（会在切换网络后主动重连，即漫游）。同时也可以使用shadowsocks连接，理论上效率会更高一些但是较前者配置麻烦。虽然PPTP也可用但是不稳定，不推荐。Windows Phone用户目前只能使用PPTP。
 * **基于openwrt的路由器**：目前较为成熟的方案是使用shadowsocks，配合iptables，ipset，dnsmasq，chinadns-c等达到智能流量定向的目的。较复杂但是可以保证路由器下所有设备自动穿墙。
