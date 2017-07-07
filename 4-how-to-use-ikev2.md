# 如何使用IKEv2

IKEv2效率比ShadowSocks要低一些，与Anyconnect/OpenConnect效率相仿，其优势在于强加密，安全稳定，而且支持漫游，在切换网络的时候不会掉线。

目前服务器证书通过Let's Encrypt签发，无需额外导入证书即可直接连接使用。

## 系统支持情况

* iOS（从iOS 9 开始），macOS（从 macOS 10.11开始）原生支持IKEv2。可以考虑使用IKEv2连接。
* Windows 从Windows 7开始（Windows Mobile 从Windows Mobile 8.1开始）内置IKEv2支持。但是Windows 10（Windows Mobile 10）默认不路由流量，表现为正常连接但是某些网站依然无法访问。
* Android 可以安装Google Play中由StrongSwan官方提供的同名Android客户端连接。
* Linux可以通过NetworkManager以及相关插件连接到服务器。

## 连接

* **iOS上使用IKEv2：** 点击 `设置`，选择 `通用-VPN-添加VPN配置`，其中 `描述` 字段可以自己取名， `服务器` 和 `远程ID` 均填写 [选择合适的连接方式](https://eduvpn.net/0-which-one-to-use.html) 处给出的服务器地址（必须填写域名，不能填写IP），用户鉴定保持默认的 `用户名` 方式，下方填入 给你的用户名，密码为可选，如果不填将在下次连接时询问。填好以后连接即可。

* **Android上使用IKEv2：** 首先从[官方地址](https://download.strongswan.org/Android/)下载到官方提供的客户端，或者下载[本站缓存的客户端](https://files.eduvpn.net/strongSwan-1.9.2.apk)。安装完成后打开软件，点击右上角 `添加VPN配置` 新建VPN配置。在接下来的对话框中依次 [选择合适的连接方式](https://eduvpn.net/0-which-one-to-use.html)  处给出的服务器地址，您得到的用户名、密码。然后点击保存，然后连接即可。

* **macOS上使用IKEv2：** 
1. 打开 `设置` 中的 `网络`，点击左下角的 `＋` 添加新的连接。在 `接口` 中选择VPN，`VPN类型` 选择 `IKEv2` ， [选择合适的连接方式](https://eduvpn.net/0-which-one-to-use.html) 处给出的服务器地址，而后点击“创建”。
2. 服务器地址处，填入 [选择合适的连接方式](https://eduvpn.net/0-which-one-to-use.html) 处给出的服务器地址，远程ID与服务器地址相同，本地ID不填。
3. 点击 `鉴定设置` ，下拉框 选择 `用户名` ，然后在下面填入您的用户名密码。点击 `好` ， 保存。
4. 点击右下方 `应用` ，然后点击 `连接` 。连接即可。

* **Windows 上使用IKEv2：** 
1. 在任何地方新建一个文本文件， 将后缀从 `.txt` 改为 `.pbk` ， 譬如 eduVPN.pbk。双击打开会提示电话簿为空，要求新建。
2. 点击新建，选择 `工作区网络` ， Internel地址处填入[选择合适的连接方式](https://eduvpn.net/0-which-one-to-use.html) 处给出的服务器地址，目标名称填写任意名称均可（会被用作连接的名称）
3. 点击连接，输入用户名、密码，域不填，然后连接即可。您也可以选择勾选 `为下面用户保存用户名和密码` ，让Windows记住用户名和密码。

**注意：** IKEv2不能更改路由设置，所有流量均会由服务器路由。