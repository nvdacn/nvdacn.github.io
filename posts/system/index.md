---
layout:  post
id:  784
title:  "当系统出现严重问题时，利用系统自带命令修复Windows10系统 无需重装(by)目光"
slug:  "system"
categories:  "经验分享"
tags:  ""
permalink:  "/archives/:slug.html"
author:  "星空"
date:  2018-10-14 18:25:00
---



我们日常使用系统偶尔出现一些小问题。有些小伙伴系统出问题第一反应是重装或者还原。今天我给朋友们带来另一种解决方法。利用微软系统自带命令工具修复。以此扩展大家的眼界与思路。希望能够给大家有所帮助。我就不废话了，直接给大家上干货。

## 第一种是利用sfc命令、
sfc本地系统文件检测，管理员命令提示符窗口输入：sfc 
SFC [/SCANNOW] [/VERIFYONLY] [/SCANFILE=<file>] [/VERIFYFILE=<file>]
    [/OFFWINDIR=<offline windows directory> /OFFBOOTDIR=<offline boot directory> [/OFFLOGFILE=<log file path>]]

/SCANNOW        扫描所有保护的系统文件的完整性，并尽可能修复
                有问题的文件。
/VERIFYONLY     扫描所有保护的系统文件的完整性。不会执行修复
                操作。
/SCANFILE       扫描引用的文件的完整性，如果找到问题，则修复文件。
                指定完整路径 <file>
/VERIFYFILE     验证带有完整路径 <file> 的文件的完整性。
                不会执行修复操作。
/OFFBOOTDIR     对于脱机修复，指定脱机启动目录的位置
/OFFWINDIR      对于脱机修复，指定脱机 Windows 目录的位置
/OFFLOGFILE     对于脱机修复，通过指定日志文件路径选择性地启用记录

示例:

        sfc /SCANNOW
        sfc /VERIFYFILE=c:\windows\system32\kernel32.dll
        sfc /SCANFILE=d:\windows\system32\kernel32.dll /OFFBOOTDIR=d:\ /OFFWINDIR=d:\windows
        sfc /SCANFILE=d:\windows\system32\kernel32.dll /OFFBOOTDIR=d:\ /OFFWINDIR=d:\windows /OFFLOGFILE=c:\log.txt
        sfc /VERIFYONLY

## 第二种是利用Dism命令、
Dism部署映像服务和管理工具，联网校验检查修复。管理员命令提示符窗口输入：Dism

部署映像服务和管理工具
版本: 10.0.17763.1

DISM.exe [dism_options] {Imaging_command} [<Imaging_arguments>]
DISM.exe {/Image:<path_to_offline_image> | /Online} [dism_options]
         {servicing_command} [<servicing_arguments>]

描述:

  DISM 枚举、安装、卸载、配置和更新 Windows 映像
 中的功能和程序包。可以使用的命令取决于提供的映像
 以及映像是处于脱机还是运行状态。


通用映像处理命令:

  /Split-Image            - 将现有 .wim 文件拆分为多个
                               只读拆分 WIM (SWM) 文件。
  /Apply-Image            - 应用一个映像。
  /Get-MountedImageInfo   - 显示有关安装的 WIM 和 VHD 映像的
                            信息。
  /Get-ImageInfo          - 显示有关 WIM、VHD 或 FFU 文件中映像的
                                 信息。
  /Commit-Image           - 保存对装载的 WIM 或 VHD 映像的更改。
  /Unmount-Image          - 卸载已装载的 WIM 或 VHD 映像。
  /Mount-Image            - 从 WIM 或 VHD 文件装载映像。
  /Remount-Image          - 恢复孤立的映像装载目录。
  /Cleanup-Mountpoints    - 删除与损坏的已安装映像
                            关联的资源。

