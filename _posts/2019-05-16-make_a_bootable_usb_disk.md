---
layout:     post                    # 使用的布局（不需要改）
title:      用Rufus不费脑制作启动盘               # 标题
subtitle:   瀚海阑干百丈冰,酸脱羟基醇脱氢  #副标题
date:       2019-05-16              # 时间
author:     Zen                      # 作者
header-img: img/pet/supremelysab-787607-unsplash.webp   #这篇文章标题背景图片
catalog: False                       # 是否归档
tags:                               #标签
    - 操作系统
---
之前写过使用软碟通制作启动盘的教程，但毕竟那是个正版收费的软件，估计王涛也觉得自己很冤，又因为之前写的软碟通的教程只适用在Windows平台，如果想做Linux甚至Macos需要手动更改的地方太多，不是一种大众的等级，所以又写了这个用[Rufus](https://rufus.ie/)制作启动盘的教程

### 在浏览器上搜索Rufus，如果用Google，第一个搜索结果就是，其它搜索引擎就不一定了

![1](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/Make_Bootable_USB/1.webp)

### 进入官网，这个官网外观很特别，外观不像的网站就是你找错了

![2](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/Make_Bootable_USB/2.webp)

### 找到下载的位置，前两个都可以，没啥区别

![3](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/Make_Bootable_USB/3.webp)

### 下载完了直接双击打开就能用

![4](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/Make_Bootable_USB/4.webp)

### 如果是首次安装运行的话，会询问你是否联网更新，选否就行，大家都懂

![5](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/Make_Bootable_USB/5.webp)

### 重点来了

![6](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/Make_Bootable_USB/6.webp)

**设备** 选择你的U盘/内存卡，总之选择你要制作为系统盘的磁盘

**引导类型** 选择你下载的系统镜像(镜像可以去[msdn.itellyou.cn](https://msdn.itellyou.cn)下载，**站长只是收集了微软官方的下载链接，然而有些人用了带广告的PE安装原装系统，反咬这位站长一口，真替他喊冤**)

**镜像选项** 只在你选择Windows10或Windows8.x的时候才会出现，选择标准安装就行，Windows To Go 是安装系统到U盘上运行的

**目标系统类型** 和 **分区类型** 的对应关系如下

主板启动方式|应该选择的分区类型|应该选择的目标系统类型
---|:--:|---:
UEFI|GPT|UEFI(非CSM)
Legacy|MBR|BIOS(或UEFI-CSM)

剩下的参数不要动，有疑问私聊

### 制作成功

![7](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/Make_Bootable_USB/7.webp)

看似七步，实际上手动操作的时间加起来也就喝口咖啡的时间。选择Rufus的另一个原因就是它可以在你安装小众Linux发行版的时候自动下载引导文件，不过既然你都会安装Linux了，这软件对你来说就太小儿科了
