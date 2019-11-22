---
layout:     post                    # 使用的布局(不需要改）
title:      更换魔法书上扶不起来的网卡       # 标题
subtitle:   贾母急的搂了宝玉道:"孽障!你生气,要打骂人容易,何苦摔那命根子!"宝玉满面泪痕泣道:"家里姐姐妹妹都没有,单我有,我说没趣;如今来了这么一个神仙似的妹妹也没有,可知这不是个好东西"贾母忙哄他道:"你这妹妹原来是有的"  #副标题
date:       2019-11-18 00:59:59 GMT+0800             # 时间
author:     Zen                 # 作者
header-img: img/photo/jiuzhaigou.webp    #这篇文章标题背景图片
catalog: False                       # 是否归档
tags:                               #标签
    - 杂谈
---
魔法书Pro科技尝鲜版自带的是瑞昱8822CE蓝牙Wi-Fi二合一芯片,信号干扰严重,只要蓝牙处在广播状态网络丢包率徘徊80%, 蓝牙数据传输时丢包率直逼100%

所以~~我有一个大胆的想法~~

如果这是瑞昱某个型号的问题,手动更换一款瑞昱更高等级的无线模块

如果这是瑞昱无线技术不过关的问题,手动更换一款Intel的高大全无线模块

我假装自己是一个消费者,询问了客服Intel版魔法书的网卡型号

华为商城客服的回答简单明了三个字`不知道`

