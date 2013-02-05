---
layout: post
title: "Ruby,Rails的一些概念和注意点"
date: 2013-02-05 14:39
comments: true
categories: [ruby, rails]
---

#### Ruby,Rails的一些概念和注意点
----
* rvm: ruby version manager, Ruby版本管理工具
* gem(rubygem): 一个ruby程序，用来管理gem包的安装等，类似linux下的apt-get  
	ruby1.9以前版本需要 `require 'rubygems'` ，ruby1.9开始已经自动包含gem。
* bundle: 用来管理一个rails web工程的所有gem包的依赖，版本等。
* rake: 一个gem包，也就是一个ruby程序，作用是用来执行其他用ruby开发的task的程序。
* rack: A Ruby Webserver interface.是一个提供了一个ruby web服务器和ruby web框架之间的最小接口的gem程序。主要是web框架开发者用的。
