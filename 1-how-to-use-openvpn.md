# 如何使用OpenVPN服务

注意：** 因为目前ipv4 openvpn服务已经基本不可用，所以OpenVPN仅推荐IPv6用户使用。**

## 一、OpenVPN服务相关信息

1. 当前所有服务器监听ipv4 udp 1194端口和ipv6 udp6 1195端口。

2. Mac要求必须从界面输入密码，Windows/Linux 系统支持从文件读取用户名密码，默认配置为从eduvpn.txt文件读取，格式应保持如下：

*xiaoming*

*getout*

3.配置文件下载：
Linux/Windows: config.zip
Mac OS: config-mac.zip

4. 如果提供的新服务器没有同步配置文件，请自行使用恰当的编辑器替换 remote 段。

## 二、客户端的安装

Window用户:访问官方下载页面下载：http://openvpn.net/index.php/open-source/downloads.html

本站缓存的安装包（可能不是最新）：


Linux用户可以直接使用本发行版的包管理器从源中安装（例：Ubuntu用户可以使用 *sudo apt-get install openvpn* 安装）。某些比较旧的系统可能提供的版本太老（2.3以前版本不支持IPV6），可以考虑自行从源码编译安装。

Mac OS 用户：访问官方下载页面下载：https://code.google.com/p/tunnelblick/

本站缓存的安装文件（可能不是最新）：[Tunnelblick](https://eduvpn.net/files/tunnelblick.zip)。

## 三、导入配置文件

Windows用户请将里面所有文件移动到OpenVPN安装目录下的config文件夹，例如：默认情况下OpenVPN被安装到 *C:\Program Files\OpenVPN\* ，则配置文件应被放到 *C:\Program Files\OpenVPN\config* 。

使用包管理器安装OpenVPN的Linux用户请将里面的所有文件放置到 */etc/openvpn* 文件夹。如果是您自己编译的OpenVPN，则放到您编译时指定的配置文件夹即可。

Mac OS用户请将所有文件放置到 *~/Library/Application Support/Tunnelblick/Configurations*。

放置好配置文件以后即可直接连接。

注意：如果需要校内地址穿透，请下载 route.zip ，打开对应学校命名的txt文档比如 bnu.txt 加入到配置文件最后即可。