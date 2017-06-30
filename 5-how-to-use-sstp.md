# 如何使用SSTP

由于目前服务器端采用的是使用python写的sstp-server，效率较低，目前实际跑出来的速度应该比上面几个协议都要略低一些。

不过SSTP的优势在于其是一个相对小众的协议，且Windows内置原生支持。可作为Windows下使用的备选方案。

## 系统支持情况

仅Windows原生支持，虽然其他各个平台均有对应的兼容客户端，但是并不推荐。

## 连接

可以采用类似Windows下使用IKEv2协议的方式连接，也可以直接通过新建VPN连接的方式进行连接。

需要提醒的是，当前服务器SSTP Server监听在8080端口，因此服务器地址需添加 `:8080` 方可连接。即若是您想链接到Tokyo服务器上的SSTP服务，则服务器地址栏应当填写 ` tokyo-jp.eduvpn.net:8080` 。

**注意：** SSTP不能更改路由设置，所有流量均会由服务器路由。