---
layout:     post                    # 使用的布局(不需要改)
title:      用Rufus不费脑制作PE              # 标题
subtitle:   我是一只被禁足的安小鸟  #副标题
date:       2020-02-17              # 时间
author:     Zen                      # 作者
header-img: img/pet/supremelysab-787607-unsplash.webp   #这篇文章标题背景图片
catalog: True                       # 是否归档
tags:                               #标签
    - 操作系统
---
首先说明PE只是用来维护系统而不是重装系统的工具,不多说,你细品
----
原料:
  - Rufus
  - 根据个人喜好选择的PE镜像
  - U盘(容量由镜像大小决定)
----

# 天才第一步

插入U盘,打开Rufus,选择PE,选择MBR或GPT,制作,打完收工

# 配图

![插入一个正常的U盘]()<center>插入一个正常的U盘</center>
![打开Rufus]()<center>打开Rufus</center>
![选择这个U盘]()<center>选择这个U盘</center>
![选择已经下载好的PE镜像]()<center>选择已经下载好的PE镜像</center>
![选择MBR/GPT]()<center>选择MBR/GPT</center>
![不要更改默认设置]()<center>不要更改默认设置</center>
![开始制作]()<center>开始制作</center>
![最后一次确认]()<center>最后一次确认</center>
![制作完成]()<center>制作完成</center>
关闭电脑后,打开电源长按F12(部分新款Thinkpad需要开机先按回车之后再按F12,部分华硕机型热键是DEL),选择这个U盘,enter进入
![启动PE]()<center>启动PE</center>
![进入PE]()<center>进入PE</center>
然后就像使用正常电脑一样,把电脑里重要的文件复制出来,粘贴到外部存储器上(移动硬盘什么的),然后就可以重装这台电脑了
可以参考
[系统盘安装原版Win10](https://zhangyiming748.github.io/2019/05/19/install_win10/)
和
[制作系统盘](https://zhangyiming748.github.io/2019/05/16/make_a_bootable_usb_disk/)
