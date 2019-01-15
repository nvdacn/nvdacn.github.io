---
layout:  post
id:  114
title:  "鼠标导航插件 3.7正式版 3.8测试版"
slug:  "114"
categories:  "插件下载"
tags:  "插件, 鼠标, 移动"
permalink:  "/archives/:slug.html"
author:  "酱油"
date:  2016-07-10 17:42:00
---



鼠标导航 
版本： 3.7正式版、3.8测试版
作者：沉浮
此插件通过设置一系列键盘快捷键对鼠标指针进行上，下，左，右四个方向移动，
其移动幅度可根据设置屏幕分辨率或是屏幕等分成百分比，
在移动过程中会时时读出鼠标指针所在处的显示信息，
同时也通过beep音调高低变化和左右声道的音量大小，让视障者可以时时觉察出鼠标指针大概是到了屏幕的左边或右边（左右是通过左右声道的音量变化区分),上下（通过beep声音调高低区分）。
这个插件的目的是为了补全nvda不能精确地用键盘来移动鼠标的功能。
在作者的努力下，所谓的“路标”功能正式被引入到NVDA中来，对于经常接触无障碍程度差的软件用户而言意义非凡。股民们一直期待的定点监视这次也一并实现了，连一向被吐槽的鼠标跟随问题也得到了添加。
txt太大不好找？用插件添加书签吧。
下面让我们一览这位“大神”的尊荣，看看这款装机必备的使用方法吧：
#3.8更新日志
增加居于窗口的百分比浏览模式，当鼠标处于限制模式且是百分比浏览状态时此功能生效。

### 3.7更新日志 ###
1.增加书签功能。在一般文档中（网业除外），可按 nvda+windows+小键盘7 逐个添加书签，数量不限，快速按下此快捷键两次清除当前标题下的所有书签，快捷键 nvda+windows+小键盘9 按照顺序依次跳转至保存书签的位置。（注：书签是根据当前的标题来区分，遇到不同的标题会保存不同的书签）
2. 优化定点监视，遇到监视对象退出时会自动停止监视
3. 在插件退出时自动停止线成，nvda不会因此而卡住
4. 对一些快捷键作了重新设置，详情请参见本文档。
### 3.6.1 更新日志 ###
1. 在开启鼠标跟随后，遇到菜单项目将不会自动跟随。
2. 可自动保存鼠标跟随的设置。
### 鼠标导航及窗口监视 ###
台式电脑快捷键
nvda+control+小键盘2 鼠标下移
nvda+control+小键盘8 鼠标上移
nvda+control+小键盘4 鼠标左移
nvda+control+小键盘6 鼠标右移
nvda+control+小键盘5（1次） 读出当前鼠标所在屏幕的位置
nvda+control+小键盘5（2次） 打开鼠标导航设置窗口
nvda+control+小键盘1 屏幕像素模式与屏幕分辨百分比模式切换
nvda+alt+小键盘减号 限制鼠标在当前焦点所在程序的开关
nvda+ctrl+小键盘回车 定点监视开关（请使用鼠标选择需要监视的丶）
nvda+windows+小键盘回车 全屏监视开关
nvda+windows+小键盘减号 鼠标跟随浏览光标开关
小键盘丶号 拷贝鼠标所指对象的名称
NVDA+windows+小键盘 7 为非网页文档添加书签
NVDA+windows+小键盘 9 跳转到下一个已有书签
笔记本电脑快捷键（全局）：
windows+control+下光标 鼠标下移
windows+control+上光标 鼠标上移
windows+control+左光标 鼠标左移
windows+control+右光标 鼠标右移
windows+control+回车（1次） 读出当前鼠标所在屏幕的位置
windows+control+回车（2次） 打开鼠标导航设置窗口
windows+control+f12 屏幕像素模式与屏幕分辨百分比模式切换
windows+alt+e 限制鼠标在当前焦点所在程序的开关
windows+alt+f8 定点监视开关（请使用鼠标选择需要监视的丶）
windows+alt+n 全屏监视开关
Windows+alt+x 鼠标跟随浏览光标开关
windows+alt+c 拷贝鼠标所指对象的名称
windows+alt+4 添加书签
windows+alt+5 切换到下一个书签
### 路标控制 ###
台式电脑 
nvda+control为组合键，加上以下小键盘的操作：
加号，下一个路标
减号，上一个路标
星号，下一个方案
除号，上一个方案
3，打开方案管理
点号，直接以当前对象名称作为路标名保存路标
小键盘7 打开保存路标对话框 
小键盘9 打开路标列表对话框 
小键盘减号 跳到上一个路标 
小键盘加号 跳到下一个路标 

笔记本方案
alt+windows+左光标 上一个路标
alt+windows+右光标 下一个路标
alt+windows+上光标 上一个方案
alt+windows+下光标 下一个方案
control+windows+f9 打开方案管理
control+windows+删除键 直接以当前对象名称作为路标名保存路标
control+windows+f11 打开保存路标对话框 
control+windows+f10 打开路标列表对话框 

### 插件窗口热键 ###
f1 保存当前鼠标位置
f2 鼠标移动时音效开关
f3时时读出鼠标指针处信息开关
回车 执行输入命令


<a accesskey="x" href="http://12355939.d.yyupload.com/down/12355939/nvdacn/addons/鼠标导航 3.7.nvda-addon">本地下载1：鼠标导航V3.7正式版</a>
<a accesskey="x" href="http://www.nvdacn.com/189.php/YfEzeefUVzie.nvda-addon">本地下载2：鼠标导航V3.7正式版</a>
<a accesskey="x" href="http://www.nvdacn.com/189.php/Mz67bqMfiyyq.nvda-addon">本地下载2：鼠标导航V3.8测试版</a>
<a accesskey="x" href="https://eyun.baidu.com/s/3coreyE">百度盘备用下载：鼠标导航（提取密码mWMr）</a>