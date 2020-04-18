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
|15:30-16:30|leetcode1.两数之和|使用快慢指针循环遍历方法实现,之后又想是否可以目标和减去第一个小于和的数,再去寻找切片中是否有这个差|
|16:30-16:50|解决git报错`ssh_exchange_identification: read: Connection reset by peer`|解决方法`$ rm ~/.ssh/known_hosts`|
|16:50-20:11|上面的方法无效,全部删除后重新生成,怀疑是之前使用公司邮箱的配置无效导致的|尝试的方法<br>`ssh-keygen -t rsa -b 4096 -C "zhangyiming748@gmail.com"`<br>`git config --global user.name "zen"`<br>`git config --global user.email "zhangyiming748@gmail.com"`<br>`ssh-keygen -t rsa -C "zhangyiming748@gmail.com"`<br>`ssh-keygen -t rsa -C 'zhangyiming748@gmail.com'`<br>`ssh -v git@github.com`|
|2020.4.12|||
|9:37-10:30|了解锁和原子操作的关系||
|10:59-11:50|了解死锁和活锁||
|12:00-13:30|了解redis五种数据类型的底层实现||
|13:30-13:50|整理笔记||
|17:17-21:08|leetcode29.两数相除|思路:商不可能大于被除数/商一定小于除数|
|21:08-21:40|解决报错`could not launch process: decoding dwarf section info at offset 0x0: too short`|`git clone https://github.com/derekparker/delve.git $GOPATH/src/github.com/derekparker/delve` 或 `git clone https://github.com/derekparker/delve.git %GOPATH%/src/github.com/derekparker/delve`|
|21:40-21:50|解决报错` RPC failed; curl 56 OpenSSL SSL_read: SSL_ERROR_SYSCALL, errno 10054`|尝试`git config --global http.sslVerify "false"`和`git config --global  http.postBuffer 524288000`|
|21:50-23:10|解决依赖问题|`git clone https://github.com/derekparker/delve.git %GOPATH%/src/github.com/derekparker/delve`<br>`git clone https://github.com/cosiner/argv.git %GOPATH%\src\github.com\cosiner\`<br>`git clone https://github.com/cpuguy83/go-md2man.git  %GOPATH%\src\github.com\cpuguy83\go-md2man`<br>`git clone https://github.com/davecgh/go-spew.git %GOPATH%\src\github.com\davecgh\go-spew`<br>`git clone https://github.com/fsnotify/fsnotify.git %GOPATH%\src\github.com\fsnotify\fsnotify`<br>`git clone https://github.com/google/go-dap.git %GOPATH%\src\golang\go-dap`<br>`git clone https://github.com/golang/protobuf.git %GOPATH%\src\golang\protobuf`<br>`git clone https://github.com/hashicorp/golang-lru %GOPATH%\src\hashicorp\golang-lru`<br>`git clone https://github.com/hpcloud/tail %GOPATH%\src\hpcloud\tail`<br>`git clone https://github.com/inconshreveable/mousetrap%GOPATH%\src\inconshreveable\mousetrap`<br>`git clone https://github.com/golang/sync.git %GOPATH%\src\golang.org\x\sync`<br>`git clone https://github.com/golang/xerrors.git %GOPATH%\src\golang\x\xerrors`<br>`git clone https://github.com/golang/arch.git %GOPATH%\src\golang\x\arch`<br>`go get -u gopkg.in/airbrake/gobrake.v2`<br>`go get -u gopkg.in/check.v1`<br>`go get -u gopkg.in/fsnotify.v1`<br>`go get -u gopkg.in/gemnasium/logrus-airbrake-hook.v2`<br>`go get -u gopkg.in/tomb.v1`<br>`go get -u gopkg.in/yaml.v2`<br>`go get -u rsc.io/pdf`<br>`go get -u go.starlark.net`|
|明日计划|解决其他依赖/完成29题/整理其他redis数据结构||
|2020.4.13|||
|15:00-16:49|leetcode29题负数问题||
|16:49|提交提示超出时间限制|重写|
|18:37|测试用例中包含奇怪的值|代码有问题|
|20:31|安装之前未安装的依赖||
|2020.4.14|||
|10:00|继续做题||
|17:00|看答案之后重新做||
|20:00|了解golang的channel用法||
<<<<<<< HEAD
|2020.4.11|||
|9:00-11:30|看答案/按照思路独立做/改成自己理解的方式||
|14:00-17:00|看推荐代码||
|17:00-19:00|看redis的string底层实现||
|明日计划|买的golang基础的书到了 看书||
|9:30-12:34|解决goland激活问题||
=======
|2020/04/16|||
<<<<<<< HEAD
|9:00-11:00|leetcode7.整数反转|按照自己的思路做没成功需要进一步了解数据类型的相互转换|
|11:00-12:00|研究goProxy|gomod需要GoProxy自动解决go get依赖否则需要git clone|
|14:00-19-00|看《Go语言趣学指南》书|第一章|
|20:30-22:00|看推荐代码|按照流程过一遍|
|明日计划|继续做题|看书第二章|画推荐系统代码流程图||
|9:00-11:00|leetcode7.整数反转|按照自己的思路做没成功|
|11:00-12:00|研究goProxy||
|14:00-19-00|看书||
|20:30-22:00|看推荐代码||
|明日计划|继续做题看书画代码流程图||
|2020/04/17|||
|9:30-11:30|解决Goland激活问题||
|14:00-20:33|看书第二章/研究goproxy并开启/研究远程调试||
|20:46|看书第二章|需要注意的点写笔记|
|2020/04/18|||
|9:30-12:30|看书到第六章节,做课后题|知识点标记|
|14:40-18:40|画推荐代码层次图|没画完|
|20:00-23:30|继续画推荐代码图||
|明日计划|继续画图|看书《Go语言趣学指南》做leetcode数据库题|
