---
layout:  post
id:  350
title:  "Windows10使用技巧"
slug:  "350"
categories:  "经验分享"
tags:  "win10, 系统, 快捷键, 优化, 自定义"
permalink:  "/archives/:slug.html"
author:  "酱油"
date:  2016-12-25 00:01:00
---



Windows10在2015年7月29号正式发布RTM版，带来了更高校的运行效率、更智慧的语音助手小娜、开始菜单回归等新特性。笔者非常喜欢这款操作系统。
但系统并不适合所有人，举例来说，尽管开始菜单回归了，但并不是传统意义上的开始菜单。资源管理器原有的菜单栏也改成选项卡的形式了。这些改变可能需要大家去适应。
上面简单的介绍了一点Win10的特性，下面就来具体介绍一些适合我们读屏用户的优化方案。

<h3>恢复简体中文美式键盘</h3>
从Win8开始，英文输入法键盘和中文输入法键盘就分开了，需要按Win+空格切换不同语言的输入法，如果你不适应新的切换习惯，导入下面的注册表，找回按CTRL+Shift切换中英文输入法吧。
<a href="http://mywind.sinaapp.com/skydrive/1805BB4AF3C3BD76!4627/Win10简体中文美式键盘.reg">下载 Win10 简体中文美式键盘</a>
<h3>隐藏通知区域的输入法指示器</h3>
若要隐藏通知区域的输入法指示器图标，请按Win+I打开设置，依次进入“时间和语言 -> 区域和语言”，然后tab浏览到“其他日期、时间和区域设置 链接”然后按回车键打开“时钟、语言和区域”设置窗口，
然后tab键浏览到“更换输入法 链接”按回车键打开“语言”设置窗口，
按tab浏览到“高级设置 链接”，按回车键打开“高级设置”窗口。
按tab键找到并选中“使用桌面语言栏(可用时) 复选框”，然后按tab浏览到“单击打开语言栏选项 链接”按回车键打开“文本服务和输入语言”设置窗口，
选中设置窗口中的“隐藏(H) 单选按钮”，取消选中“在任务栏中显示其他语言栏图标(I) 复选框”，然后点击确定按钮，这样就把输入法指示器图标隐藏了。
<h3>删除此电脑置顶文件夹</h3>
微软从Win7开始引入了库的概念，有意让用户淡化文件系统的概念，而按分类来管理文件，但并不是每个人都喜欢这种方式，因此，此电脑中的这些置顶文件夹也就失去了意义。如果你打开此电脑只想看到盘符和连接的设备，不想看到这些文件夹，导入下面的注册表即可。
<a href="http://mywind.sinaapp.com/skydrive/1805BB4AF3C3BD76!4628/删除此电脑置顶文件夹.reg">删除此电脑置顶文件夹.reg</a>
<h3>卸载Win10内置应用</h3>
Win10自带了一些通用应用，NVDA对于通用应用的支持没有桌面应用支持的那么好，也许你也不喜欢，按照下面的方法就可以卸载他们。
在开始菜单所有应用中找到Windows PowerShell 文件夹，展开Windows PowerShell文件夹然后按下光标找到Windows PowerShell，按右键以管理员身份运行Windows PowerShell。
复制下面你要删除的应用名字下一行的文字，粘贴到Windows PowerShell中按回车，即可删除他们。
OneNote：
Get-AppxPackage *OneNote* | Remove-AppxPackage
3D：
Get-AppxPackage *3d* | Remove-AppxPackage
相机：
Get-AppxPackage *camera* | Remove-AppxPackage
邮件和日历：
Get-AppxPackage *communi* | Remove-AppxPackage
新闻订阅：
Get-AppxPackage *bing* | Remove-AppxPackage
Groove音乐、电影与电视：
Get-AppxPackage *zune* | Remove-AppxPackage
人脉：
Get-AppxPackage *people* | Remove-AppxPackage
手机伴侣（Phone Companion）：
Get-AppxPackage *phone* | Remove-AppxPackage
照片：
Get-AppxPackage *photo* | Remove-AppxPackage
纸牌游戏：
Get-AppxPackage *solit* | Remove-AppxPackage
录音机：
Get-AppxPackage *soundrec* | Remove-AppxPackage
Xbox：
Get-AppxPackage *xbox* | Remove-AppxPackage

<h3>显示或隐藏Win10更新</h3>
Win10会自动更新一些Windows Update中能找到的设备驱动，但有些驱动可能会引起一些问题，下载下面的文件就可以手动选择隐藏这些更新。
<a href="http://mywind.sinaapp.com/skydrive/1805BB4AF3C3BD76!4629/显示或隐藏Windows10更新.diagcab">下载显示或隐藏Win10更新疑难解答</a>

<h3>修复Win10无法启动设置</h3>
新系统的发布往往会带来一些意想不到的Bug，Win10也出现了一些让人哭笑不得的Bug，无法启动设置就是其中之一，如果你遇到了这样的问题，不妨尝试下下面的疑难解答程序。
<a href="http://mywind.sinaapp.com/skydrive/1805BB4AF3C3BD76!4630/Win10无法启动设置修复.diagcab">下载修复Win10无法启动设置疑难解答</a>

