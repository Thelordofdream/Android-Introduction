# 创建Android新项目
* 点击"Start a new Android Studio project"；  

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/016.png onload = 'this.width=400'/></div>  

* 命名Application name，如需要则修改Project location，点击"Next"；

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/023.png onload = 'this.width=400'/></div>

* 选择想要的Phone and Tablet的Minimum SDK(最低适配的安卓系统版本)，最好选择为Android 6.0+，因为出于设备安全与用户数据的安全考虑，Android 6.0上相比之前的历史版本各种功能的权限门槛都有所提升，并引入了新的分级的权限体系，因此编程上差异会比较大，旧版本的程序并不能适应新版本对权限管理的要求，当然考虑到应用的用户群数量，也可根据选择框下文字提示的覆盖设备比例选择合适的SDK，之后点击"Next"；  

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/024.png onload = 'this.width=400'/></div>  

* 选择Project类型，建议选择Basic Activity，点击"Next"；  

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/025.png onload = 'this.width=400'/></div>  

* 设置Activity Name（主界面名），可以不做修改，点击"Finish"；  

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/026.png onload = 'this.width=400'/></div>  * 如果VPN支持[HTTPS]协议，则点选"Enable HTTPS Proxy"，一般VPN都支持且大部分自动下载的必须内容都是HTTPS协议的，所以建议点选，点击"OK"；  

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/027.png onload = 'this.width=400'/></div>  

* 新的项目已经创建完成，等待Android Studio自动启动项目并Build Gradle即可。

对于Windows端的读者，如果无法点击"Start a new Android Studio project"，则表示当前Android Studio的JDK 或者 Android SDK 目录指向有问题。那么你可以选择 Configure --> Project Defaults --> Project Structure，进入SDK和JDK路径的配置页面，将安装JDK的路径和SDK的目录确认配置好。  

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/028.png onload = 'this.width=400'/></div>  

如对文本内容有改进建议或者反对意见者，可致信笔者电子邮箱告知笔者进行修改:<574483817@qq.com>。

[HTTPS]:https://zh.wikipedia.org/zh-hans/超文本传输安全协议