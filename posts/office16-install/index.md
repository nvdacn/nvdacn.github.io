---
layout:  post
id:  661
title:  "漫辰推荐-Office2016-Install自定义安装工具"
slug:  "office16-install"
categories:  "经验分享"
tags:  ""
permalink:  "/archives/:slug.html"
author:  "星空"
date:  2017-01-26 13:56:00
---



软件简介：

Office 2016 Install 5.3 绿色汉化中文版由大眼仔旭汉化发布。
Office 2016 Install 是由国外软件爱好者 Ratiborus 开发的一款针对微软发布的 Office 2016 及组件在线下载安装工具。它不仅是一款在线 Office 2016 下载安装工具，还可以用于 Office 2016 离线安装包的组件自定义安装，如果你只想安装 Word/Excel/PowerPoint 或者只想安装其中一款软件，Office 2016 Install 就是最简单的辅助安装工具。
此外，它还可以用于强制卸载 Office,对解决 Office 安装失败而造成的无法再次安装的问题提供了解决方法。

PS:
大眼仔旭只是汉化了软件，而英文版的说明文档并没有翻译，为了方便大家使用，我翻译以下重要内容，有翻译不当之处望各位海涵。
--------------------
后面是Advanced，能用到的朋友肯定不用我在这儿啰嗦，另外，为什么我要使用最新的office呢？
一是因为我们的NVDA完整支持了最新的office办公套件，以下言论皆基于此。
二是我是个喜欢挑战，愿意适应新事物的人，尽管对于2003有诸多不舍，我深知，那不过是习惯使然而已
三身为一名不折不扣的学生党，学会Office的应用只能是有利无弊。
四一个资深老盲的虚荣心作祟，为什么他们可以，而我也有条件做到却不去争取。？
倘若你的想法与我不谋而合，那么欢迎，我们一起学习，共同进步。
联系方式：
QQ： 603715146
E-mail： manchen_0528@outlook.com

-------

翻译开始
设计此程序的目的是用于在线安装和激活Microsoft Office 2013/2016 C2R。当然，你也可以用它创建Office离线自定义安装包以供日后使用。
如何使用本工具呢？
1. 删除现有版本的office2016（可以通过控制面板 > 添加或删除程序）
2. 使用本工具强制删除office并重新启动计算机。
3. 单击“安装Office”按钮，安装Office。
注： 在安装前推荐您选自己所需。
 4.安装完毕，在本程序“实用程序”选项卡，执行“Office 零售转批量版”按钮。
 5.然后单击“激活 Office”按钮。
或者
 6.启动KMSAuto Net 2015并单击“激活Office”按钮。
PS: KMSAuto Net 2015这款激活工具与此工具师出同门。

如何使用书签下载Office：
书签下载—用于创建不同版本的Microsoft Office的离线安装包，具有随后安装产品而无需从外部下载或接收文件的可能性。

1.选择适当的Office版本和语言。我建议创建一个完整的x86-x64发行版。
为此，请选择“下载 Office”选项卡，组合框内选择"all"，单击下载按钮并选择一个目录用于存储文件。
您可以选择程序上一次创建的目录以进一步扩展它，或开始一个新的创建过程。
2.  当你已经创建了一个版本之后，而你又要进行多语言版本的增量，请选中另外的语言，单击下载按钮，并选择相同的下载目录。
3.下载完所有需要的版本和语言后，推荐创建ISO镜像。
为此，请单击“创建ISO”。
4. 完毕之后，在选定的目录下，您将看到一个现成的Microsoft Office离线安装程序。
注： 选择版本。
在相同的增量中，只可以增量语言和位宽，而不能增量版本。及： 2013和2016不能使用同一目录，只能创建于不同的文件夹，否则您将无法使用。
5. 现在，你可以创建多个项目，或添加、更正已下载的项目。对于Office 2013软件总会下载最新版。然而对于Office 2016，您可以在下载前点击“获取版本”按钮以检查新的版本。


------------------


			   Advanced startup options (keys):
                 ——————————————————————————————————————————————————

/configure "d:\MyPath\Configuration.xml"    - Launch the program in hidden mode, and perform the installation.
or
/proplus x64 en-us excludeExcel excludeOneNote /apps visio
or
/apps x64 ru-ru en-us word excel visio
or
/proplus x86 en-us excludeOneNote /apps project /convert /activate


Changes in versions:
————————————————————
v5.3
 -Changes in program for compatibility with antivirus software.

v5.2
- New Office 2016 Deployment Tool

v5.1
- New Office 2013 Deployment Tool

v5.0
- New Office 2016 Deployment Tool

v4.9
 -Small changes to the interface.

v4.8
- For Office 2013 and Office 2016 used different lists available languages.
- Fixed bug  for creating a task to reactivate in the Task Scheduler.

v4.7
- "Force Remove Office C2R/MSI" button removes all traces of Office 2013/2016 C2R and MSI.

v4.6.1
- Fixed: Uninstall Office 2013/2016.

v4.6
- Added "Search for new version."
- Added language et-EE, ms-MY.
- Added button "Create ISO"
- Downloading of distribution can be interrupted.

v4.5
- Added support for Office 2013 C2R.
- Added "Download Office".
- Added language kk-KZ.

v4.4
- Fixed: the work program from ReadOnly disc.

v4.3
- Immediately after installation of Office the button "Office RETAIL => VL" operates in the forced mode,
  you can the conversion without starting the Office application.
- Added language hu-HU.

v4.2
- Added the ability to create a task scheduler for reactivation Office.

v4.1
- Added conversion RETAIL => VL and activation of Office 2010/2013/2016.

v4.0
- Added language nl-NL, lt-LT, sv-SE, sk-SK, sr-latn-rs.
- Integrated newer version OffScrubc2r.vbs, version 1.95 is replaced by 1.97,
  (you must delete the folder files).
- New Office 2016 Deployment Tool
- Added the installation of Office 2016 Mondo.

v3.9
- The program was renamed in "Office 2016 Install", executable file - O16Install.exe
- Added languages ​​nb-NO, ro-RO, el-GR, th-TH.
- Running the program with command line parameters.

v3.8
- The program is a single file that can be placed in the root of original ISO or DVD.

v3.7
- Added languages ​​lv-LV, ko-KR, ar-SA, fi-FI, pt-PT, pl-PL, cs-CZ, da-DK.
- Changes in the program interface.
- The program works with ReadOnly disc.

v3.6
- Added languages ​​sl-SI, ja-JP.
- Changes in the program interface.
百度网盘下载
<a href="http://pan.baidu.com/s/1jIRZHga">百度云下载Office2016Install5.3绿色汉化中文版</a>
密码： nvda
