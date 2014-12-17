# eduVPN服务介绍

eduVPN从2010年开始服务，eduVPN目前提供以下服务：

 * openVPN （同时提供ipv4 和ipv6接入但是ipv4因为受干扰而无法使用）
 * shadowsocks （在相同的端口同时提供ipv4 和ipv6接入）
 * ocserv （仅提供ipv4接入，同时兼容openconnect和anyconnect客户端）
 * pptp （仅提供ipv4接入，受干扰严重，不推荐）

其中除了shadowsocks以外其他所有VPN均接入freeradius统一进行认证，也就是同一个用户名/密码使用openvpn，pptp。anyconnet/openconnect。
没有配置l2tp的主要考虑是l2tp目前跟pptp差不多半残废，而没有配纯ikev2的主要原因是麻痹配了好几久都没搞定。

预期在不久的将来提供ikev2支持。

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

