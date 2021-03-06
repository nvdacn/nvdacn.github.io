---
layout:  post
id:  781
title:  "NVDA2018.3.2更新检报"
slug:  "update20183-2"
categories:  "最新情报"
tags:  ""
permalink:  "/archives/:slug.html"
author:  "星空"
date:  2018-09-18 16:10:00
---



* NVDA2018.3.2次要版已发布，主要修复了使用google chrome 浏览twitter推文闪退的BUG。
** 各位好，NVDA2018.3如期而至的发布了，这次稳定版主要支持了盲文点显器的自动检测，新的Windows 10 表情符号输入面板，和其他错误修复，这次新功能不多，下面发上更新日志：**
# 2018.3#
- 此版本的新特姓包括支持许多盲文点显器的自动检测，支持新的Windows 10 表情符号输入面板，以及其他错误修复。-
## 新特性##
- 当Mozilla Firefox和Google Chrome中的网页提供语法检查信息时，NVDA将朗读语法错误。 (#8280)
- 现在标记为在网页中插入或删除的内容在Google Chrome中朗读。 (#8558)
- NVDA内用BrailleNote做盲文显示器时，增加了对BrailleNote QT和Apex BT滚轮的支持。 (#6316)- (#5992, #5993)
- 在Foobar2000中添加了用于报告当前曲目的已用时间和总时间的脚本。 (#6596)
- 使用任何合成器读取文本时，现在会朗读Mac Command键。 (#8366)
- 现在，所有Web浏览器都支持通过aria-roledescription属性的自定义标签。 (#8448)
- 新的盲文表: 捷克语8点电脑点字, 中库尔德语一级点字, 世界语一级点字, 匈牙利语一级点字, 匈牙利语八点电脑点字. (#8227)- (#8226, #8437)
- 新增后台自动检测盲文显示器功能。 (#1271)
 - 目前支持ALVA，Baum / HumanWare / APH / Orbit，Eurobraille，Handy Tech，Hims，SuperBraille和HumanWare BrailleNote和Brailliant BI / B盲文点显器。
 - 您可以通过NVDA设置的盲文选项中的盲文显示列表选择自动选项来启用此功能。
 - 有关其他详细信息，请参阅用户指南。
- 现在，Mozilla Firefox 63支持使用ARIA标签块引用的内容。 (#8577)
- 添加了最近Windows 10版本中新引入的各种现代输入功能支持。包括表情符号面板（Fall Creators Update），听写（Fall Creators Update），硬件键盘输入建议（2018年4月更新）和云剪贴板粘贴（2018年10月更新）。 (#7273)
## 修改##
- “NVDA常规设置”对话框中可用语言的列表现在将根据语言名称进行排序而不是ISO 639代码。 (#7284)
- 为所有支持的Freedom Scientific盲文显示器添加alt shift标签和windows标签的默认手势。 (#7387)
- 对于ALVA BC680和协议转换器的点显器，现在可以为左右智能平板，拇指和etouch键分配不同的功能。 (#8230)
- 对于ALVA BC6点显器，键组合sp2 + sp3现在将公布当前日期和时间，而sp1 + sp2模拟Windows键。 (#8230)
- 如果用户在自动检查更新时想向NV Access发送NVDA使用情况统计数据，则会在NVDA启动时询问用户一次。 (#8217)
- 当重装或检查更新时，如果用户同意向NV Access发送使用统计数据，NVDA现在将发送当前使用的合成器驱动程序和盲文显示器的名称，以帮助更好地确定这些驱动程序的未来开发顺序。 (#8217)
- 更新liblouis盲文翻译器版本到3.6.0。 (#8365)
- 更新正确的俄罗斯八点盲文表的路径。 (#8446)
- 更新eSpeak-ng1.49.3开发板 commit 910f4c2 (#8561)
## 错误修复##
- 当标签没有以内容本身的形式出现时，浏览模式下可以更容易地报告Google Chrome浏览器中控件的可访问标签。 (#4773)
- Zoom现在支持通知。例如，包括静音/取消静音状态和传入消息。(#7754)
- 在浏览模式下，切换盲文上下文显示不再导致盲文输出停止跟随。 (#7741)
- 修复ALVA BC680盲文点显器不再间歇性地无法初始化的BUG。 (#8106)
- 默认情况下，当按下涉及sp2 + sp3的键组合以触发内部功能时，ALVA BC6显示将不再执行模拟系统键盘键。 (#8230)
- 按ALVA BC6显示屏上的sp2以模拟alt键现在可以像宣传的那样工作。 (#8360)
- NVDA不再朗读冗余键盘布局更改。 (#7383, #8419)
- 现在，在包含超过65535个字符的文档中，鼠标跟踪在记事本和其他纯文本编辑控件中更加准确。 (#8397)
- NVDA将识别Windows 10和其他现代应用程序中的更多对话框。 (#8405)
- 修复在Windows 10 10月2018更新和服务器2019及更高版本上，当应用程序冻结或充斥事件时，NVDA不再无法跟踪系统焦点。 (#7345, #8535)
- 现在，用户在尝试读取或复制空状态栏时会收到通知。 (#7789)
- 修复了如果控件先前已被检查过半，则在语音中未报告控件上的“未检查”状态的情况的bug。 (#6946)
- 修复在NVDA的常规设置中的语言列表中，在Windows 7上正确显示缅甸语的语言名称。 (#8544)
- 在Microsoft Edge中，NVDA将朗读通知，例如读取视图可用性和页面加载进度。 (#8423)
- 修复与其他多行文本字段类似，当以盲文定位在文档的开头时，现在平移显示，使得文档的第一个字符位于显示的开头。 (#8406)
- 当导航到Web上的列表时，如果Web作者提供了标签，NVDA现在将朗读其标签。 (#7652)
- 当手动将功能分配给特定盲文点显器的手势时，这些手势现在总是显示为分配给该显示器。以前，它们显示为被分配到当前活动的点显器。 (#8108)
- 支持64位版本的Media Player Classic。 (#6066)
- 启用了UI自动化的Microsoft Word中对盲文支持的一些改进：
 - 与其他多行文本字段类似，当以盲文定位在文档的开头时，现在平移显示，使得文档的第一个字符位于显示的开头。 (#8406)
 - 在聚焦Word文档时，减少语音和盲文中过于冗长的焦点显示。 (#8407)
 - 盲文中的光标路由现在可以在Word文档的列表中正常工作。 (#7971)
 - 在Word文档中新插入的项目符号/数字可以在语音和盲文中正确朗读。 (#7970)
- 在Windows 10 1803及更高版本中，如果启用了“使用Unicode UTF-8支持全球语言”功能，则现在可以安装插件。 (#8599)
## 开发者更改##
- Added scriptHandler.script, which can function as a decorator for scripts on scriptable objects. (#6266)
- A system test framework has been introduced for NVDA. (#708)
- Some changes have been made to the hwPortUtils module: (#1271)
 - listUsbDevices now yields dictionaries with device information including hardwareID and devicePath.
 - Dictionaries yielded by listComPorts now also contain a usbID entry for COM ports with USB VID/PID information in their hardware ID.
- Updated wxPython to 4.0.3. (#7077)
- As NVDA now only supports Windows 7 SP1 and later, the key "minWindowsVersion" used to check if UIA should be enabled for a particular release of Windows has been removed. (#8422)
- You can now register to be notified about configuration saves/reset actions via new config.pre_configSave, config.post_configSave, config.pre_configReset, and config.post_configReset actions. (#7598)
 - config.pre_configSave is used to be notified when NVDA's configuration is about to be saved, and config.post_configSave is called after configuration has been saved.
 - config.pre_configReset and config.post_configReset includes a factory defaults flag to specify if settings are reloaded from disk (false) or reset to defaults (true).
- config.configProfileSwitch has been renamed to config.post_configProfileSwitch to reflect the fact that this action is called after profile switch takes place. (#7598)
- UI Automation interfaces updated to Windows 10 October 2018 Update and Server 2019 (IUIAutomation6 / IUIAutomationElement9). (#8473)
*** 日志就到这而了，大家也许看完以后觉得这次的新功能真的不多，可以说大部分是已修复维主。但是，大家不要气馁，NVDA是不会让用户失望的。大家期待NVDA2018.4的发布吧！我们NVDA2018.4再见。
[下载NVDA2018.3.2](https://www.nvaccess.org/files/nvda/releases/2018.3.2/nvda_2018.3.2.exe)