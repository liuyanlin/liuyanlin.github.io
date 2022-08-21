---
layout: post
title: "Blog By HuxBlog QuickStart"
subtitle: "Hello Github Page"
date: 2020-08-13
author: "liu"
published: true
header-style: text
# header-img: "img/post-bg-2015.jpg"
# header-mask: 0.1
# catalog: false
mathjax: true
tags: [其他]
---

> “Yeah It's on. ”

下载ruby+devkit并全部安装：[https://rubyinstaller.org/downloads/](https://rubyinstaller.org/downloads/)

clone 模板
```
$ git clone git@github.com:Huxpro/huxblog-boilerplate.git
```

初始化Bundle，并安装相关插件
模板中没有Gemfile，需要先拷贝他的[Gemfile](https://github.com/Huxpro/huxpro.github.io/blob/master/Gemfile)
```
cd 模板根目录
bundle init
bundle install
```
本地启动服务  
```
bundle exec jekyll serve 或者 jekyll server
```
访问地址：[127.0.0.1:4000](//127.0.0.1:4000) 或 [localhost:4000](//localhost:4000)

快速创建Page  
模板git中没有Rakefile，需要拷贝他的[Rakefile](https://github.com/Huxpro/huxpro.github.io/blob/master/Rakefile#L11)  
```
rake post title="Hello 2015" subtitle="Hello World, Hello Blog"
```

参考：  
[https://docs.github.com/cn/pages/quickstart](https://docs.github.com/cn/pages/quickstart)
[https://github.com/Huxpro/huxpro.github.io/blob/master/_doc/Manual.md](https://github.com/Huxpro/huxpro.github.io/blob/master/_doc/Manual.md)

### 其他修改
#### 导航排序
导航是按读取顺序排序，所以：  
将about.html 修改为 0about.html  
将archive.html 修改为 1archive.html  
其他html有相对路径，需要一并修改  