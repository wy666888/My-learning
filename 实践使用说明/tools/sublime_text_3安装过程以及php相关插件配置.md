# [sublime_text_3 安装](http://www.cnblogs.com/yi220284/p/6367098.html)
  

安装Package Control 
通过 ctrl+` 快捷键或者 View > Show Console菜单打开控制台，复制粘贴回车如下代码即可
import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)

Package Control的使用方法：安装插件
快捷键 Ctrl+Shift+P（菜单 – Tools – Command Paletter），输入 install 选中Install Package并回车，输入或选择你需要的插件回车就安装了（注意左下角的小文字变化，会提示安装成功）。

遇到的问题
当点击 Package Control: Install Package时，会出现如下的报错：
Package Control
There are no packages available for installation
出现的原因：
This error is happened with IPv6 problem. If your Internet Service Provider (ISP) does not support for IPv6 you will get this error.
解决方案(OSX/Linux/Ubuntu/CentOS/etc..)：
sudo echo "50.116.34.243 sublime.wbond.net" >> /etc/hosts

sublime_text_3 常用的php插件
安装步骤》Ctrl + Shift + P 调用出Sublime Text, 点击 Package Control: Install Package,出现了输入框，输入要安装的插件名，回车进行安装即可

SublimeLinter 
用于高亮提示用户编写的代码中存在的不规范和错误的写法，支持 JavaScript、CSS、HTML、Java、PHP、Python、Ruby 等十多种开发语言
SublimeCodeIntel
自动代码提醒+当前文件内函数定义等跳转插件，能够在当前文件内的代码互相跳转，同时支持当前所有项目目录下面代码的自动识别跳转
BracketHighlighter
高亮显示匹配的括号、引号和标签
PHP Code Beautifier
PHP代码美化插件
DocBlockr
自动给函数变量增加注释功能
Emmet
快速生成HTML代码段的插件
htmlpretty 
代码格式化，支持js css html 
如果使用Thinkphp框架进行开发，可以使用Thinkphp插件进行开发
相关介绍如下：http://www.thinkphp.cn/extend/257.html


参考来源：
http://www.cnblogs.com/etiao/p/5423141.html  
http://www.jianshu.com/p/87f87b0e3df7  
http://blog.csdn.net/gui8304451/article/details/51105198  
https://stackoverflow.com/questions/25105139/sublime-text-2-there-are-no-packages-available-for-installation  
http://www.thinkphp.cn/extend/257.html  



