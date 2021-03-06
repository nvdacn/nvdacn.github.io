---
layout:  post
id:  777
title:  "NVDA2018.2更新盘点和下载"
slug:  "release"
categories:  "最新情报"
tags:  ""
permalink:  "/archives/:slug.html"
author:  "星空"
date:  2018-06-14 20:50:00
---



就在昨天，NVACCESS官方发布了最新的NVDA2018.2，这次主要整合了基本设置对话框，支持了一些盲文显示器，支持了Kindle的PC表格，完善了Onecore和Sapi5语音合成器，还改进了Microsoft Outlook。下面是具体更新日志:
2018.2
此版本的亮点包括支持Kindle的PC表格，支持Humanwear BrailleNote Touch和BI14盲文显示器，Onecore和Sapi5语音合成器的改进，Microsoft Outlook的改进等等。
新功能
NVDA 现在能用语音和盲文报告表格单元格的行和列范围。2642
Google文档现已支持NVDA表格的导航命令 以及（启用盲文模式）。7946
NVDA 当前已支持在 Kindle 上的 表格阅读 和 导航 操作。7977
通过USB和蓝牙支持BrailleNote touch和Brailliant BI 14盲文显示器。6524
在Windows 10 Fall Creators Update及更高版本中，NVDA可以报告来自应用程序（例如Calculator和Windows Store）的通知。8045
新盲文表：立陶宛8点，乌克兰语，蒙古语2级。7839
添加了一个脚本来报告特定盲文单元下文本的格式信息。7106
更新NVDA时，现在可以推迟将更新安装到计算机。4263
新增翻译: 蒙古语,瑞士德语.
您现在可以从盲文键盘切换控制，移位，替代，窗口和NVDA，并将这些修饰符与盲文输入（例如按下控制键+ s）进行组合。7306
您可以使用输入手势对话框中仿真系统键盘键下的命令来分配这些新的修改器切换。
恢复对Handy Tech Braillino和Modular（带有旧固件）的盲文显示器的支持。8016
支持的Handy Tech设备（如Active Braille和Active Star）的日期和时间现在会在NVDA超过五秒钟不同步时自动同步。8016

更改

NVDA 插件管理器中的状态列已更改，以提示插件是启用还是禁用，而不是运行或挂起。7929
更新 liblouis 盲文 翻译器到3.5.0.7839
立陶宛盲文表已更名为立陶宛6点，以避免与新的8点立陶宛盲文混淆。7839
法国（加拿大）1级和2级表已被删除。相反，将分别使用法语（统一）6点计算机盲文和2级盲文表。7839
Alva BC6，EuroBraille和Papenmeier盲文显示器上的次要路由按钮现在报告该按钮的盲文单元下文本的格式信息。7106
在不可编辑的情况下（即没有光标或浏览模式的控件），缩小盲文输入表将自动回退到未收缩模式。7306
在Microsoft Outlook消息列表中，NVDA现在会报告消息是否已被回复或转发。6911
NVDA 现在可以分配输入手势以临时禁用所有配置文件触发器。4935
现在，所有NVDA的首选项都可以在NVDA菜单 - >首选项 - >设置下的一个设置对话框中找到，而不是通过许多对话框进行分散。7302
在Windows 10上当前运行的默认语音合成器现在是oneCore语音而不是eSpeak。8176

bug修复

输入电子邮件地址后，NVDA不再无法在设置中的Microsoft帐户登录屏幕中阅读集中控件。7997
返回到Microsoft Edge中的上一页时，NVDA不再无法读取页面。7997
随着机器解锁，NVDA将不再错误地宣布Windows 10登录PIN的最终字符。7908
Chrome和Firefox中复选框和单选按钮的标签在选项卡或在浏览模式下使用快速导航时不再报告两次。7960
将咏叹调目前的值设为 false而不是 true7892
如果配置的语音已被卸载，则Windows Onecore语音合成器驱动程序不再无法加载。7999
改变Windows Onecore Voices合成器驱动程序中的声音现在速度要快得多。7999
修复了多个盲文桌面的格式错误盲文输出，包括8点缩写丹麦盲文的大写签名。7526, #7693)
NVDA现在可以在Microsoft Word中报告更多的子弹类型。6778)
按报告格式化脚本不再错误地移动reviewPosition并因此多次按下它不再给出不同的结果。7869)
盲文输入不再允许您在不受支持的情况下使用缩写盲文（即，整个单词将不再在文本内容和浏览模式之外发送到系统）。7306)
修复Handy Tech简易盲文和盲文波显示器的固定连接稳定性问题。8016
在Windows 8和更高版本中，打开快速链接菜单时，NVDA将不再宣布“未知”）Windows + X）并从此菜单中选择项目。8137
Hims显示器上按钮的模型特定手势现在按照用户指南中的说明进行操作。8096
NVDA现在将尝试纠正导致Firefox和Internet Explorer等程序无法访问的系统COM注册问题，并通过NVDA报告“未知”。2807
解决任务管理器中的错误，导致NVDA不允许用户访问有关进程的特定详细信息的内容。8147
当Outlook日历中的约会或时间段覆盖一整天时，NVDA现在不会变得冗长。7949
较新的Microsoft SAPI5语音在语音结束时不再滞后，因此使用这些语音导航效率会更高。8174
在最近版本的Windows中访问时钟时，NVDA不再以盲文或按字符语音报告（LTR和RTL标记）。5729
在一些文本控件中，特别是在Delphi应用程序中，提供的关于编辑和导航的信息现在更加可靠.8102
Hims Smart Beetle盲文显示器上滚动键的检测再次不再不可靠。6086
在Windows 10 RS5中，当使用alt +选项卡切换任务时，NVDA不再报告额外的冗余信息。8258

开发者更改

The developer info for UIA objects now contains a list of the UIA patterns available.5712
App modules can now force certain windows to always use UIA by implementing the isGoodUIAWindow method.7961
The hidden boolean flag "outputPass1Only" in the braille section of the configuration has again been removed. Liblouis no longer supports pass 1 only output.7839
<a href="https://www.nvaccess.org/files/nvda/releases/2018.2/nvda_2018.2.exe">官方下载NVDA2018.2</a>
<a href="http://www.nvdacn.com/189.php/QFrqEvBvANZf.exe">本地下载NVDA2018.2</a>
有星空编辑于2018-0614