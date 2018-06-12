# Socks代理的使用
本服务器提供两种基于Socks5的代理：ShadowSocks和YSocks,使用大同小异，只是后者暂只支持windows。Socks代理的原理是，在本地计算机开一个客户端，客户端和服务器加密通信防止被墙，因为标准的Socks代理是明文的会直接被墙，客户端会在本地开启一个标准的Socks代理（未加密），应用程序通过内部的代理设置使用这个本地的标准的未加密的代理（因为本地通信没有墙）来上网。

## 1.安装客户端
### ShadowSocks
可在[shadowsocks.org](https://shadowsocks.org/en/download/clients.html)找到下载客户端，本站提供部分客户端安装包：
+ [Android](https://proxy.njunova.com/file/Shadowdsocks-3.3.1.apk)
+ [Windows](https://proxy.njunova.com/file/Shadowsocks-3.4.3.zip)
+ [Mac OS](https://proxy.njunova.com/file/ShadowsocksX-NG-1.4-beta.zip)

安装启动后填写配置：
+ 服务器地址 proxy.njunova.com
+ 服务器端口 53
+ 加密方式 AES-256-CFB
+ 密码请咨询管理员
+ 本地端口可以自己定，譬如1080

### YSocks
下载[客户端](../file/socks-client.rar)，解压后有两个文件：主程序+配置文件。   
配置文件是Json格式，可以继续添加多个代理。直接双击主程序即可启动本地Socks代理。
配置项有三个：
* local_port 本地端口，可以自己指定
* remote_host 远程服务器地址，可以使用域名或者ip。默认配置文件分别使用ipv4,ipv6和域名写了三条。
* remote_port 远程服务器端口，本站固定为8888  

默认的配置文件是可以直接用的。大家可以自行根据需求调整本地端口或远程服务器地址。

## 2.使用Socks代理
除了ShadowSocks的Android/iOS通过结合VPN支持了全局代理外，Socks代理只支持内部允许设置代理的应用程序，笔者使用的程序譬如Chrome，IDM，Spotify都是支持的。其设置大同小异，只要确保设置中，代理类型是 Socks5，服务器地址是127.0.0.1，端口填写自己在客户端配置的端口。  

譬如IDM的设置：  
![](/assets/socks5-idm.png)  
Spotify的设置  
![](/assets/spotify-socks.png)  

Chrome的设置也类似，只是需要先安装Switchy Omega插件并在该插件里设置代理。详见 [《在chrome中使用Socks代理》](socks-proxy-chrome.md)。