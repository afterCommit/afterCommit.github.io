---
layout:     post                    # 使用的布局(不需要改）
title:      插入搜索引擎设置              # 标题
subtitle:   少男与少女并排坐在那里,少男盯着少女 "我来大姨妈了"少女道,少年微微一叹气,但依然盯着少女,没有放弃的意思 "我痔疮犯了",少女道,少年微微一叹气,但依然盯着少女没有放弃的意思. "我口腔溃疡了"少女继续道,眼里满是委屈. 少年似乎终于放弃了,他满脸遗憾的道,那好吧, 那好吧,来个鸳鸯锅.   #副标题
date:       2019-09-14 00:01:00 GMT+0800               # 时间
author:     Zen                      # 作者
header-img: img/photo/jiuzhaigou.webp   #这篇文章标题背景图片
catalog: ture                       # 是否归档
tags:                               #标签
    - 测试
---
<!--baidu-->
<div>
<form action="http://www.baidu.com/s">
<input type="text" name="wd" id="kw"/>
<input type="submit" value="Baidu" />
</form>


<!--google-->

<form action="http://www.google.com/search" method="get">
<input type="text" name="q" size="20" maxlength="255" value="" />
<input type="submit" name="btnG" value="Google" />
</form>
</div>


		<input type="button" value="Run" id="embedRun">
		<div id="banner">
			<div id="head" itemprop="name">The Go Playground</div>
			<div id="controls">
				<input type="button" value="Run" id="run">
				<input type="button" value="Format" id="fmt">
				<div id="importsBox">
					<label title="Rewrite imports on Format">
						<input type="checkbox" id="imports">
						Imports
					</label>
				</div>

				<input type="button" value="Share" id="share">
				<input type="text" id="shareURL" style="display: none;">
				<label id="embedLabel" style="display: none;">
					<input type="checkbox" id="embed">
					embed
				</label>

			</div>
			<div id="aboutControls">
				<input type="button" value="About" id="aboutButton">
			</div>
		</div>
		<div id="wrap">
			<div class="linedtextarea" style="height:100%; overflow:hidden"><div class="lines" style="width: 3%; margin-top: 0px;"><div>1</div><div>2</div><div>3</div><div>4</div><div>5</div><div>6</div><div>7</div><div>8</div><div>9</div><div>10</div><div>11</div><div>12</div><div>13</div><div>14</div><div>15</div><div>16</div><div>17</div><div>18</div><div>19</div><div>20</div><div>21</div><div>22</div><div>23</div><div>24</div><div>25</div><div>26</div><div>27</div><div>28</div><div>29</div><div>30</div><div>31</div></div><textarea itemprop="description" id="code" name="code" autocorrect="off" autocomplete="off" autocapitalize="off" spellcheck="false" wrap="off" style="width: 97%;">// You can edit this code!
// Click here and start typing.
package main

import "fmt"

func main() {
  fmt.Println("Hello, 世界")
}</textarea></div>
		</div>
		<div id="output"><pre></pre></div>
		<img itemprop="image" src="/static/gopher.png" style="display:none">
		<div id="about">
<p><b>About the Playground</b></p>

<p>
The Go Playground is a web service that runs on
<a href="https://golang.org/">golang.org</a>'s servers.
The service receives a Go program, <a href="https://golang.org/cmd/vet/">vets</a>, compiles, links, and
runs the program inside a sandbox, then returns the output.
</p>

<p>
If the program contains <a href="https://golang.org/pkg/testing">tests or examples</a>
and no main function, the service runs the tests.
Benchmarks will likely not be supported since the program runs in a sandboxed
environment with limited resources.
</p>

<p>
There are limitations to the programs that can be run in the playground:
</p>

<ul>

<li>
The playground can use most of the standard library, with some exceptions.
The only communication a playground program has to the outside world
is by writing to standard output and standard error.
</li>

<li>
In the playground the time begins at 2009-11-10 23:00:00 UTC
(determining the significance of this date is an exercise for the reader).
This makes it easier to cache programs by giving them deterministic output.
</li>

<li>
There are also limits on execution time and on CPU and memory usage.
</li>

</ul>

<p>
The article "<a href="https://blog.golang.org/playground" target="_blank" rel="noopener">Inside
the Go Playground</a>" describes how the playground is implemented.
The source code is available at <a href="https://go.googlesource.com/playground" target="_blank" rel="noopener">
https://go.googlesource.com/playground</a>.
</p>

<p>
The playground uses the latest stable release of Go.<br>
The current version is <a href="/p/Ztyu2FJaajl">go1.13</a>.
</p>

<p>
The playground service is used by more than just the official Go project
(<a href="https://gobyexample.com/">Go by Example</a> is one other instance)
and we are happy for you to use it on your own site.
All we ask is that you
<a href="mailto:golang-dev@googlegroups.com">contact us first (note this is a public mailing list)</a>,
use a unique user agent in your requests (so we can identify you),
and that your service is of benefit to the Go community.
</p>

<p>
Any requests for content removal should be directed to
<a href="mailto:security@golang.org">security@golang.org</a>.
Please include the URL and the reason for the request.
</p>
		</div>
