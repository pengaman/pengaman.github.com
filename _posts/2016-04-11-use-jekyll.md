---
published: true
layout: post
title: Jekyll 博客
category: jekyll
tags: 
  - jekyll
time: 2016.04.11 13:02:00
excerpt: 一直想搭一个博客，今天终于开始做了。以后要养成写博客的习惯，把学习的东西记录下来。那我先记录下我是如何建立博客的。
---


一直想搭一个博客，今天终于开始做了。以后要养成写博客的习惯，把学习的东西记录下来。那我先记录下我是如何建立博客的。

<!--more-->

## 了解jekyll是什么
jekyll是一个简单的免费的Blog生成工具，类似WordPress。但是和WordPress又有很大的不同，原因是jekyll只是一个生成静态网页的工具，不需要数据库支持。但是可以配合第三方服务,例如Disqus。最关键的是jekyll可以免费部署在Github上，而且可以绑定自己的域名。

## 找一个模版
因为我在昨天之前完全不会使用jekyll，所以我决定选一个模版然后修改一下，以后再慢慢增删功能。当然，如果你想自己写也可以。对于我来说，下载下来的模版的目录结构都十分陌生，然后我找到了一个官方网站[jekyll](http://jekyll.bootcss.com/)，仔细研究了下各种文档的作用。

>* `config.yml`
这个文件是为了保存配置的。所谓的配置，其实可以用在命令行里面。放在这个文件里面主要是比较方便。
* `includes`
这里面的就是可以重复利用的文件。这个文件可以被其他的文件包含，重复利用。
* `layouts`
这里存放的是模板文件。
* `posts`
这里的文件就实际的文章内容了。文件名必须使用YEAR-MONTH-DATE-title.MARKUP的格式。如果使用textile的话，扩展名就是textile.


## 学会使用markdown

Markdown 的语法十分简单。常用的标记符号也不超过十个，这种相对于更为复杂的HTML标记语言来说，Markdown学习成本也不需要太多，且一旦熟悉这种语法规则，会有一劳永逸的效果。二十分钟足够你搞定它了。



## 图床推荐
在Markdown里加图片最好用图床，生成一个外链，在哪都能用。推荐一个[极简图床](http://yotuku.cn/) 是基于七牛的图床网站，注册一个七牛账户就能用了。

## kramdown
kramdown是一个Markdown解析器,它能够正确解释公式内部的符号,不会与Markdown语法冲突。为啥要用kramdowm呢？因为github不再采用Maruku解释器,而是采用kramdown解释器。
