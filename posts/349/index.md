---
layout:  post
id:  349
title:  "无法直接修改快捷键的插件如何来修改快捷键（附案件表）"
slug:  "349"
categories:  "经验分享"
tags:  "插件, 快捷键, 热键, 输入手势"
permalink:  "/archives/:slug.html"
author:  "酱油"
date:  2015-10-08 18:26:00
---



随着NVDA插件的增多，难免会出现插件与插件、插件与NVDA之间的快捷键冲突。也许你也想把各种插件的快捷键改成你习惯的按键。可是很多插件还不支持通过NVDA的“输入手势”设置来更改热键。下面笔者就教大家来修改无法通过“输入手势”修改的插件快捷键。
  首先进入NVDA用户配置目录，打开开始菜单，进入所有应用，展开NVDA子菜单，执行“浏览NVDA用户配置目录”菜单。
然后进入用户配置目录中的addons文件夹。接下来找到你要修改快捷键的插件文件夹，进入插件文件夹后再进入globalPlugins文件夹。
一些不太复杂的插件，在globalPlugins文件夹中就可以找到Python脚本文件，有些插件需要再进入子文件夹。
一般开发者不想加密的话都会保留源代码文件，扩展名是“.py”，我们就是要改这个“.py”文件，不用管后面的“.pyo”或者“.pyc”文件。。
找到“.py”文件后，按apps键（即右键），弹出上下文菜单，找到打开方式，选择用记事本打开。
记事本加载完py文件后，按CTRL+F弹出查找对话框，搜索“kb:”（不含双引号），这样就能找到脚本文件中定义的快捷键了，按照这个方式依次查找脚本文件中的快捷键进行修改，修改完直接按CTRL+S保存。
重启NVDA后，或者执行重新加载插件命令后，修改的快捷键就生效了。
若修改快捷键后出现插件不稳定或者快捷键更混乱的情况，那就直接重装插件吧。
下面附上一些键盘按键在Py脚本中的写法，多数字母键、数字键和符号键写法就是他们本身。

窗口键: windows
CTRL键: control
Shift键: shift
Alt键: alt
ESC键: escape
F1: f1
F2: f2
F3: f3
F4: f4
F5: f5
F6: f6
F7: f7
F8: f8
F9: f9
F10: f10
F11: f11
F12: f12
暂停键: pause
滚动锁定键: scrolllock
回车键: enter
Apps键: applications
空格键: space
退格键: backspace
NVDA键: nvda
删除键: delete
行首键: home
行尾键: end
上翻页键: PageUp
下翻页键: PageDown
上箭头: uparrow
下箭头: downarrow
左箭头: leftarrow
右箭头: rightarrow
小键盘1: numpad1
小键盘2: numpad2
小键盘3: numpad3
小键盘4: numpad4
小键盘5: numpad5
小键盘6: numpad6
小键盘7: numpad7
小键盘8: numpad8
小键盘9: numpad9
小键盘除号: numpaddivide
小键盘乘号: multiply
小键盘减号: numpadminus
小键盘加号: numpadplus
小键盘删除: numpaddelete
小键盘回车: numpadenter
