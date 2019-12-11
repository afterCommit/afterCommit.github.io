---
layout:     post                    # 使用的布局(不需要改)
title:      Git常用commit参数       # 标题
subtitle:   有些人看上去风风光光,背地里都是我替他收蚂蚁森林的能量   #副标题
date:       2019-12-10 00:59:59 GMT+0800             # 时间
author:     Zen                 # 作者
header-img: img/photo/jiuzhaigou.webp    #这篇文章标题背景图片
catalog: False                      # 是否归档
tags:                               #标签
    - 杂谈
---

`git commit -m "message"`

-m 参数表示可以直接输入后面的提交信息

还有另外一种方法

```
git commit -m 'message1
message2
message3'
```

`git commit -a -m "massage"`

加的-a参数可以将所有已跟踪文件中的执行修改或删除操作的文件都提交到本地仓库,即使它们没有经过git add添加到暂存区,注意,\新加的文件(即没有被git系统管理的文件)是不能被提交到本地仓库的。

`git commit --amend`

如果我们不小心提交了一版我们不满意的代码,并且给它推送到服务器了,在代码没被merge之前我们希望再修改一版满意的,而如果我们不想在服务器上abondon,也叫追加提交,它可以在不增加一个新的commit-id的情况下将新修改的代码追加到前一次的commit-id中
       
