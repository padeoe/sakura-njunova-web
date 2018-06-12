# HTTPS代理的使用
## 1.安装Chrome浏览器和SwitchyOmega插件
Chrome的官方下载地址 ：[Chrome](https://www.google.com/intl/en/chrome/browser/desktop/index.html?standalone=1)。  
SwitchyOmega插件可在[Chrome商店](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif?hl=en)或者[Github](https://github.com/FelisCatus/SwitchyOmega/releases)下载，

本站的离线安装包：   
[windows 32位Chrome(55.0.2883.87)](https://proxy.njunova.com/file/ChromeStandaloneSetup.exe)   
[windows 64位Chrome(55.0.2883.87)](https://proxy.njunova.com/file/ChromeStandaloneSetup64.exe)   
[SwitchyOmega.crx](https://proxy.njunova.com/file/SwitchyOmega.crx)
## 2.在插件中配置代理
打开swichy omega的配置界面，新建情景模式-代理服务器，如图填写，确保协议是HTTPS，服务器地址是proxy.njunova.com,端口是5678.并点击端口右边的锁状图标🔒，填写用户名密码。  
填写完毕后，点击应用更改。   
![](/assets/chrome-conf.png)
## 3.使用代理
在浏览器右上角选中刚才创建的代理，就可以开始愉快的浏览网页了。  
![](/assets/use-proxy-in-chrome.png)
