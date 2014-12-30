# eduVPN服务介绍

eduVPN从2010年开始服务，eduVPN目前提供以下服务：

 * openVPN (ipv6 / ipv4)
 * shadowsocks (ipv6 / ipv4)
 * openconnect / anyconnect (ipv4 only, by ocserv)
 * pptp (ipv4 only)
 * pure ikev2 ( ipv4 only, by strongswan)

# 致谢

我们使用了以下开源软件(项目)来为您提供服务，包括但不限于：

 * [Ubuntu](http://www.ubuntu.com/) ：基础系统。
 * [Saltstack](http://www.saltstack.org/) ：用于多台VPS配置同步，管理。
 * [ocserv](http://www.infradead.org/ocserv/)：提供openconnect/anyconnect兼容VPN接入。
 * [openVPN](http://openvpn.net/)：提供openvpn接入。
 * [shadowsocks](http://shadowsocks.org/)：提供shadowsocks接入。
 * [bind9](http://www.isc.org/downloads/bind/)：在非标准端口提供DNS缓存服务。
 * [munin](http://munin-monitoring.org/)：用于系统监控。
 * [supervisor](http://supervisord.org/)：用于进程守护，主要是shadowsocks，考虑换成更完备的monit。
 * [fail2ban](http://www.fail2ban.org/)：用于系统加固。
 * [pptpd](http://sourceforge.net/projects/poptop/files/pptpd/)：提供pptp接入。
 * [freeradius](http://freeradius.org/)：用于提供中心认证系统。

