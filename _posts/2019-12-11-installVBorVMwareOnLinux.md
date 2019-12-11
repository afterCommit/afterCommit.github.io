---
layout:     post                    # 使用的布局(不需要改)
title:      在Linux下安装Virtual Box或VMware workstation Pro       # 标题
subtitle:   老同学聚会,发现贫富差距特别大,有些人穷,而有些人更穷   #副标题
date:       2019-12-11 00:59:59 GMT+0800             # 时间
author:     Zen                 # 作者
header-img: img/photo/jiuzhaigou.webp    #这篇文章标题背景图片
catalog: True                      # 是否归档
tags:                               #标签
    - 常识
---
# Virtual Box
是一款免费的虚拟机软件
## 下载
进入[VB官网Linux分支](https://www.virtualbox.org/wiki/Linux_Downloads)选择你电脑的发行版下载deb/rpm包

[下载扩展工具包](https://download.virtualbox.org/virtualbox/6.0.14/Oracle_VM_VirtualBox_Extension_Pack-6.0.14.vbox-extpack)

## 安装
打开终端cd到下载目录
输入

`sudo dpkg -i *.deb`

如果没有报错就安装完了
否则

`sudo apt-get -f install`

接下来看个人喜好决定是否安装扩展工具包,安装方法与Windows平台相同,不在教程范围内

# VMware workstation Pro
是一款收费的虚拟机软件
## 下载

## 安装
