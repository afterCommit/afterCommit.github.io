---
layout:     post                    # 使用的布局(不需要改）
title:      使用三天左右的魔法书简评             # 标题
subtitle:   你认为大禹三过家门而不入真的是什么都没干吗?不要忘了,他媳妇后来变成望夫石了,而孙悟空是从石头里蹦出来的,关键是,大禹的定海神针还听孙悟空的话;你认为孙悟空当年定住了七仙女,真的什么都没干吗？不然玉帝王母也不会随意发那么大的火,蟠桃园过后也没再见过七仙女了不是么?紧接着就出现了七个葫芦娃,正好七个,为什么他们能像孙悟空一样变成石头?后来,那七个小葫芦天天欺负衣衫不整的蛇精,把蛇精压在下面你以为只是单纯的压住了吗？那七龙珠怎么来的？要知道蛇是产蛋的.后来为什么孙悟空又到处寻找七龙珠?再后来愚公把葫芦娃变得山移开了,放出里面的蛇精,蛇精修炼千年之后为了报答当年的愚公移山救命之恩,找到了愚公转世的许仙,并且嫁给了他.这也就解释了为什么许仙能生下文曲星了,那是猴子儿媳生的啊. #副标题
date:       2019-10-18 00:00:00 GMT+0800             # 时间
author:     Zen                 # 作者
header-img: img/photo/jiuzhaigou.webp    #这篇文章标题背景图片
catalog: True                       # 是否归档
tags:                               #标签
    - 杂谈
---
魔法书的学名是 MagicBook Pro

买的是R7 8+512 deepin 版

使用了大概三天

简单说一下

说之前先来张图片

![订单](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/MagicBook/订单.jpg)

晒单只是为了证明我并非在云评测这台电脑,毕竟现在认为自己能看懂几个参数就怼天怼地怼空气的人太多了

----

## 开箱

直接上图

![](https://s2.ax1x.com/2019/10/18/KVqwcD.jpg "去掉外包装")

![](https://s2.ax1x.com/2019/10/18/KVqR9f.jpg "D面")

![](https://s2.ax1x.com/2019/10/18/KVq0je.jpg)

![](https://s2.ax1x.com/2019/10/18/KVqNh6.jpg)

![](https://s2.ax1x.com/2019/10/18/KVqa9K.jpg)

![](https://s2.ax1x.com/2019/10/18/KVqcNt.jpg)

![](https://s2.ax1x.com/2019/10/18/KVqg4P.jpg)


## 开机

科技尝鲜版实际预装的是deepin系统,这系统基于Ubuntu,个人喜欢deb系,接上适配器开盖直接开机,进入OOBE阶段,设置用户名密码区域时间后进入系统,`sudo password`设置`root`用户密码,这里要重点提示,Linux电脑默认的安装源是根服务器,而且一般都是在国外,安装软件和更新之前一定要切换成中国的服务器,我推荐阿里和华为的,用vi编辑器直接改就行

`sudo vi /etc/apt/sources.list`

打开的文件只要在首行添加

`deb [by-hash=force] http://mirrors.aliyun.com/deepin panda main contrib non-free`

就行,然后就可以更新软件列表和软件本体了,命令分别是

`sudo apt-get update`
`sudo apt-get upgrade`

到这里基本上可以正常使用了
需要什么就装什么

`sudo apt-get install <sorfwareName>`

出现依赖问题就

`sudo apt-get -f install`

自己下的deb软件包就

`sudo dpkg -i <softwareName>`

deepin的软件中心,emmm,我个人是不需要,有些软件缺少依赖不能安装,报错信息只告诉你依赖错误而不说明是哪一个依赖,还不能使用`-f install`修复,这就很尴尬了,对新手来说这个应用商店应该还不错吧

## 换系统

根据我之前的[教程](https://zhangyiming748.github.io/2019/10/12/MagicBook/)换到了Windows系统,开始暴露了一些问题

小螃蟹(Realtek瑞昱)家的蓝牙Wi-Fi二合一芯片抗干扰性真的是差到极致,只要开着蓝牙,Wi-Fi丢包率直逼百分百,网络几乎无法连接,幸亏主板设置里可以屏蔽掉蓝牙,外接USB蓝牙适配器能暂时解决问题.

触摸板上半部分不能按下,这种设计应该是很复古了,如果是因为钱的问题当我没说,因为我也没钱

安装了hilink,一碰传确实是方便,但因为蓝牙问题这个功能开启时电脑就别打算上网了
## 性能

由于农企的崛起,这个电脑运行

`ADOBE Audition`

`ADOBE PhotoShop`

`Adobe Dreamweaver`

`Microsoft Office 2019`

`jetbrains Goland`

`jetbrains CLion`

`jetbrains PyCharm`

均无压力

## 便携

>你见过北京高峰期的地铁十三号线吗?

买这个电脑其中一个原因就是实在是心疼带着五位数MacBook Pro去挤地铁

在魔法书上安装好git工具,hosts指向代码库,不在公司的时候随时随地看代码,修改,提交

简单来说就是`抗(二声)造` `不心疼`

## 竞品

同价格段位的某品牌3700U宣传的是 **满血版** APU

真是重新定义了“满血版”的意思

荣耀的H后缀都没宣传自己是满血版

某家文案U后缀好意思说自己满血版?

您算老几?

华为商城下单3750H到手价4699

这个满血版打算卖多少?

## 总结

+ 不要想着用四千的电脑能干四万元电脑干的事,它符合我的预期,我就会买,并且认为值

+ 会用电脑就会物尽其用,不会用电脑四万块钱也只是玩个连连看

+ 同样或差不多性能的电脑,我会优先选择国产

+ 毕竟华为还是刚开始做电脑,电脑的详细参数很难找到,至少官网上我看不见,询问客服也只是沉默后的答非所问,我甚至怀疑客服知不知道他们卖的是啥

+ 上一条不要杠,否则跟我说说```两个硬盘位分别是什么接口,支持什么协议```

+ 总体来说我对这个电脑非常满意
