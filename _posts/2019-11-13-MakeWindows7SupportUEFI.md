---
layout:     post                    # 使用的布局(不需要改）
title:      魔改Windows7支持UEFI       # 标题
subtitle:   2019年双11发展方向:把优惠券藏在大兴安岭丛林深处一颗四百年古树右后方300英尺的刘姓土拨鼠家的车库里，在2小时内找到土拨鼠一家并在车库前合影留念，即可获得5元优惠券  #副标题
date:       2019-11-13 00:59:59 GMT+0800             # 时间
author:     Zen                 # 作者
header-img: img/photo/jiuzhaigou.webp    #这篇文章标题背景图片
catalog: False                       # 是否归档
tags:                               #标签
    - 操作系统
---

对于有特殊需求的人群,Windows7才是他们需要的操作系统,现在的廉价笔记本很多都是纯efi了,Windows7却原生不支持uefi启动,以下是解决方法
----
1. 从Windows8的安装文件中提取
`Bootmgr.efi`
2. 文件重命名为
`BOOTX64.EFI`
3. 拷贝到win7ISO的
`\EFI\Boot\`下
没有BOOT文件夹新建一个
`Bootmgr.efi`
也可以从已经安装好的Win8/10系统获得
路径`%SystemRoot%\boot`
4. 将修改过的ISO文件[制作为启动盘](https://zhangyiming748.github.io/2019/05/16/make_a_bootable_usb_disk/)
进入安装界面[正常安装](https://zhangyiming748.github.io/2019/05/20/install_win7/)
