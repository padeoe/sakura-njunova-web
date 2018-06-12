# Android
Android上有两种方式建立VPN，一种是利用系统自带的VPN，一种是安装app：Strongswan建立vpn。区别是前者建立的是IPSec Xauth PSK类型的VPN，后者建立的是IKEv2 EAP认证的VPN。
前者好像不是很稳，推荐安装app。

## 使用StrongSwan创建VPN
[点此下载](../file/strongswan-1.9.6.apk)(8.71MB)客户端 “Strongswan.apk”，安装后打开，新建连接如下。填好后保存。然后连接。

![](/assets/android-strongswan.png)

## 使用系统设置创建VPN
打开设置-更多-VPN，添加VPN。如图，确保其中：服务器地址是 sakura.njunova.com ，VPN类型是IPSec Xauth PSK，IPSec预共享密钥是 myPSKkey。

![](/assets/android-system.png)