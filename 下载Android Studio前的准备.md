# 下载Android Studio前的准备 
## [VPN][]
因为[GFW][]的存在，开发者在国内会无法访问Google Android的一些官方网站，更要重要是在Android Studio版本更新、SDK下载和Build [Gradle][]的时候将无法连接到谷歌服务器。所以在开始下载安装Android Studio之前，读者需要自备[翻墙][]的工具。依据个人经验而言，做Android开发如果没有具备翻墙的技能，几乎是寸步难行的。  
鉴于绝大部分免费翻墙软件都存在速度慢、不稳定、内容不纯净的问题，笔者在这里就直接推荐读者使用付费VPN。Windows平台上，笔者推荐“[云梯][]”；Mac OS平台上，笔者推荐“[鱼摆摆][]”。这两款VPN价格都很便宜，而且比较稳定，后者的速度偏慢一点但已经够用了。如果读者自己配备了私有的VPN服务器，自然是最好的。

## [JDK][]
### 下载JDK
在开始基于[Java][]的Android开发之前，首先需要为自己的电脑安装Java JDK(Java Development Kit，面向开发者的Java组件)，搭建一个Java的开发环境和运行环境。  
* 登录[Oracle(甲骨文)][]官网Java下载页面:
<http://www.oracle.com/technetwork/java/javase/downloads/index-jsp-138363.html>;
* 点击页面中的“JDK Download”进入JDK的下载页面:
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/001.png onload = 'this.width=400'/></div>
* 点击“Accept License Agreement”同意许可;
* 根据电脑情况选择适配的JDK版本，[Windows][] [32位][]电脑选择下载 “Windows [x86][]”，Windows [64位][]电脑选择下载“Windows [x64][]”，[Mac OS][]平台选择下载“[Mac OS X][]”;
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/002.png onload = 'this.width=400'/></div>
* 点击左侧下载链接下载;
* 双击Java JDK安装包“jdk-8u71-windows-x64”;
* 点击“Next”（"下一步"）按钮;
* 选择需要安装的功能后，点击“Next”（“下一步”）按钮;
* 等待安装结束。

如需验证Java JDK是否安装成功，可  

* 打开[命令提示符(cmd)][];
* 运行命令“java -version”;
* 命令行返回正确的java信息，即为安装成功。

Mac OS平台的安装过程类似以上步骤，其中在Mac OS上验证Java JDK需要打开[Terminal终端][]而指令相同，也可以在[Safari][]中通过Ocrale提供Java在线验证。
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/011.png onload = 'this.width=500'/></div>
### 配置[环境变量][]
下一步我们需要配置环境变量。在Windows平台上(以[Windows 8.1][]为例):  
* 右键“开始按键”点击“系统”;
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/003.png onload = 'this.width=300'/></div>* 点击“高级系统设置”;
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/004.png onload = 'this.width=400'/></div>* 点击“环境变量”;
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/005.png onload = 'this.width=400'/></div>
* 打开环境变量设置窗口;
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/006.png onload = 'this.width=400'/></div>
* 在“系统变量”下点击“新建”，设置变量名为: JAVA_HOME，变量值为JDK安装目录，如: C:\Program Files\Java\jdk1.8.0_25 ;
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/007.png onload = 'this.width=400'/></div>
* 再点击“新建”，设置变量名为: CLASSPATH，变量值为: .;%JAVA_HOME%\lib\tools.jar;%JAVA_HOME%\lib\dt.jar *(注意：点号表示当前目录，不能省略)*;
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/008.png onload = 'this.width=400'/></div>
* 选择变量名为：Path的变量，点击“编辑”，在变量值的最前面添加字段: ;%JAVA_HOME%/bin; *(注意:这里的分号不能省略)*;  
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/009.png onload = 'this.width=400'/></div>
<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/010.png onload = 'this.width=400'/></div>  
如对文本内容有改进建议或者反对意见者，可致信笔者电子邮箱告知笔者进行修改:<574483817@qq.com>。[VPN]:https://zh.wikipedia.org/wiki/虛擬私人網路
[GFW]:https://zh.wikipedia.org/wiki/防火长城
[Gradle]:https://zh.wikipedia.org/wiki/Gradle
[翻墙]:https://zh.wikipedia.org/wiki/突破网络审查
[云梯]:https://www.ytpub.com
[鱼摆摆]:https://ybb1024.com
[JDK]:https://zh.wikipedia.org/wiki/JDK
[Java]:https://zh.wikipedia.org/wiki/Java
[Oracle(甲骨文)]:https://zh.wikipedia.org/wiki/甲骨文公司
[Windows]:https://zh.wikipedia.org/wiki/Microsoft_Windows
[32位]:https://zh.wikipedia.org/wiki/32位元
[x86]:https://zh.wikipedia.org/wiki/X86
[64位]:https://zh.wikipedia.org/wiki/64位元
[x64]:https://zh.wikipedia.org/wiki/X86-64
[Mac OS]:https://zh.wikipedia.org/wiki/Mac_OS
[Mac OS X]:https://zh.wikipedia.org/wiki/OS_X
[命令提示符(cmd)]:https://zh.wikipedia.org/wiki/命令提示字元
[Terminal终端]:https://zh.wikipedia.org/wiki/终端_(OS_X)
[Safari]:https://zh.wikipedia.org/wiki/Safari
[环境变量]:https://zh.wikipedia.org/wiki/环境变量
[Windows 8.1]:https://zh.wikipedia.org/wiki/Windows_8.1