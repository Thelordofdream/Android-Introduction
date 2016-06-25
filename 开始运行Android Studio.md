# 开始运行Android Studio 
## Windows端
打开Android Studio，进入相关的配置页面。在导入Android studio的配置文件的界面，如果是第一次安装，选择最后一项：不导入配置文件，然后点击OK即可。之后，程序会开始检查SDK的更新情况，但是此时因为防火墙的缘故，程序将无法连接到谷歌服务器并进行正常的更新，因此需要先跳过SDK的更新检查直接开始建立工程，操作如下:  

* 在Android Studio安装目录下的 bin 目录下，找到 idea.properties 文件，在文件最后追加disable.android.first.run=true;
* 关闭Android Studio后重新启动，便可进入界面;

如果读者后期需要更新SDK，需先设置Android Studio的HTTP配置环境中的Proxy Settings根据VPN的设置填写[Host Name][]、[Port Number][]等内容，使Android Studio在VPN开启时以这个配置连接谷歌服务器。之后，读者就可以在开启VPN后，更新Android Studio的SDK了。如果读者之前下载了Recommended版本，并没有必要时常进行更新。

## macOS端
首先，需要更改JDK的版本信息:  

* [Finder]中，应用程序中找到Android Studio;
* 右击显示包内容，在目录下找到 info.plist 并用任意文本编辑器打开;
* 找到 JVMVersion 并将\<string>1.6*\</string>中的版本号改为当前系统JDK的版本号(即刚才下载的JDK的版本号，可在设置-Java中查看)(注意：Android Studio只支持JDK1.6及以上版本);

然后设置以跳过SDK的更新:

* 进入应用程序，找到Android Studio，右键-->显示包内容-->Contents-->bin，找到文件idea.properties，使用文本工具打开;
* 在idea.properties文件末尾添加一行:disable.android.first.run=true，然后保存文件;
* 关闭Android Studio后重新启动，便可进入界面;

如果用户需要更新SDK，则操作与Windows端一致。  
如对文本内容有改进建议或者反对意见者，可致信笔者电子邮箱告知笔者进行修改:<574483817@qq.com>。[Host Name]:https://zh.wikipedia.org/wiki/主機名稱[Port Number]:https://zh.wikipedia.org/wiki/通訊埠  
[Finder]:https://zh.wikipedia.org/wiki/Finder  
