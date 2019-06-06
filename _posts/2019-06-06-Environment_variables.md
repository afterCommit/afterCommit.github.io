---
layout:     post                    # 使用的布局(不需要改）
title:      高逼格设置环境变量               # 标题
subtitle:    水一百度会开,人一百度会死  #副标题
date:       2019-06-06 11:45:00              # 时间
author:     Zen                      # 作者
header-img: img/pet/supremelysab-787607-unsplash.jpg   #这篇文章标题背景图片
catalog: true                       # 是否归档
tags:                               #标签
    - 常识
---

## 这个方法适用于以下的场景

你电脑对面的女神希望你帮他设置他电脑的环境变量，而你又不想在她面前表现出你是在一边查怎么设置一边设置的

----

|功能|PowerShell命令|示例|CMD命令|示例|
|:--:|:--:|:--:|:--:|:--:|
|要验证刚刚的用户环境变量有没有创建成功|||echo %刚刚创建的变量名%|`echo %JAVA_HOME%`|
|创建用户变量|[Environment]::SetEnvironmentVariable("要创建的用户环境变量的变量名", "要创建的用户环境变量的变量值" ,"User")|`[Environment]::SetEnvironmentVariable("JAVA_HOME","C:\Program Files\Java\jdk1.8.0_201","User")`|setx 要创建的用户环境变量的变量名 "要创建的用户环境变量的变量值"|`setx JAVA_HOME "C:\Program Files\Java\jdk1.8.0_201"`|
|创建系统变量|[Environment]::SetEnvironmentVariable("要创建的系统环境变量的变量名", "要创建的系统环境变量的变量值" ,"Machine")|`[Environment]::SetEnvironmentVariable("JAVA_HOME","C:\Program Files\Java\jdk1.8.0_201","Machine")`|setx /M 要创建的系统环境变量的变量名"要创建的系统环境变量的变量值"|`setx /M JAVA_HOME "C:\Program Files\Java\jdk1.8.0_201"`|
|追加变量|||setx 变量名 %变量名%;"新变量值"|`setx testx %testx%;"C:\Users\zhang\Desktop\PINBALL"`|

**实例** 你的女神让你设置JAVA环境变量

```
setx /M JAVA_HOME "C:\Program Files\Java\jdk1.8.0_201"
setx /M PATH %PATH%;"%JAVA_HOME%\bin"
setx /M CLASSSPATH ".;%JAVA_HOME%\lib;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar"
```
