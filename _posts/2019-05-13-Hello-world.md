---
layout:     post                    # 使用的布局（不需要改）
title:      怎么写markdown              # 标题
subtitle:   副标题好难想 #副标题
date:       2019-05-13              # 时间
author:     Zen                      # 作者
header-img: img/post-bg-2015.jpg    #这篇文章标题背景图片
catalog: true                       # 是否归档
tags:                               #标签
    - 测试
---


# 这是一级标题
## 这是二级标题
### 这是三级标题
#### 这是四级标题
##### 这是五级标题
###### 这是六级标题
**这是加粗的文字**

*这是倾斜的文字*`

***这是斜体加粗的文字***

~~这是加删除线的文字~~
>这是引用的内容
>>这是引用的内容
>>>这是引用的内容

---
----
***
*****

![blockchain](https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/
u=702257389,1274025419&fm=27&gp=0.jpg "区块链")

[简书](http://jianshu.com)
[百度](http://baidu.com)

- 列表内容
+ 列表内容
* 列表内容

1.列表内容
2.列表内容
3.列表内容

表头|表头|表头
---|:--:|---:
内容|内容|内容
内容|内容|内容

 `print("hell world")`

 ```
 def binary_search(hkey, nums):
   low = 0
   high = len(nums) - 1
   while low <= high:
       mid = low + (high - low) // 2
       if nums[mid] < hkey:
           low = mid + 1
       elif nums[mid] > hkey:
           high = mid - 1
       else:
           return mid
```
