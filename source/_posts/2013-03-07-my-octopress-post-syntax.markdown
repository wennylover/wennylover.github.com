---
layout: post
title: "我的octopress博客写法总结"
date: 2013-03-07 10:51
comments: true
categories: [moyan manual]
---

我的octopress博客写法遵循如下:

* 写小标题分段如下:

#### 小标题
----

* 对于在句子中用到的命令，写法如下:

这里是一个命令 `git status` ，用来查看当前git仓库的状态。

* 使用 `*` 进行无须列表，使用 `1.` 进行有序列表

* 写链接  

[一篇很好的讲到linux软连接和硬链接的文章](http://www.ibm.com/developerworks/cn/linux/l-cn-hardandsymb-links/)

* 写more, 这样的话就会在主页上显示到这个以上为止，其他的内容省略。  
	<！-- more -->

#### 写代码片段

方法1  
（每行前面是一个tab，或者四个空格，特别注意，如果代码code片段前面是一个序列的时候，比如ul，ol，那么这种方法无效）

	路径：/usr/local/rvm/rubies/ruby-1.9.3-p286/lib/ruby/1.9.1/webrick
	文件：server.rb
	方法：GenericServer#start_thread
	代码：
	addr = sock.peeraddr 改为 addr = sock.peeraddr(:numeric)

方法2

```ruby
	puts 'hello world'
```

