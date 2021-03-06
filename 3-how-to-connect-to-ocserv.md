# 如何使用AnyConnect / OpenConnect

## 一、安装 AnyConnect / OpenConnect 客户端

操作系统 | 下载链接 | 本站缓存
--- | --- | ---
Windows | 从官网下载要求授权 | [anyconnect-win-4.4.03034-core-vpn-predeploy-k9.msi](https://files.eduvpn.net/anyconnect-win-4.4.03034-core-vpn-predeploy-k9.msi)
macOS | 从官网下载要求授权 | [anyconnect-macos-4.4.03034-predeploy-k9.dmg](https://files.eduvpn.net/anyconnect-macos-4.4.03034-predeploy-k9.dmg)
Linux | 用包管理器安装OpenConnect | 无
Android | [Google Play: anyconnect](https://play.google.com/store/apps/details?id=com.cisco.anyconnect.vpn.android.avf&hl=zh_CN) <br /> [Google Play: OpenConnect](https://play.google.com/store/apps/details?id=app.openconnect&hl=zh_CN) | [OpenConnect.apk](https://files.eduvpn.net/app.openconnect_1119.apk)
iOS | [App Store: anyconnect](https://itunes.apple.com/cn/app/cisco-anyconnect/id392790924?mt=8) | 无

## 连接

* **Android/iOS上使用AnyConnect：** 需要点击界面的`连接`，选择 `添加新的VPN连接`，然后填入 [选择合适的连接方式](https://eduvpn.net/0-which-one-to-use.html) 处给出的服务器地址，说明可以任意设置。然后点击`完成`，继续回到主界面，点击上方的`Off`按钮打开VPN，开始连接。在接下来的界面输入给你的用户名，密码即可连接。

* **Android上使用OpenConnect：** 需要先点击右上角的`带圈+号图标`新建VPN配置。在接下来的对话框中输入 [选择合适的连接方式](https://eduvpn.net/0-which-one-to-use.html) 处给出的服务器地址，此处可以修改配置文件名称，方便您区分不同服务器。其他选项保持不变，回到主界面，点击配置文件名称开始连接。在接下来的界面输入给你的用户名，密码即可连接。

* **macOS/Windows上使用AnyConnect：** 直接填入 [选择合适的连接方式](https://eduvpn.net/0-which-one-to-use.html) 处给出的服务器地址，然后点击Connect，输入用户名，密码即可连接。

**注意：** AnyConnect/OpenConnect默认不能更改路由设置，服务器默认已经配置了国内路由穿透。
