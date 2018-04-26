全部是c盘 安装有一个建立一个WAMP文件夹
1、win7系统安装Visual C++ Redistributable for Visual Studio 2012 Update 4
win7步骤php环境-上课====》Apache(VC11)-不支持xp与serv03==》Visual C++ Redistributable for Visual Studio 2012 Update 4 成功之后不会有显示，只是显示会成功
注意：都是向导安装


2、现在开始安装Apache php环境-上课====》Apache(VC11)-不支持xp与serv03==》Apache 2.4.x VC11文件下的httpd-2.4.27-x64-vc11.zip放在c盘下建立一个WAMP，把这个Apache 2.4.x VC11文件下的httpd-2.4.27-x64-vc11.zip
在WAMP文件夹下解压然后点进去===》httpd-2.4.27-x64-vc11===》Apache24下===》bin里面  单击空白处 开启命令行shift  右键
c:\WAMP\httpd-2.4.27-x64-vc11\Apache24\bin>  然后输入httpd（是一个端口号）
会出现一连串英文串这是报错现象  然后去bin同级下的conf进去==》httpd.con httpd - 副本.conf复制一个更改前先复制一个副本 f右键用编辑器打开更改 38行
Define SRVROOT "C:/WAMP/httpd-2.4.27-x64-vc11/Apache24"
ServerRoot "${SRVROOT}"
然后把上面的命令关掉==》新开 window快捷键 cmd右键以管理员身份打开  输入地址  cd /中间是空格 斜线是正斜线 意思根目录下然后回车
==》每次都以cd 开头意思是进入，依次把你哪个目录下的文件名输入进去 每次都是cd 空格 文件下一直找到bin目录下
然后输入httpd是端口号一个编号，-k 然后stop 按完之后看services.msc 就不启动了  httpd -k start 看services.msc又启动了==》httpd -k uninstall就把services.msc里面的apche还在右键停止就没有了
httpd -k install安装成功刷新services.msc 让他启动httpd -k start就启动了
然后出现c:\WAMP\httpd-2.4.27-x64-vc11\Apache24\bin> 要正斜线才是对的 C:/WAMP/Apache 2.4.x VC11/Apache24按httpd回车下面有一个横线在闪烁，说明可以了，然后去谷歌浏览器输入127.0.0.1地址，有页面出现说明成功
cmd


3、现在是php环境
php\PHP环境-20170905\PHP_win\PHP 5.6 (5.6.31)\VC11 x64 Thread Safe (2017-Jul-06 174139)php-5.6.31-Win32-VC11-x64
安装php-5.6.31-Win32-VC11-x64解压到和wamp文件下的httpd-2.4.27-x64-vc11和这个文件夹同级打开这个问件夹
有一个这个php.ini-development意思是开发阶段用这个，产品阶段用下面的，然后复制一个副本php.ini-development 改名为php.ini
然后打开httpd-2.4.27-x64-vc11==》Apache24==》htdocs把里面的内容改掉他是根目录你的所有的网站都在这个里面==》conf==》
httpd.conf用编辑器打开更改下面的地址
注意路径一定要对
#使得apache 加载php模块
LoadModule php5_module "C:\WAMP\php-5.6.31-Win32-VC11-x64\php5apache2_4.dll"

#告知apache什么后缀的文件让php处理
AddType application/x-httpd-php .php

#加载php的配置文件
PHPIniDir "C:\WAMP\php-5.6.31-Win32-VC11-x64\php


注意参考文档在安装WAMP环境-说明
数据库也要在wamp下安装
4、数据库安装目录php\PHP环境-20170905\MySQL_win\MySQL_5.6.37_win详情看安装WAMP环境-说明





下面咱们两个一起安装你别弄了网易弄坏了就不好了
5、node环境直接傻瓜式安装  测试安装是否成功cmd窗口node -v 可以看到版本然后npm install less -g检查版本 lessc -v可以看到版本
npm install -g nodemon
npm config set registry https://registry.npm.taobao.org下载之后不会有任何变化就说明安装成功
在用户下.npmrc文件
npm install http-server -g
npm install babel-cli -g
npm install webpack -g
查看http-server可以访问127.0.0.1：8080 要在项目下打开

6、git 密钥配置

7、nvm配置

多版本安装方式

- 卸载已有的Node.js
- 
下载nvm
- 在C盘创建目录dev
- 
在dev目中创建两个子目录nvm和把nodejs
 
并且把nvm里 1)elevate.cmd 2)elevate.vbs 3)install.cmd 4)LICENSE 5) nvm.exe删掉
修改文件中配置信息
- 配置nvm和Node.js环境变量（我的电脑右键属性==》高级系统设置==》系统属性===》高级===》环境变量）
  
新建两个值 1) NVM_HOME:C:\dev\nvm
     2) NVM_SYMLINK:C:\dev\nodejs
- 
把配置好的两个环境变量加到系统环境  环境变量 ==》Path中==》编辑
- 
;%NVM_HOME%;%NVM_SYMLINK%; 确定保存 检查一下在不在


打开nvm-setup.zip压缩包压缩在别的目录下（他是一个nvm-setup.exe文件）
开始安装 第一个路径配置C:\dev\nvm 第二个路径配置C:\dev\nodejs 一路是就可以
 
最后dev下的Node.js
- （删除）
nvm常用的命令

- nvm list 查看当前安装的Node.js所有版本
- 

1）命令nvm use 版本号 选择指定版本的Node.js

2)查看dev下多了一个nodejs文件并且有一个勾选意思是快捷方式 意思是使用那个出来那个版本




