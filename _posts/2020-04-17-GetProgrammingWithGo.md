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

### 第2章 实验
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
### 第3章 实验
```
func myAnswer() {
	num := rand.Intn(100) + 1
	var guess int


	for {
		log.Println("input a num")
		_,_=fmt.Scan(&guess)
		if guess>num {
			fmt.Println("more than answer")
			continue
		}else if guess<num {
			fmt.Println("less than answer")
			continue
		}else {
			fmt.Println("right answers")
			return
		}
	}

}
```
### 第4章 实验
```
package main

import (
	"fmt"
	"math/rand"
)

var era = "AD"

func myAnswer() {
	for i := 0; i < 10; i++ {
		year := rand.Intn(2020) + 1
		month := rand.Intn(12) + 1
		daysInMonth := 31
		leap := isLeapYear(year)
		switch leap {
		case true:
			if month == 2 {
				daysInMonth = 28
			}

		case false:
			daysInMonth = 30
		}

		day := rand.Intn(daysInMonth) + 1

		fmt.Println(era, year, month, day)
	}

}
func isLeapYear(year int) bool {
	if year%400 == 0 || (year%4 == 0 && year%100 != 0) {
		return true
	}
	return false
}
```
### 第5章 实验
```
package main

import (
	"fmt"
	"math/rand"
)

const (
	secondsPerDay = 86400
)

func ticket() {

	var (
		distance int
		company  string
		trip     string
	)
	fmt.Println("Spaceline\tDays\tTrip\tType\tPrice")
	fmt.Println("==================================")
	for count := 0; count < 10; count++ {
		switch rand.Intn(3) {
		case 0:
			company = "Intel"
		case 1:
			company = "AMD"
		case 2:
			company = "Nvidia"
		}
	}
	speed := rand.Intn(15) + 16
	duration := distance / speed / secondsPerDay
	price := 20.0 + speed
	if rand.Intn(2) == 1 {
		trip = "Round-trip"
		price = price * 2
	}else {
		trip="One-way"
	}
	fmt.Println(company,duration,trip,price)
}
func main(){
	ticket()
}
```
### 第6章 实验
```
package main

import (
	"fmt"
	"math/rand"
)

func piggy(x, y float64) float64 {
	//存入
	fmt.Println(x)
	//现有
	fmt.Println(y)
	//存后
	return x + y
}
func main() {
	money := make(map[int]float64, 0)
	money[0] = 0.05
	money[1] = 0.10
	money[2] = 0.25
	var kind int
	//var once float64
	var totol float64
	for {
		kind = rand.Intn(3)

		if totol >= 20.00 {
			break
		} else {
			totol = totol + piggy(money[kind], totol)
		}
	}
	fmt.Printf("final%v", totol)
}

```

### 第章 实验
### 第章 实验
### 第章 实验
### 第章 实验
### 第章 实验
### 第章 实验
### 第章 实验
### 第章 实验
### 第章 实验
### 第章 实验
### 第章 实验
### 第章 实验
