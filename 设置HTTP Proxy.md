# 设置HTTP [Proxy]
成功进入以后，会看到如下界面：
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/016.png onload = 'this.width=400'/></div>  

* 点击右下角"Configure"按钮；
* 点击"Preferences"选项，进入设置界面；
* 选择父级菜单"Appearance & Behavior"；  
* 选择一级子菜单"System Settings"；
* 选择"HTTP Proxy"选项； 

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/019.png onload = 'this.width=200'/></div>  
 
* 在右侧界面，选择"Manual proxy configuration"。

## 基于[HTTP]协议的VPN  
以基于HTTP协议的鱼摆摆为例，应填写配置信息如下：  

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/017.png onload = 'this.width=400'/></div>  

* 选择协议为"HTTP"；  
* 本地[Host name]一般情况下为127.0.0.1；  
* 鱼摆摆的[Port number]一般情况下为9743；
* 无需帐号免费VPN后面的Proxy authentication不需要填写；
* 点击"Apply"应用设置。  

## 基于[SOCKS]协议的VPN
以基于SOCKS5协议的Shadowocks为例，应填写配置信息如下：
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/018.png onload = 'this.width=400'/></div>  

* 选择协议为"SOCKS"；
* 本地Host name一般情况下为127.0.0.1；
* Shadowsocks的Prot number一般情况下为1080，ShadowsocksX-NG的为1086；
* 无需账户登录的情况下，Proxy authentication不需要填写；
* 点击"Apply"应用设置。 

而后保持VPN正常运行，准备开始下载SDK和自动更新Gradle。  

如对文本内容有改进建议或者反对意见者，可致信笔者电子邮箱告知笔者进行修改:<574483817@qq.com>。


[Proxy]:https://zh.wikipedia.org/wiki/代理服务器
[HTTP]:https://zh.wikipedia.org/wiki/超文本传输协议
[SOCKS]:https://zh.wikipedia.org/wiki/SOCKS
[Host name]:https://zh.wikipedia.org/wiki/主機名稱[Port number]:https://zh.wikipedia.org/wiki/通訊埠 
