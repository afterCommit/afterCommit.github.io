---
layout:     post                    # 使用的布局（不需要改）
title:      蓝屏日志              # 标题
subtitle:   家长A:“你家宝宝的微积分这次考了多少分?”家长B:“嗨，别提了。才99分，全班倒数第三。 ”家长A:“你要孩子之前没定制数学加强款呐?  ”家长B:“我们家孩子爸爸嫌贵呀，只买了6个基因包，全癌症免疫和长跑、双眼皮显性遗传都有了，结果数学加强这块，就没买最新款。家长A:“那你们准备什么时候要老二啊?”家长B:“明年吧，听说明年要出新款，先天免疫疾病比现款多21种，平均寿命高40年，还有限量版的金城武颜值加强款。”家长A:“还是晚点儿要孩子好，我家这个才3岁，配置已经明显过时了。  ”家长B:“可不是，这周末我就找售后去闹一下，最起码也得让他们给打个折怎么着也得给我们家老大数学基因这块给补齐喽” #副标题
date:       2019-08-01  08:00:00            # 时间
author:     Zen                      # 作者
header-img: img/post-bg-2015.jpg    #这篇文章标题背景图片
catalog: False                       # 是否归档
tags:                               #标签
    - 操作系统
---

1. 0xc000007b或0xc0000428
  如果出现像以下类似的

  `bootsafe.sys`

  `bootsafe64.sys`

  `bootsafe64_ev.sys`

  `bootsafe_ev.sys`

  都可以以下方法来解决。
  ```
  你的电脑/设备需要修复
  无法加载操作系统，原因是关键系统驱动程序丢失或包含错误。
  文件：\windoiws\system32\drivers\bootsafe64_ev.sys
  错误代码：0xc000007b
  你需要使用恢复工具。如果没有任何安装介质（如光盘或USB设置），请联系你的电脑管理员或电脑？设备制造商。
  ```
  看图说话大概就是这样

  ![1](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/bluescreen/1.png)

  如果是win7的话就是这样的画风

  ![2](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/bluescreen/2.png)

  **分析原因**

    此问题就出在金山、驱动精灵等一些产品给系统加入的这个文件，它不知出于什么原因不正常了，但是由于它存在于driver目录下，Windows启动时仍然要加载它，所以不能进入系统。它不是Windows的东西，所以微软没有应对方案。

    上面看不懂的话我翻译成中文给你们听: 大部分的流氓软件没有能力通过好好做产品留住客户,所以就选择一种更简单粗暴的方法——你不敢卸载,我装上我的守护程序,你敢卸载我就敢让你不能开机,所以,能远离这些尽量远离,翻翻我以前的博客

  **解决方法**

    1. 无脑

    重装一个纯净的原版系统,方法看我之前的博文,然后远离流氓软件

    2. 有脑

    在安全模式(win7)RE环境(win10)删掉

    `C:\WINDOWS\system32\drivers\ bootsafe64_ev.sys`

    `C:\WINDOWS\system32\drivers\kavbootc64.sys`

    等可疑文件即可

    如果以上文件无法删除,显示权限问题

    做一张ubuntu live USB 随身带着 以后还会用得上的

 ----

 待续
