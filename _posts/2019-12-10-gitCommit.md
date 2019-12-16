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


开始跟踪新文件/把已跟踪的文件放到暂存区

`git add main.go`

提交修改到本地

`git commit`

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
       
推送提交的修改到远程

`git push git@url.git gethistory_api`

克隆现有代码库

`git clone git@url.git`

可选指定文件夹名

`git clone git@url.git dirName`

查看文件状态

`git status`

查看当前频道

`git branch -a`

克隆指定分支的代码库

`git clone -b <branchName> git@url.git`

分支是用来将特性开发绝缘开来的在你创建仓库的时候,`master`是`默认的`分支在其他分支上进行开发,完成后再将它们合并到主分支上

创建一个叫做`feature_x`的分支,并切换过去:

`git checkout -b feature_x`

切换回主分支:

`git checkout master`

再把新建的分支删掉:

`git branch -d feature_x`
除非你将分支推送到远端仓库,不然该分支就是不为他人所见的:

`git push origin <branch>`
### 建立本地分支与远程分支的映射关系(或者为跟踪关系track)
```
//这样使用git pull或者git push时就不必每次都要指定从远程的哪个分支拉取合并和推送到远程的哪个分支了.

$ git branch -vv
// 输出映射关系

// dev为远程分支名
$ git branch -u origin/dev
// 将当前本地分支与远程分支建立映射关系

$ git branch --unset-upstream
//撤销当前本地分支与远程分支的映射关系
```