<h3>桌面创建特殊IE图标</h3>
Win10带来了全新的Edge浏览器，微软特意的将 Internet Explorer 放入了 Windows附件文件夹中，如果你是IE的忠实用户，希望在桌面上创建带有右键功能的特殊IE图标，可以导入下面提供的注册表。
<a href="http://mywind.sinaapp.com/skydrive/1805BB4AF3C3BD76!4631/给桌面创建IE图标windows7以上都可以使用内附说明.rar">下载桌面创建特殊IE图标</a>

<h3>防止Win10自动转换为平板模式</h3>
笔者层遇到过这样一种问题，按Win+M无法返回桌面，偶然发现这是因为Win10转换到了平板模式，对于非平板用户，显然不需要这样的功能，而且这个功能还会造成我遇到过的这种问题。我们可以通过下面的设置避免Win10自动转换为平板模式。
按Win+I打开设置，依次进入系统 -> 平板电脑模式，按tab键会浏览到一些组合框，
将“当我登录时”设置为 “转到桌面”，
将“当该设备自动将平板电脑模式切换为开或关时” 设置为“不询问我，不进行切换”。
这样就不用担心你的电脑自动切换成平板模式了。

<h3>在登录窗口自动启用讲述人</h3>
如果你担心NVDA的朗读安全桌面服务进程会造成系统不稳定，那么你可以利用讲述人来朗读登陆窗口。具体设置如下：
按Win+U打开轻松使用设置中心，按tab键浏览到“更改登录设置”并进入，
在“更改登陆设置”窗口中按tab键浏览到“登录时 朗读屏幕内容(讲述人)”复选框，将其选中，这样在开机进入到登陆画面时，讲述人就会自动启动为你朗读登陆窗口了。

<h3>开机自动登录Win10</h3>
如果你是用微软账户登陆的windows10，每次开机就必须输入开机密码，不想输入开机密码怎么办？windows10 现在可以免密码自动登陆了。设置方法如下：
按下Win+R快捷键，打开运行对话框，
在运行对话框中输入Control Userpasswords2，按下回车键，打开“用户账户”窗口
在打开的用户账户窗口中，取消选中“要使用本计算机，用户必须输入用户名和密码”复选框，然后点击应用按钮，（注意一定要先这么做，如果直接点击确定而不点击应用的话，有可能自动登陆设置失败。）
在之后弹出的窗口中输入你的用户名与微软账户密码，最后点击确定保存退出。
重新启动电脑后，下次开机就可以免密码自动登录了，但这样进入桌面的速度会稍微慢一些，具体根据自己的需要设置吧。

<h3>关闭快速启动</h3>
一些比较老的电脑或者硬件存在问题的电脑如果启用windows10的快速启动功能，可能会造成无法关机的情况，如果你遇到了这样的问题，按照下面的方法操作可以关闭快速启动功能。
按Win+X打开高级用户功能菜单，进入“电源选项”，
打开“电源选项”窗口后tab键浏览到“选择电源按钮的功能”进入，
然后点击“更改当前不可用的设置”。按tab找到“启用快速启动(推荐)”复选框，将其取消选中，
然后点“保存修改”按钮。这样快速启动功能就关闭了。

<h3>启用开机音乐</h3>
如果你设置了开机自动登陆，对于我们读屏用户来说，就有必要启用开机音乐了。
按Win+B定位到通知区域，找到扬声器图标，按Apps键弹出菜单，执行“声音”菜单，
打开“声音”对话框后，按tab浏览到“播放 Windows 启动声音(P)”，将这个复选框选中，然后点击“确定”按钮，下次开机就能听到开机音乐了。

<h3>Windows10快捷键</h3>

Win + A：打开通知中心

Win + B：将焦点定位到通知区域工具栏

Win + C：开始与Cortana对话

Win + D：最小化所有窗口，再次按下还原所有窗口

Win + E：打开资源管理器

Win + G：打开XBox游戏录制工具栏

Win + H：激活应用分享功能

Win + I：打开设置

\Win + K：激活无线显示器连接或音频设备连接

Win + L：锁定屏幕

Win + M：返回桌面

Win + P：打开多屏显示切换

Win + Q：打开搜索/Cortana

Win + R：打开运行对话框

Win + S：打开搜索/Cortana

Win + T：将焦点定位到任务栏

Win + U：打开轻松使用设置中心

Win + X：弹出高级用户功能菜单

Win + 上箭头：桌面模式最大化当前窗口，平板模式向上移动应用窗口

Win + 下箭头：桌面模式最小化当前窗口，平板模式向下移动应用窗口

Win + 左箭头：桌面模式将窗口最大化停靠到屏幕左边缘，平板模式向左移动应用窗口

Win + 右箭头：桌面模式将窗口最大化停靠到屏幕右边缘，平板模式向右移动应用窗口

CTRL+Win + 回车：启动讲述人(1703)

Win + =：启动放大镜

Win + 1到9：打开任务栏上对应位置固定的程序

