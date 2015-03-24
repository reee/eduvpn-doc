# 如何使用OpenVPN服务

## 一、OpenVPN服务相关信息

注意：当前OpenVPN仅开放IPv6连接。服务器当前监听 IPv6 udp6 1195端口

## 二、安装openVPN客户端

系统 | 下载链接 | 本站缓存
--- | --- | ---
Windows | [openVPN官方页面](http://openvpn.net/index.php/open-source/downloads.html) | [Win XP 32位](https://eduvpn.net/files/openvpn-install-2.3.6-I003-i686.exe) <br />[Win XP 64位](https://eduvpn.net/files/openvpn-install-2.3.6-I003-x86_64.exe) <br /> [Win Vista及以上 32位](https://eduvpn.net/files/openvpn-install-2.3.6-I603-i686.exe) <br /> [Win Vista及以上 64位](https://eduvpn.net/files/openvpn-install-2.3.6-I603-x86_64.exe)
Mac OS | [TunnelBlick 官方页面](http://sourceforge.net/projects/tunnelblick/) | [Mac OS 10.6-10.10](https://eduvpn.net/files/Tunnelblick_3.4.4_build_4055.4236.dmg)
Linux | 请直接从发行版源中安装 | 无

## 三、导入配置文件

### 首先需要下载配置文件：

Linux/Windows: [config.zip](https://eduvpn.net/files/config.zip)

Mac OS: [config-mac.zip](https://eduvpn.net/files/config-mac.zip)

Linux/Windows与Mac OS的区别在于前者支持从文本文件读取用户名，密码，而后者不支持。默认配置为从eduvpn.txt文件读取，格式为：首行用户名，次行密码：

  xiaoming

  getout

**需要自行加入到eduvpn.txt文件** 否则会报错无法连接。

如果提供的新服务器没有同步配置文件，请自行使用恰当的编辑器替换 remote 段。

### 将配置文件解压后放到相应目录

系统 | 默认目录 | 注意
--- | --- | ---
Windows | *C:\Program Files\OpenVPN\config* | 即您选择的安装目录下的config文件夹
Mac OS | *~/Library/Application Support/Tunnelblick/Configurations* | 无
Linux | */etc/openvpn* | 如果您自行编译的话，以编译时指定的目录为准

放置好配置文件以后即可直接连接。

注意：如果需要校内地址穿透，请下载 [routes.zip](https://eduvpn.net/files/route.zip) ，打开对应学校命名的txt文档。比如您在北师大则打开 *bnu.txt* ，将里面的所有内容加入到配置文件最后即可。