至于为什么不去找华为官方客户服务中心,他们的各种[弱智操作](https://zhangyiming748.github.io/2019/11/04/Honor/)已经抵消了我对专业人员的信任

----
以下是详细操作的计划

按照维修思想,先从预期收益最大的方式入手

购买[IntelAX200NGW网卡](https://detail.tmall.com/item.htm?spm=a230r.1.14.19.743868c9qB44vR&id=602306932858&ns=1&abbucket=15&skuId=4221965037035)

购买[防静电设备](https://detail.tmall.com/item.htm?id=537354759539&spm=a1z09.2.0.0.6a4a2e8d83hKPI&_u=i2cc9fmub8f4)

购买[螺丝刀套装](https://item.jd.com/100005054710.html)

等待MagicBook Pro 过保

----

插播

昨天我以消费者的身份致电华为客服,询问了一下intel版魔法书的网卡型号

答复居然是`由于涉及供应商的涉密信息,我们不能提供详细的硬件信息`

我自己开盖看就不涉密,你告诉我电脑里边装的啥就是泄密?

----

没耐心,不等了

东西已经在路上了

到货之后找个黄道吉日就直接换了

----

插播

刚才接到了华为客服中心的电话

官方确认是Intel-AC9560

突然心里一沉

我买的是AX200

看下对比

||Intel® Wi-Fi 6 AX200 Module|Intel® Wireless-AC 9560|
|:---:|:---:|:---:|
|状态|Launched|Launched|
|发行日期 |Q2'19|Q4'17|
|重量（克）|2.8|2.8|
|操作温度范围|0°C to 80°C|0°C to 80°C|
|支持的操作系统|Windows 10, 64-bit*, Linux*, Chrome OS*|Windows 10, 64-bit*, Linux*, Chrome OS*|
|天线|2x2|2x2|
|TX/RX 流|2x2|2x2|
|频带|2.4Ghz, 5Ghz (160Mhz)|2.4Ghz, 5Ghz (160Mhz)|
|最高速度|2.4Gbps|1.73Gbps|
|Wi-Fi CERTIFIED*|WiFi 6 (802.11ax)|802.11ac|
|兼容性|FIPS, FISMA|FIPS, FISMA|
|集成蓝牙|是|是|
|主板板型|M.2 2230, M.2 1216|M.2 2230, M.2 1216|
|封装大小|22mm x 30mm x 2.4mm, 12mm x 16mm x 1.65mm|22mm x 30mm x 2.4mm, 12mm x 16mm x 1.57mm|
|系统接口类型|<font color="#FF0000">Wi-Fi(PCIe), BT(USB)</font>|<font color="#FF0000">M.2: CNVio</font>|

其中系统接口类型的差异让我看的夜不能寐

常识告诉我,PCIE通道的硬盘通常很贵,接口也很稀有,我买的电脑预装了廉价的小螃蟹芯片会是PCIE通道的吗?一切只有到货之后才知道,现在只能听天由命了

![包裹](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/Honor/package.jpg)<center>拜双十一所赐,龟速快递</center>

----

插播

更正,论坛上有人说之前的网卡是8822CE,但是在官网查询并没有这个型号,最接近的一款是[8821CE](https://www.realtek.com/zh-tw/products/communications-network-ics/item/rtl8821ce)

另外还有

+ 8822BE
>802.11AC/ABGN PCIE WLAN WITH BLUETOOTH 4.2 SINGLE-CHIP CONTROLLER The Realtek RTL8822BE-CG is a highly integrated single-chip that supports 2-stream 802.11ac solutions with Multi-user MIMO (Multiple-Input, Multiple-Output) and Wireless LAN (WLAN) PCI Express network interface controller and integrated Bluetooth 2.1/3.0/4.2 USB interface controller. It combines a WLAN MAC, a 2T2R capable WLAN baseband, and RF in a single chip. The RTL8822BE-CG provides a complete solution for a high-performance integrated wireless and Bluetooth device.FeaturesGeneralTFBGA 6.5x6.5mm package802.11 ac/abgn802.11ac 2x2, Wave-2 compatible with MU-MIMOBluetooth 4.2 (Software only)Host interfacePCI Express 1.1 for WLAN controllerUSB2.0 for Bluetooth controllerApplicationsThe product is applicable for PC/NB, Set-top box applications
>>(机翻)带蓝牙4.2单片机的802.11AC/ABGN PCIE WLAN Realtek RTL8822BE-CG是一个高度集成的单片机，支持2流802.11ac解决方案，支持多用户MIMO(多输入、多输出)和无线局域网(WLAN) PCI Express网络接口控制器，以及集成的蓝牙2.1/3.0/4.2 USB接口控制器。它将一个WLAN MAC、一个支持2T2R的WLAN基带和射频集成在一个芯片中。RTL8822BE-CG为高性能集成无线和蓝牙设备提供了完整的解决方案。WLAN controllerUSB2.0蓝牙控制器应用本产品适用于PC/NB、机顶盒应用

+ RTL8822BEH-VR
>802.11AC/ABGN PCIE WLAN WITH BLUETOOTH 4.1 SINGLE-CHIP CONTROLLER The Realtek RTL8822BEH-VR-CG is a highly integrated single-chip that supports 2-stream 802.11ac solutions with Multi-user MIMO (Multiple-Input, Multiple-Output) and Wireless LAN (WLAN) PCI Express network interface controller with integrated Bluetooth 2.1/3.0/4.1 USB interface controller. It combines a WLAN MAC, a 2T2R capable WLAN baseband, and RF in a single chip. The RTL8822BEH-VR-CG provides a complete solution for a high-performance integrated wireless and Bluetooth device. TFBGA 6.5x6.5mm package 802.11 ac/abgn 802.11ac 2x2, Wave-2 compatible with MU-MIMO Bluetooth 4.1 Host interface PCI Express 1.1 for WLAN controller HS-UART for Bluetooth controller Applications The product is applicable for Set-top box and AP router application
>>(机翻)802.11AC/ABGN PCIE WLAN带蓝牙4.1单片机控制器 Realtek rtl8822behr - vr - cg是一个高度集成的单片机，支持2流802.11ac解决方案，支持多用户MIMO(多输入、多输出)和无线局域网(WLAN) PCI Express网络接口控制器，支持集成蓝牙2.1/3.0/4.1 USB接口控制器。它将一个WLAN MAC、一个支持2T2R的WLAN基带和射频集成在一个芯片中。rtl8822behr - vr - cg为高性能集成无线和蓝牙设备提供了完整的解决方案。TFBGA 6.5x6.5mm封装802.11ac /abgn 802.11ac 2x2, Wave-2兼容MU-MIMO蓝牙4.1主机接口

+ RTL8822BS
>802.11AC/ABGN SDIO WLAN WITH BLUETOOTH 4.1 SINGLE-CHIP CONTROLLER The Realtek RTL8822BS-CG is a highly integrated single-chip that supports 2-stream 802.11ac solutions with Multi-user MIMO (Multiple-Input, Multiple-Output) and Wireless LAN (WLAN) SDIO interface controller with integrated Bluetooth 2.1/3.0/4.1 HS-UART interface controller. It combines a WLAN MAC, a 2T2R capable WLAN baseband, and RF in a single chip. The RTL8822BS-CG provides a complete solution for a high-performance integrated wireless and Bluetooth device. TFBGA 6.5x6.5mm package 802.11 ac/abgn 802.11ac 2x2, Wave-2 compatible with MU-MIMO Bluetooth 4.1 system Host interface SDIO 1.1/2.0/3.0 for WLAN controller HS-UART for Bluetooth controller Applications The product is applicable for Set-top box, virtual reality, and LTE router application
>>(机翻)Realtek RTL8822BS-CG是一个高度集成的单片机，支持2流802.11AC解决方案，支持多用户MIMO(多输入、多输出)和无线局域网(WLAN) SDIO接口控制器，支持集成蓝牙2.1/3.0/4.1 HS-UART接口控制器。它将一个WLAN MAC、一个支持2T2R的WLAN基带和射频集成在一个芯片中。RTL8822BS-CG为高性能集成无线和蓝牙设备提供了完整的解决方案。TFBGA 6.5x6.5mm封装802.11ac /abgn 802.11ac 2x2, Wave-2兼容MU-MIMO蓝牙4.1系统主机接口SDIO 1.1/2.0/3.0 for WLAN controller HS-UART for Bluetooth controller Applications本产品适用于机顶盒、虚拟现实、LTE路由器应用

+ RTL8822BU
>802.11AC/ABGN USB WLAN WITH BLUETOOTH 4.1 SINGLE-CHIP CONTROLLER The Realtek RTL8822BU-CG is a highly integrated single-chip that supports 2-stream 802.11ac solutions with Multi-user MIMO (Multiple-Input, Multiple-Output) and Wireless LAN (WLAN) with integrated Bluetooth 2.1/3.0/4.1 USB-multi interface controller. It combines a WLAN MAC, a 2T2R capable WLAN baseband, and RF in a single chip. The RTL8822BU-CG provides a complete solution for a high-performance integrated wireless and Bluetooth device. TFBGA 6.5x6.5mm package 802.11 ac/abgn 802.11ac 2x2, Wave-2 compatible with MU-MIMO Bluetooth 4.1 system Host interface USB2.0 for WLAN and BT controller Applications The product is applicable for TV and Set-top box application
>>(机翻)Realtek RTL8822BU-CG是一个高度集成的单片机，支持2流802.11AC解决方案，多用户MIMO(多输入、多输出)和无线局域网(WLAN)，集成了蓝牙2.1/3.0/4.1 USB-multi interface CONTROLLER。它将一个WLAN MAC、一个支持2T2R的WLAN基带和射频集成在一个芯片中。RTL8822BU-CG为高性能集成无线和蓝牙设备提供了完整的解决方案。TFBGA 6.5x6.5mm封装802.11ac /abgn 802.11ac 2x2, Wave-2兼容MU-MIMO蓝牙4.1系统主机接口USB2.0用于WLAN和BT控制器应用本产品适用于电视和机顶盒应用

<font size=18>看来具体型号有待确认,不如现在来有奖竞猜一下,评论区留下你的答案,猜对可获得群成员稀有ASMR,正确答案即将揭晓</font>

----

![到货](https://raw.githubusercontent.com/zhangyiming748/zhangyiming748.github.io/master/img/Honor/item.jpg)<center>如果换不成功,最坏的打算,USB无线网卡</center>

----

我理解华为想要扶持中国企业,但有的真的是扶不起来啊,扶瑞昱扶声卡、以太网卡、读卡器和分线器都是可以的,无线网卡还是算了吧

----
换下来的网卡不要扔,裹上鸡蛋液,粘上面包糠,下锅炸至金黄酥脆控油捞出,老人小孩都爱吃,隔壁小孩都馋哭了
