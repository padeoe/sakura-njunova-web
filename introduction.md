﻿本服务器提供三种网络服务：VPN，HTTPS代理和Socks5代理，那么它们各自有何特点呢，该如何选择呢？  

服务名|不需要客户端|跨平台跨应用|域名分流|速度稳定
---|---|---|---|---
VPN|✓|✓||✓
HTTPS代理|✓||✓|
Socks代理|||✓|✓

（上表所述并非绝对，譬如VPN也可以域名分流，只是本站不支持）

## VPN
#### 全局性
本服务器提供的是IKEV2/L2TP的VPN。是一种全局代理上网方式。
全局性既是VPN的优点（可对设备上所有程序进行代理），又是其缺点（有些程序无需爬墙，耗费流量；无法分流，访问国内网站卡顿）。
#### 全平台支持，无需客户端
几乎所有系统都原生支持。

## HTTPS代理
本服务器提供的HTTPS代理并非标准SSL HTTP代理，只有Chrome配合代理插件才能使用。因此只能用于桌面系统（Windows+Mac OS+Linux）的Chrome浏览器。
#### 无需客户端，可分流
十分适合浏览网页，无需后台运行客户端，且可以使用插件分流。
#### 速度不稳定
由于HTTPS代理加密传输，会受到GFW的随机丢包，因此速度不稳定，看网页不成问题，但大流量下载就会体现出来。

## Socks代理
本服务器的Socks代理实则是经过改进的Socks代理。原生的Socks代理是明文传输，访问“非法”网站会直接被墙。由于改进的Socks代理需要加密，因此需要客户端。譬如Shadowsocks就是一种基于Socks5的代理。本服务器的YSocks代理暂时只提供Windows平台的客户端。