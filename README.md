#Markdown demo

This is a demonstration of how to use Markdown to write README.  
This file would demonstrate two syntax.  

- the traditional (original) Markdown
- GitHub Flavored Markdown.

**本文档部分摘抄整理自以下几篇文章**  

1. [markdown syntax 原作者](http://daringfireball.net/projects/markdown/syntax) on daringfireball.net 
2. [上文的简体中文翻译](http://wowubuntu.com/markdown/basic.html) from wowubuntu.com
3. [献给写作者的 Markdown 新手指南 ](http://jianshu.io/p/q81RER#login-modal)from 简书
4. <http://www.ituring.com.cn/article/504>

## 目录

- 传统 Markdown
    - 标题
	- 段落
	- 加粗和斜体
	- 引用
	- 列表
	- 超链接
	- 图片
	- 代码
	- 分隔线
	- 自动链接
	- 转义字符
- GitHub 风格 Markdown
    - 换行(GFM)
    - 斜体(GFM)
    - 自动链接(GFM)
    - 删除线(GFM)
    - 代码段和代码高亮(GFM)
    - 任务列表(GFM)

## 标题
	
注意 \# 和字之间要有空格

	This is an H1
	=============
 
	This is an H2
	-------------
	
	# This is an H1
	## This is an H2
	### This is an H3
	#### This is an H4
	##### This is an H5
	###### This is an H6

## 段落

1. 正常的段落不要使用任何空格或者TAB缩进  
2. 连续回车分段
3. 行尾使用2个空格换行

## 加粗和斜体
可以使用\_或者\#

	*斜体*		_斜体_
	**加粗**		__加粗__
	
## 引用

使用\>添加区域引用

	> This is a blockquote.
	> 
	> This is the second paragraph in the blockquote.
	>
	> ## This is an H2 in a blockquote

## 列表

- 无序列表 使用（星号，加号，减号）+ **空格**
- 有序列表使用数字+点+**空格**  
- 列表中的项可以有多行，只要在开头放一个tab或者四个空格即可

## 超链接

- 行内形式
- 参考形式

title是可选的

	行内
	This is an [example link](http://example.com)
	This is an [example link](http://example.com/ "With a Title")
	
	参考
	I get 10 times more traffic from [Google][1] than from
	[Yahoo][2] or [MSN][3]
	
	[1]: http://google.com/        "Google"
	[2]: http://search.yahoo.com/  "Yahoo Search"
	[3]: http://search.msn.com/    "MSN Search"
	
## 图片

- 行内形式
- 参考形式

title是可选的

	行内
	![alt text](/path/to/img.jpg "Title")
	
	参考
	![alt text][id]

	[id]: /path/to/img.jpg "Title"

## 代码

- 反引号
- TAB or 4 space

使用反引号插入代码( \` )  
如果需要插入反引号就使用两个反引号，用空格分开  
起始端后面一个，结束端前面一个  
	`` `foo` ``


## 分隔线

你可以在一行中用三个或以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号中间插入空白。下面每种写法都可以建立分隔线：

	* * *
	
	***
	
	*****
	
	- - -
	
	------

## 自动链接
	
	<http://example.com/>

## 转义字符
	
	\   反斜杠
	`   反引号
	*   星号
	_   底线
	{}  大括号
	[]  方括号
	()  括号
	#   井字号
	+    加号
	-    减号
	.   英文句点
	!   惊叹号

## 换行(GFM)

GFM中，换行可以不用在行尾加两个空格
第一行（不加空格）
第二行	

## 斜体(GFM)

GFW中字符串中间的下划线会被忽略
比如 `perform_complicated_task do_this_and_do_that_and_another_thing`  
perform_complicated_task do_this_and_do_that_and_another_thing
	
## 自动链接(GFM)

GFW中直接添加URL就好，比如 https://github.com 

## 删除线(GFM)

	~~Mistaken text.~~
显示成
~~Mistaken text.~~

## 代码段和代码高亮(GFM)

	Here's an example:
	
	```
	function test() {
	  console.log("notice the blank line before this function?");
	}
	```
显示成

Here's an example:

```
function test() {
  console.log("notice the blank line before this function?");
}
```

针对某种代码，可以指明

	```ruby
	require 'redcarpet'
	markdown = Redcarpet.new("Hello World!")
	puts markdown.to_html
	```

显示成

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

## 任务列表(GFM)

	- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
	- [x] list syntax required (any unordered or ordered list supported)
	- [x] this is a complete item
	- [ ] this is an incomplete item

显示成

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

