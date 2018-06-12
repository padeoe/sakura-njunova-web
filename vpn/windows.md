# Windows
Windows创建vpn这里提供两种方式，一种是通过系统自带的引导程序创建，另一种是通过powershell命令创建，本质上没有区别。
### 通过系统引导程序
1.在网络和共享中心中“设置新的连接或网络”-“连接到工作区”-“否，创建新连接”-“使用我的Internet连接”-“Internet地址：sakura.njunova.com,目标名称随意填写”-"创建"

![](/assets/windows-m1-step1.png)
![](/assets/windows-m1-step2.png)
![](/assets/windows-m1-step3.png)
![](/assets/windows-m1-step4.png)
![](/assets/windows-m1-step5.png)

2.在系统网络中找到创建的VPN连接，点击连接，输入用户名密码。

![](/assets/windows-m1-step6.png)

### 通过Powershell命令
运行命令
```
Add-VpnConnection -Name njunova -ServerAddress sakura.njunova.com -AuthenticationMethod Eap -EncryptionLevel Required -RememberCredential -TunnelType Ikev2
```
后系统网络中找到新创建的名为njunova的VPN点击连接。