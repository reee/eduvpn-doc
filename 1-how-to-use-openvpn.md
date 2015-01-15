# 如何使用OpenVPN服务

注意：** 因为目前ipv4 openvpn服务已经基本不可用，所以OpenVPN仅推荐IPv6用户使用。**

## 一、OpenVPN服务相关信息

当前所有服务器监听ipv4 udp 1194端口和ipv6 udp6 1195端口。

## 二、客户端的安装

Window用户请根据自己的系统，选择下载：[OpenVPN-32bit](https://eduvpn.net/files/openvpn-32bit.zip)，或者：[OpenVPN-64bit](https://eduvpn.net/files/openvpn-64bit.zip)。注意本站提供的不一定是最新的程序。请考虑从OpenVPN官方下载最新程序：(http://openvpn.net)  *需要翻墙*。

Linux用户可以直接使用本发行版的包管理器从源中安装（例：Ubuntu用户可以使用 *sudo apt-get install openvpn* 安装）。某些比较旧的系统可能提供的版本太老（2.3以前版本不支持IPV6），可以考虑自行从源码编译安装。

Mac OS 用户请安装 ：[Tunnelblick](https://eduvpn.net/files/tunnelblick.zip)，或者访问 [Tunnelblick官方站点](https://code.google.com/p/tunnelblick/)下载。 *需要翻墙*

对于移动端用户，目前iOS和Android暂时只支持IPv4下的OpenVPN，所以暂时均不可用，如果需要尝试：

Andorid用户请直接从Play安装由OpenVPN官方提供的[OpenVPN Connect](https://play.google.com/store/apps/details?id=net.openvpn.openvpn&hl=zh_CN) iOS用户可以从App Store安装同样由OpenVPN官方提供的[OpenVPN Connect](https://itunes.apple.com/cn/app/openvpn-connect/id590379981?mt=8)。

## 三、导入配置文件

OpenVPN配置文件是以.ovpn结尾的配置文件，可以使用文本编辑器（注意Windows系统自带的记事本对换行符支持不好，如有编译配置文件需要，推荐在Windows系统使用Notepad++ 或者Notepad2）直接编辑。

请直接下载[config.zip](https://eduvpn.net/files/config.zip)

Windows用户请将里面所有文件移动到OpenVPN安装目录下的config文件夹，例如：默认情况下OpenVPN被安装到 *C:\Program Files\OpenVPN\* ，则配置文件应被放到 *C:\Program Files\OpenVPN\config* 。

使用包管理器安装OpenVPN的Linux用户请将里面的所有文件放置到 */etc/openvpn* 文件夹。如果是您自己编译的OpenVPN，则放到您编译时指定的配置文件夹即可。

Mac OS用户请将所有文件放置到 *~/Library/Application Support/Tunnelblick/Configurations*。

放置好配置文件以后即可直接连接。

## 四、连接到OpenVPN服务器



## 五、其他问题

### 1、让OpenVPN连接时从文件读取用户名密码而不需要手动输入

注意：**Mac OS客户端不支持从文件读取用户名密码，在配置文件加入下列项会报错。**

在配置文件中加入一行：

 *auth-user-pass xxx.txt*

然后在配置文件目录下，新建xxx.txt 然后依次输入用户名密码。例假设用户名为 *xiaoming* 密码为 *get-out* 则文件应该内容如下：

*xiaoming*
*get-out*

重新以后 ，OpenVPN将从文本文件读取用户名密码而不再通过交互界面询问。
