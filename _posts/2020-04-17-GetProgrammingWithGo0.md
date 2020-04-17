---
layout:     post                    # 使用的布局(不需要改)
title:     GetProgrammingWithGo             # 标题
subtitle:   我是一只被禁足的安小鸟 #副标题
date:       2020-04-17 00:00:01 GMT+0800             # 时间
author:     Zen                 # 作者
header-img: img/photo/birdAngle.webp    #这篇文章标题背景图片
catalog: Ture                   # 是否归档
tags:                               #标签
    - 读书
---
# 第0单元
```
1-1
package main

import (
	"fmt"
)

func main() {
	fmt.Println("Hello, playground")
}
```
# 第1单元
### 第2章
##### 2-1
```
// My weight loss program.
package main

import "fmt"

// main is the function where it all begins.
func main() {
	fmt.Print("My weight on the surface of Mars is ")
	fmt.Print(149.0 * 0.3783)
	fmt.Print(" lbs, and I would be ")
	fmt.Print(41 * 365 / 687)
	fmt.Print(" years old.")
}
```
##### 2-2
```
package main

import "fmt"

func main() {
	fmt.Printf("My weight on the surface of Mars is %v lbs,", 149.0*0.3783)
	fmt.Printf(" and I would be %v years old.\n", 41*365/687)
	fmt.Printf("My weight on the surface of %v is %v lbs.\n", "Earth", 149.0)
	fmt.Printf("%-15v $%4v\n", "SpaceX", 94)
	fmt.Printf("%-15v $%4v\n", "Virgin Galactic", 100)
}
//%4v左边填充四个空格
//%-4v右边填充四个空格
```
##### 2-3
```
// How long does it take to get to Mars?
package main

import "fmt"

func main() {
	const lightSpeed = 299792 // km/s
	var distance = 56000000   // km

	fmt.Println(distance/lightSpeed, "seconds")

	distance = 401000000
	fmt.Println(distance/lightSpeed, "seconds")
}
//const定义的值不能被重新赋值
//var hour,minute = 24,60 可以连续赋值
```
##### 2-4
```
package main

func main() {
	var weight = 149.0
	weight = weight * 0.3783
	weight *= 0.3783

}
```
##### 2-5
```
package main

func main() {
    var age = 41
    age = age + 1
    age += 1
    age++
}
//不支持前置运算++i
```
##### 2-6
```
package main

import (
	"fmt"
	"math/rand"
)

func main() {
	var num = rand.Intn(10) + 1
	fmt.Println(num)

	num = rand.Intn(10) + 1
	fmt.Println(num)
}
//Intn(10)指的是0-9
```
##### 实验
```
package main

import (
	"fmt"
	_ "log"
)

const (
	DISTANCE   = 56000000
	HOURPERDAY = 24
	DAY        = 28
)

func myAnswer() {
	fmt.Println(DISTANCE / (DAY * HOURPERDAY))
}
func main() {
	myAnswer()
	answer()
}
func answer() {
	fmt.Printf("%v", 56000000/(24*28))
}
```
### 第3章
##### 3-1
```
package main

import (
	"fmt"
	"strings"
)

func main() {
	fmt.Println("You find yourself in a dimly lit cavern.")

	var command = "walk outside"
	var exit = strings.Contains(command, "outside")

	fmt.Println("You leave the cave:", exit)
}
// Contains 判断字符串 s 中是否包含子串 substr
// 如果 substr 为空，则返回 true
```
##### 3-2
```
package main

import "fmt"

func main() {
	fmt.Println("There is a sign near the entrance that reads 'No Minors'.")

	var age = 41
	var minor = age < 18

	fmt.Printf("At age %v, am I a minor? %v\n", age, minor)
}
```
##### 3-3
```
package main

import "fmt"

func main() {
	var command = "go east"

	if command == "go east" {
		fmt.Println("You head further up the mountain.")
	} else if command == "go inside" {
		fmt.Println("You enter the cave where you live out the rest of your life.")
	} else {
		fmt.Println("Didn't quite get that.")
	}
}
```
##### 3-4
```
package main

import "fmt"

func main() {
	fmt.Println("The year is 2100, should you leap?")

	var year = 2100
	var leap = year%400 == 0 || (year%4 == 0 && year%100 != 0)

	if leap {
		fmt.Println("Look before you leap!")
	} else {
		fmt.Println("Keep your feet on the ground.")
	}
}

```
##### 3-5
`||`或
`&&`与
`!`非
```
package main

import "fmt"

func main() {
	var haveTorch = true
	var litTorch = false

	if !haveTorch || !litTorch {
		fmt.Println("Nothing to see here.")
	}
}
```
##### 3-6
```
package main

import "fmt"

func main() {
	fmt.Println("There is a cavern entrance here and a path to the east.")
	var command = "go inside"

	switch command {
	case "go east":
		fmt.Println("You head further up the mountain.")
	case "enter cave", "go inside":
		fmt.Println("You find yourself in a dimly lit cavern.")
	case "read sign":
		fmt.Println("The sign reads 'No Minors'.")
	default:
		fmt.Println("Didn't quite get that.")
	}
}
```
##### 3-7
```
package main

import "fmt"

func main() {
	var room = "lake"

	switch {
	case room == "cave":
		fmt.Println("You find yourself in a dimly lit cavern.")
	case room == "lake":
		fmt.Println("The ice seems solid enough.")
		fallthrough
	case room == "underwater":
		fmt.Println("The water is freezing cold.")
	}
}
```
##### 3-8
```
package main

import (
	"fmt"
	"time"
)

func main() {
	var count = 10

	for count > 0 {
		fmt.Println(count)
		time.Sleep(time.Second)
		count--
	}
	fmt.Println("Liftoff!")
}
```
# 第2单元
# 第3单元
# 第4单元
# 第5单元
# 第6单元
# 第7单元
### 第章
