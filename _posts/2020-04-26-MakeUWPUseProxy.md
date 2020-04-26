---
layout:     post                    # 使用的布局(不需要改)
title:     为Win10-UWP应用使用设置代理             # 标题
subtitle:   我是一只被禁足的安小鸟 #副标题
date:       2020-04-26 00:00:00 GMT+0800             # 时间
author:     Zen                 # 作者
header-img: img/photo/birdAngle.webp    #这篇文章标题背景图片
catalog: False                   # 是否归档
tags:                               #标签
    - 技巧
---
Win 10 的 UWP应用（应用商店下载的APP，如OneDrive、我的世界基岩版等），默认是不走代理的（沙盒的网络隔离特性：禁止APP访问localhost ），即使使用了「小飞机」软件，UWP软件仍然无法得到加速。
网上有很多解决此类问题的方法，要不就是使用 Fiddler 软件进行设置，要不就是使用CheckNetIsolation命令来解除限制，但是需要通过注册表来获取应用的SID，都比较麻烦。
其实有一个办法，不需要下载软件，也不需要打开注册表。
----
