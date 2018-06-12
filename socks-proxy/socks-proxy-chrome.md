# 在Chrome中使用Socks代理
## 1.安装客户端,Chrome浏览器和SwitchyOmega插件
客户端下载见上一页。
Chrome的官方下载地址 ：[Chrome](https://www.google.com/intl/en/chrome/browser/desktop/index.html?standalone=1)。  
SwitchyOmega插件可在[Chrome商店](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif?hl=en)或者[Github](https://github.com/FelisCatus/SwitchyOmega/releases)下载，

本站的离线安装包：   
[windows 32位Chrome(55.0.2883.87)](../file/ChromeStandaloneSetup.exe)   
[windows 64位Chrome(55.0.2883.87)](../file/ChromeStandaloneSetup64.exe)   
[SwitchyOmega.crx](../file/SwitchyOmega.crx)
## 2.在插件中配置代理
打开swichy omega的配置界面，新建情景模式-代理服务器。   
![](/assets/chrome-socks-conf.png)  
如图填写，确保协议是**Socks5**，服务器地址是**127.0.0.1**,端口是配置文件中对应服务器的端口（默认配置文件1080端口是通用的，1081端口是ipv4代理，1082端口是ipv6代理）。  

填写完毕后，点击应用更改。   

## 3.使用代理
在浏览器右上角选中刚才创建的代理，就可以开始愉快的浏览网页了。  
![](/assets/chrome-socks5-use.png)
