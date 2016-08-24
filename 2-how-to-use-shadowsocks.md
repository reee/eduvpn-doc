# 如何使用shadowsocks

shadowsocks是一个比较新的协议，相比其他方式，主要特点如下：

 * 优势：效率高。
 * 劣势：默认不提供全局代理（而是提供一个SOCKS5代理），如果需要全局代理（比如游戏）则需要额外的设置。

**考虑到效率问题，推荐IPv4/IPv6用户首选。**

## 一、shadowsocks 相关信息

目前shadowsocks采取不同用户使用不同端口的方式来避免因为单个端口流量过高而被防火墙识别阻断的问题。当前采用的加密方式为 `aes-128-cfb`

注意：考虑到效率问题，加密方式可能会有所变更，请注意我们的邮件或者关注此页面。

## 二、安装shadowsocks客户端

系统 | 下载链接 | 本站缓存
--- | --- | ---
Windows | [官方github站点](https://github.com/shadowsocks/shadowsocks-windows/releases) | [Shadowsocks-3.0.zip](https://files.eduvpn.net/Shadowsocks-3.0.zip) 
Mac OS | [官方github站点](https://github.com/shadowsocks/shadowsocks-iOS/releases) | [ShadowsocksX-2.6.3.dmg](https://files.eduvpn.net/ShadowsocksX-2.6.3.dmg)
Linux | 直接从包管理器安装 | 无
Android | [Google Play](https://play.google.com/store/apps/details?id=com.github.shadowsocks) | 无
iOS | [Apple App Store](https://itunes.apple.com/cn/app/shadowsocks/id665729974?mt=8) | 无

## 三、连接

打开shadowsocks，依次填入以下信息：

选项 | 内容填写
--- | ---
服务器地址： | 请从[选择合适的连接方式](https://eduvpn.net/0-which-one-to-use.html)页面选择。
服务器端口： | 发送给您的端口
密码： | 发送给您的密码
加密： | 当前为  `aes-128-cfb`  
备注： | 可不填，为该配置文件的名称
一次性认证： | 不勾选
代理端口： | 如无特殊需要，不更改


然后在任务栏小飞机图标点击右键，选择`启用系统代理`。

**注意：**

1. 默认为国内地址穿透，可以在任务栏小飞机图标点击右键，在菜单 --> `系统代理模式` 中选择`全局模式`，改为全部流量均过服务器。
2. 如果在启用代理的情况下异常关机，会导致下次打开浏览器出现无法连接情况，请打开shadowsocks，在任务栏小飞机图标点击右键，取消`启用系统代理`即可。
3. 在Windows系统，如果您将shadowsocks放置于C盘程序目录，需要给予shadowsocks管理员权限，shadowsocks才能正常运行。