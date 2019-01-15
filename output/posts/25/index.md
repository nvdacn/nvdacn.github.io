---
layout:  post
id:  25
title:  "NVDA集成aisounds方法及所需资源"
slug:  "25"
categories:  "经验分享"
tags:  ""
permalink:  "/archives/:slug.html"
author:  "蓦然回首"
date:  2014-06-09 14:25:00
---



科大的aisounds音库受到了很多读屏使用者的好评，一些读屏对此作了支持，其中就包括nvda的香港版。然而香港版的更新速度有限，也就是说，如果想体验nvda最新版，就无法使用aisounds音库，这大概也就是鱼和熊掌不可兼得吧！
然而事实真的如此吗，鱼和熊掌真的不可兼得?今天，我就告诉大家，鱼和熊掌可以兼得。我们可以吧aisounds集成进最新版的nvda，方法如下：
首先，我们可以在网上获取一个香港版的nvda，将其用7z或者其他工具解包，会得到两个文件夹“$_OUTDIR”和“$PLUGINSDIR”。进入“$_OUTDIR”，吧"synthDrivers"里的"aisound.pyc","_aisound.pyc"和"hkbu_aisound.dll"复制到要集成的nvda安装目录中的"synthDrivers"里，再找到“$PLUGINSDIR”，进入“app”，找到library.zip，打开，找到synthDrivers进去，再找到“_aisound.pyo”和“aisound.pyo”，把它们复制出来，然后把扩展名改为.pyc。最后，把改好扩展名的“_aisound.pyc”和“aisound.pyc”复制进nvda安装目录下的library.zip里的synthDrivers下。至此，集成工作大功告成。
看了上面繁琐的步骤如果觉得麻烦，那么压缩包内有已经修改好的文件，只需将包内的"synthDrivers"放进要集成的nvda的安装目录，把“_aisound.pyc”和“aisound.pyc”复制进nvda安装目录下的library.zip里的synthDrivers下即可。

版权说明

本资源及说明搜集自互联网，仅供学习研究之用，不得用于商业用途，请下载后24小时内删除。对于使用本资源给您造成的损失，本人不承担任何责任。一旦您选择使用本资源即表明您已同意上述内容，否则后果自负！

<a href="http://pan.baidu.com/s/1mgJVmTa">点此下载</a>                                            