Win + Tab：激活任务试图

Win + CTRL加D：新建虚拟桌面

Win + CTRL加F4：关闭虚拟桌面

Win + 左右箭头：切换虚拟桌面

Win + Shift + 左右箭头：将应用从一个显示屏移动到另一个显示屏


<h3>windows 10 运行命令大全</h3>
关于Windows winver 
添加设备 devicepairingwizard 
添加硬件 hdwwiz 
用户账户 netplwiz 
授权管理器 azman（Win7） 
备份和还原 sdclt 
Bluetooth文件传送 fsquirt 
计算器 calc 
证书 certmgr（Win7） 
性能选项 systempropertiesperformance 
数据执行保护 systempropertiesdataexecutionprevention 
打印机用户界面 printui 
字符映射表 charmap 
ClearType文本调谐器 cttune 
颜色管理 colorcpl 
命令提示符 cmd 
组件服务 comexp（Win7） 
组件服务 dcomcnfg 
计算机管理 compmgmt 
计算机管理 compmgmtlauncher 
连接到网络投影仪 netproj（Win7） 
显示切换 displayswitch 
控制面板 control 
创建共享文件夹向导 shrpubw 
创建系统修复光盘 recdisc 
存储的用户名和密码 credwiz 
默认位置 locationnotifications（Win7） 
设备管理器 devmgmt.msc 
Microsoft 支持诊断工具 msdt 
数字化校准工具 tabcal 
DirectX 诊断工具 dxdiag 
磁盘清理 cleanmgr 
优化驱动器 dfrgui 
磁盘管理 diskmgmt.msc 
显示 dpiscaling 
显示颜色校准 dccw 
受保护的内容迁移 dpapimig 
驱动程序验证程序管理器 verifier 
轻松使用设置中心 utilman 
加密文件系统 rekeywiz 
事件查看器 eventvwr 
传真封面编辑器 fxscover 
文件签名验证 sigverif 
Windows 入门 gettingstarted（Win7） 
IExpress 向导 iexpress 
导入 Windows 联系人 wabmig 
Microsoft iSCSI iscsicpl 
安装或卸载显示语言 lpksetup 
本地组策略编辑器 gpedit.msc 
本地安全策略 secpol.msc 
本地用户和组 lusrmgr.msc 
放大镜 magnify 
Microsoft Windows 恶意软件删除工具 mrt 
数学输入面板 mip 
MMC管理控制台 mmc 
NAP 客户端配置 napclcfg（Win7） 
讲述人设置 narrator 
扫描仪 wiaacmgr 
记事本 notepad 
ODBC 数据源管理程序 odbcad32 
屏幕键盘 osk 
画图 mspaint 
性能监视器 perfmon 
电话括号程序 dialer 
演示设置 presentationsettings 
打印管理 printmanagement.msc 
打印机迁移 printbrmui 
专用字符编辑程序 eudcedit 
步骤记录器 psr 
注册表编辑器 regedit 
远程桌面连接 mstsc 
资源监视器 resmon 
组策略结果集 rsop 
保护 Windows 账户数据库的安全 syskey 
服务 services.msc 
设置程序访问此计算机的默认值 computerdefaults 
共享文件夹 fsmgmt.msc 
截图工具 snippingtool 
录音机 soundrecorder（Win7） 
SQL Server 客户端网络实用工具 cliconfg 
便签 stikynot 
同步中心 mobsync 
系统配置 msconfig 
系统信息 msinfo32 
系统属性-高级 systempropertiesadvanced 
系统属性-计算机名 systempropertiescomputername 
系统属性-硬件 systempropertieshardware 
系统属性-远程 systempropertiesremote 
系统属性-系统保护 systempropertiesprotection 
系统还原 rstrui 
任务管理器 taskmgr 
任务计划程序 taskschd.msc 
受信任的平台(TPM)管理 tpm.msc 
用户账户控制设置 useraccountcontrolsettings 
音量合成器 sndvol 
Windows 激活 slui 
联系人 wab 
Windows 光盘映像刻录机 isoburn 
Windows 资源管理器 explorer 
Windows 传真和扫描 wfs 
Windows 功能 optionalfeatures 
高级安全 Windows 防火墙 wf.msc 
Windows 帮助和支持 winhlp32 
Windows 日记本 journal 
Windows Media Player wmplayer 
Windows 内存诊断 mdsched 
Windows 移动中心 mblctr 
Windows Powershell powershell 
Windows PowerShell ISE powershell_ise 
Windows 远程协助 msra 
Windows 脚本宿主设置 wscript 
Windows Update wuapp（Win7） 
Windows 更新独立安装程序 wusa 
WMI 管理 wmimgmt.msc 
WMI 测试器 wbemtest 
写字板 write 
XPS 查看器 xpsrchvw 
屏幕分辨率 desk.cpl 
鼠标属性 main.cpl 
安全性与维护 wscui.cpl 
网络连接 ncpa.cpl 
电源选项 powercfg.cpl 
卸载或更改程序 appwiz.cpl 
系统属性 sysdm.cpl 
Windows 防火墙 firewall.cpl 
