# 如何使用shadowsocks

shadowsocks是一个比较新的协议，相比其他方式，主要特点如下：

 * 优势：效率高。
 * 劣势：默认不提供全局代理（而是提供一个SOCKS5代理），如果需要全局代理（比如游戏）则需要额外的设置。

**考虑到效率问题，推荐IPv4/IPv6用户首选。**

## 一、shadowsocks 相关信息

目前shadowsocks采取不同用户使用不同端口的方式来避免因为单个端口流量过高而被防火墙识别阻断的问题。当前采用的加密方式为 *aes-128-cfb*

注意：考虑到效率问题，加密方式可能会有所变更，请注意我们的邮件或者关注此页面。

## 二、安装shadowsocks客户端

系统 | 下载链接 | 本站缓存
--- | --- | ---
Windows | [官方sf站点](http://sourceforge.net/projects/shadowsocksgui/) | Win 8 以及更新的系统：[Shadowsocks-win-dotnet4.0-2.5.2.zip](https://eduvpn.net/files/Shadowsocks-win-dotnet4.0-2.5.2.zip) <br /> Win 7及更早系统：[Shadowsocks-win-2.5.2.zip](https://eduvpn.net/files/Shadowsocks-win-2.5.2.zip)
Mac OS | [官方sf站点](http://sourceforge.net/projects/shadowsocksgui/) | [ShadowsocksX-2.6.3.dmg](https://eduvpn.net/files/ShadowsocksX-2.6.3.dmg)
Linux | 直接从包管理器安装 | 无
Android | [Google Play](https://play.google.com/store/apps/details?id=com.github.shadowsocks) | 无
iOS | [Apple App Store](https://itunes.apple.com/cn/app/shadowsocks/id665729974?mt=8) | 无

## 三、连接

例如:

  tokyo-jp.eduvpn.net

  your-port

  your-password

  aes-128-cfb
  
  any-comment-you-want

然后点击连接即可。

默认为国内地址穿透，可以在右键菜单中改为全部流量均过服务器。
