---
layout:  post
id:  773
title:  "让nvda“”“飞”起来"
slug:  "733"
categories:  "经验分享"
tags:  ""
permalink:  "/archives/:slug.html"
author:  "打酱油"
date:  2018-03-13 21:26:00
---



多年以来，nvda以“慢”著称，大家不愿意把他用起来，这个原因占主要。几年过去了，nvda仍然是那么“慢”吗？其实不然。下面分享一系列电脑优化设置，让你的nvda“飞”起来。
第一、加快nvda启动速度。从windows8开始，微软开始引入按优先级顺序启动的模式，故此，为了开机速度有个好看的数字，微软把许许多多程序排在了开机之后。值得注意的是，微软为无障碍程序“开绿灯”了。设置方法为：
1、打开开始菜单/开始屏幕，键入“轻松访问中心”（不包括引号），在windows10下的搜索结果为“轻松使用设置中心”，照样打开即可；
2、点击“使用没有显示的计算机”链接，打开“使用没有显示的计算机”窗口；
3、勾选“nvda”复选框并点击确定，第一步设置完成。
第二、发挥电脑的真正性能，让nvda“飞”起来。通常情况下，为了适应不同的使用需要，厂商都会为电脑们设置各种各样的电源方案。其中最常见的当属“平衡”了，这个方案的设置介乎于电量和性能之间，为电量和性能取得有效平衡。然而很多时候，省电可能并不是最重要的，牺牲速度才是最可怕的。笔者一度认为电源方案设置意义有线，区别不大，直到我也买了属于自己的笔记本。为了让电脑的真正性能发挥起来，我们可以把电源方案修改成高性能，设置方法为：
1、按windows+x组合件，打开超级菜单；
2、在其中选择“移动中心”，打开“Windows 移动中心”窗口。
3、在“选择一个电源计划”组合框把电源方案改成“高性能”并直接关闭窗口即可，这样被禁锢已久的cpu等就可以放飞自我，你的nvda也就可以放飞自我了。
第三、修改nvda进程优先级，让系统资源分配更实时。此处设置方法可能因系统而有所差异，因为我手上并没有windows8/8.1的机器，所以请各位自行摸索吧。大体思路为，进入任务管理器，找到nvda.exe和nvdaRemoteHelperLoader.exe，把优先级改成实时即可。下面以windows10为例，其他系统思路相近：
1、按ctrl+shift+esc组合件打开任务管理器窗口，windows由于为其增加了许多保护措施，加载速度非常缓慢；
2、找到“详细信息”选项卡；
3、在列表中选中nvda.exe（NvdaRemoteHelperLoader.exe也相同）；
4、按应用建或使用鼠标右键弹出菜单，找到“优先级”子菜单；
5、最后选择实时并点击“更改优先级”按钮关闭窗口，关闭任务管理器即可完成设置。
第四、nvda虽然速度变快了，但是读起来太啰嗦，咋整？方法仍然是有的，以浏览网页为例
，excel、word等办公套件需要的是精度，可酌情勾选：
先引用nvda帮助原文
9.1.12. 文档格式设置 (NVDA+control+d)
此对话框可以在“选项”菜单下的“文档格式...”找到。
此对话框的大多数复选框都是用来配置，在您用光标浏览整个文档时朗读什么类型的格式信息。 例如，如果您选择了“朗读字体名称”复选框，每次您用光标进入拥有不同字体的文本时，字体名称就会被读出。
文档格式信息已经被编成群组了。 您可以配置的朗读有：
• 字体
◦ 字体名称
◦ 字体大小
◦ 字体属性
◦ 强调
◦ 缩进
◦ 颜色
• 文档信息
◦ 注释
◦ 编辑者修订
◦ 拼写错误
• 页面和间距
◦ Page numbers
◦ 行数
◦ 行首缩进提示方式 (关闭，语音，声音，语音和声音)
◦ 段落缩进 (例如悬挂式缩进，首行缩进)
◦ 行间距 (单行行间距，双倍行间距等)
◦ 对齐方式
• 表格信息
◦ 表格
◦ 行/列标题
◦ 单元坐标
• 元素
◦ 标题
◦ 链接
◦ 列表
◦ 引用区
◦ 路标
◦ 框架
◦ 可点击
-如果某些东西可点击 -
要想在任何地方切换这些设置，可在输入手势对话框设置一个自定义手势
浏览网页时建议保留的设置为：
链接
标题
路标
表格信息如有读取网页内容的特殊需求，请按需勾选。
经过这么一番设置之后，nvda将变得更快，朗读内容变得更加精准，使用愉快！