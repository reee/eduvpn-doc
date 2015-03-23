# eduVPN服务介绍

eduVPN从2010年开始服务，eduVPN目前提供以下服务：

 * openVPN (IPv6 only)
 * shadowsocks (IPv6 / IPv4)
 * openconnect / anyconnect (IPv4 only, by ocserv)
 * shadowvpn (IPv4 /IPv6)

# 致谢

我们使用了以下开源软件(项目)来为您提供服务，包括但不限于：

 * [Ubuntu](http://www.ubuntu.com/) ：基础系统。
 * [ocserv](http://www.infradead.org/ocserv/)：提供openconnect/anyconnect兼容VPN接入。
 * [openVPN](http://openvpn.net/)：提供openvpn接入。
 * [shadowsocks](http://shadowsocks.org/)：提供shadowsocks接入。
 * [bind9](http://www.isc.org/downloads/bind/)：在非标准端口提供DNS缓存服务。
 * [munin](http://munin-monitoring.org/)：用于系统监控。
 * [supervisor](http://supervisord.org/)：用于shadowsocks进程守护
 * [fail2ban](http://www.fail2ban.org/)：用于系统加固。
 * [freeradius](http://freeradius.org/)：用于提供中心认证系统。