WIM 命令:

  /Apply-CustomDataImage  - 冻结自定义数据映像中包含的文件。
  /Capture-CustomImage    - 将自定义设置捕获到 WIMBoot 系统上的增量 WIM 文件中。
                            捕获的目录包括所有
                            子文件夹和数据。
  /Get-WIMBootEntry       - 显示指定磁盘卷的
                            WIMBoot 配置项。
  /Update-WIMBootEntry    - 更新指定磁盘卷的
                            WIMBoot 配置项。
  /List-Image             - 显示指定映像中的文件
                            和文件夹的列表。
  /Delete-Image           - 从具有多个卷映像的 WIM 文件
                            删除指定的卷映像。
  /Export-Image           - 将指定映像的副本导出到其他
                            文件。
  /Append-Image           - 将其他映像添加到 WIM 文件中。
  /Capture-Image          - 将驱动器的映像捕获到新的 WIM 文件中。
                            捕获的目录包含所有子文件夹和
                            数据。
  /Get-MountedWimInfo     - 显示有关安装的 WIM 映像的信息。
  /Get-WimInfo            - 显示有关 WIM 文件中的映像的信息。
  /Commit-Wim             - 保存对安装的 WIM 映像的更改。
  /Unmount-Wim            - 卸载安装的 WIM 映像。
  /Mount-Wim              - 从 WIM 文件安装映像。
  /Remount-Wim            - 恢复孤立的 WIM 安装目录。
  /Cleanup-Wim            - 删除与损坏的已安装 WIM
                            映像关联的资源。

FFU COMMANDS:

  /Capture-Ffu            - Captures a physical disk image into a new FFU file.
  /Apply-Ffu              - Applies an .ffu image.
  /Split-Ffu              - Splits an existing .ffu file into multiple read-only
                            split FFU files.

映像规格:

  /Online                 - 以正在运行的操作系统为目标。
  /Image                  - 指定脱机 Windows 映像的根目录的路径。

DISM 选项:

  /English                - 用英文显示命令行输出。
  /Format                 - 指定报告输出格式。
  /WinDir                 - 指定 Windows 目录的路径。
  /SysDriveDir            - 指定名为 BootMgr 的系统加载程序文件的路径。
  /LogPath                - 指定日志文件路径。
  /LogLevel               - 指定日志(1-4)中所示的输出级别。
  /NoRestart              - 取消自动重新启动和重新启动提示。
  /Quiet                  - 取消除错误消息之外的所有输出。
  /ScratchDir             - 指定暂存目录的路径。

若要获得有关这些 DISM 选项及其参数的详细信息，请在紧挨着 /? 之前指定一个选项。

  示例:
    DISM.exe /Mount-Wim /?
    DISM.exe /ScratchDir /?
    DISM.exe /Image:C:\test\offline /?
    DISM.exe /Online /?

常用命令示例:

1.检查

联网在线扫描映像来检查损坏。管理员命令提示符窗口输入：Dism /Online /Cleanup-Image /ScanHealth  
这条命令将扫描全部系统文件并和官方系统文件对比，扫描计算机中的不一致情况，扫描完成后会有提示。

连网在线检查报告，管理员命令提示符窗口输入：Dism /Online /Cleanup-Image /CheckHealth
注意：这条命令必须在前一条命令执行完以后，发现系统文件有损坏时使用。

当使用 /CheckHealth 参数时，DISM 工具将报告映像是状态良好、可以修复、还是不可修复。如果映像不可修复，必须放弃该映像，并重新开始。如果映像可以修复，可以使用 /RestoreHealth 参数来修复映像。

2.修复

若扫描出系统中的不一致情况，检测到系统中存在损坏的文件，并报告映像是状态良好、可以修复等，就可以用 /RestoreHealth 参数进行修复。
连网在线映像文件中与官方文件在线修复，管理员命令提示符窗口输入：DISM /Online /Cleanup-image /RestoreHealth
这条命令是把那些不同的系统文件还原成官方系统源文件，其他的第三方软件和用户设置完全保留，比重装好多了。而且在扫描与修复的时候系统未损坏部分正常运行，电脑可以照常工作。

联网无法修复的多尝试几次，使用挂载本地文件较为繁琐，

或者，若要使用你自己的一些来源，不使用 Windows 更新来修复一个联机映像。如下：
本地自定义映像文件修复，管理员命令提示符窗口输入：Dism /Online /Cleanup-Image /RestoreHealth /Source:路径\windows /LimitAccess

例如这样： Dism /Online /Cleanup-Image /RestoreHealth /Source:c:\test\mount\windows /LimitAccess
注：解释下上面命令的意思，test\mount\windows这个windows实际上说的是从ISO镜像的wim中提取的，然后解压在test\mount目录下，此方法不建议新手使用，麻烦。

好了，就说到这里了，假如遇到问题无法还原后不想重装系统，不放考虑下以上方法。

部分资料引用来源于[蓝点网](https://www.landiannews.com/archives/897.html)