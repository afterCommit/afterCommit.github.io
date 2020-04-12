---
layout:     post                    # 使用的布局(不需要改)
title:      日报             # 标题
subtitle:   我是一只被禁足的安小鸟 #副标题
date:       2020-04-12 00:00:03 GMT+0800             # 时间
author:     Zen                 # 作者
header-img: img/photo/birdAngle.webp    #这篇文章标题背景图片
catalog: False                    # 是否归档
tags:                               #标签
    - 学习
---

|时间|内容|细节|
|:------:|:---:|:---:|
|2020/04/11|||
|15:30-16:30|leetcode上做题:1.两数之和|使用快慢指针循环遍历方法实现,之后又想是否可以目标和减去第一个小于和的数,再去寻找切片中是否有这个差|
|16:30-16:50|解决git报错`ssh_exchange_identification: read: Connection reset by peer`|解决方法`$ rm ~/.ssh/known_hosts`|
|16:50-20:11|上面的方法无效,全部删除后重新生成,怀疑是之前使用的新英体育公司邮箱的配置无效导致的|尝试的方法<br>`ssh-keygen -t rsa -b 4096 -C "zhangyiming748@gmail.com"`<br>`git config --global user.name "zen"`<br>`git config --global user.email "zhangyiming748@gmail.com"`<br>`ssh-keygen -t rsa -C "zhangyiming748@gmail.com"`<br>`ssh-keygen -t rsa -C 'zhangyiming748@gmail.com'`<br>`ssh -v git@github.com`|
|2020.4.12|||
|9:37-10:30|了解锁和原子操作的关系||
|10:59-11:50|了解死锁和活锁||
|12:00-13:30|了解redis五种数据类型的底层实现||
|13:30-13:50|整理笔记||
