# Android Studio工程目录简介  

Android项目开发主要的工作在app这个目录下，Android高级开发会涉及到Gradle Scripts目录下的文件，接下来介绍app目录下的各文件作用：  
* Manifests一级子目录下的AndroidManifest.xml文件中，包含了这个app需要的系统权限，app的图标依赖文件名，app的名字依赖变量名，app的主题依赖对象；  
* Java一级子目录下的第一个二级子目录下的MainActiviy文件，是一个java程序，也就是app中MainActivity（主界面）对应的后台程序逻辑。开发者编写的语句、监听都在OnCreate方法（本质是主线程）中实现，“全局变量”的声明和子线程、异线程、自定义方法在OnCreate方法前@Override之上实现；  
* Java一级子目录下的第二个二级子目录下的ApplicationTest文件，是基本依赖文件，无需编写，具体作用请读者自行了解；  
* Res一级子目录下的drawable目录默认为空，开发者可以向其中添加工程所需的图片或者自定义的xml依赖文件；  
* Res一级子目录下的layout目录包含了app所有的前端界面xml文件，activity_main.xml就是主界面的依赖文件，其中包含了所有UI控件及其属性，开发者在这个文件中添加修改UI控件，点击底部的Design/Text可以切换界面的图形设计模式和程序设计模式，开发者在图形设计模式中可以直接拖动UI控件实现布局；  
* Res一级子目录下的menu目录包含了app的菜单栏依赖文件menu.xml，读者可自行了解；  
* Res一级子目录下的mipmap二级子目录中的ic_launcher.png三级子目录包含了各种分辨率下的app图标文件，均为png格式，开发者可以通过修改图标文件的指向路径来修改app的图标；  
* Res一级子目录下：
	* values二级子目录中包含了该工程下的宏变量：dimens.xml包含了所有尺寸的宏定义变量，此处开发者可以定义一些常用的尺寸；	* strings.xml包含了所有字符串的宏定义变量，此处开发者可以修改“app_name”的宏定义内容来修改app名字；	* styles.xml包含了app的style类型，修改：  
`<style name="AppTheme" parent= "Theme.AppCompat.Light.DarkActionBar"> `
 中的语语句内容即可改变app的风格，例如改为：  
`parent= "Theme.AppCompat.Light.NoActionBar"`

<div align="center"><image src = https://raw.githubusercontent.com/Thelordofdream/Android-Introduction/master/images/029.png onload = 'this.width=400'/></div>
