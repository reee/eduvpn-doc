# 如何使用openVPN服务

注意：因为目前ipv4 openvpn服务已经基本不可用，所以openvpn仅推荐IPV6用户使用。

## 一、openVPN服务相关信息

当前所有服务器监听ipv4 udp 1194端口和ipv6 udp6 1195端口。

## 二、客户端的安装

Window用户请根据自己的系统，选择下载：openVPN-bit，或者：openVPN-64bit。注意本站提供的不一定是最新的程序。请考虑从openvpn官方下载最新程序：(http://openvpn.net)  //注意需要翻墙。

Linux用户可以直接使用本发行版的包管理器从源中安装（例：Ubuntu用户可以使用 *sudo apt-get install openvpn* 安装）。某些比较旧的系统可能提供的版本太老（2.3以前版本不支持IPV6），可以考虑自行从源码编译安装。

Mac OS 用户请安装 Tunnelblick

Andorid用户请直接从play安装由openvpn.net官方提供的openvpn connect。

目前iOS用户必须要越狱才能使用openVPN，所以在此不推荐。

## 三、导入配置文件

请直接下载config.zip

Windows用户请将里面所有文件移动到openVPN安装目录下的config文件夹，例如：

Linux用户请将里面的所有文件放置到/etc/openvpn 文件夹。

Mac OS用户请将所有文件放置到 ~/Library/Application Support/Tunnelblick/Configurations。

Andorid用户需要

放置好配置文件以后即可直接连接。

## 四、其他问题

### 1、
