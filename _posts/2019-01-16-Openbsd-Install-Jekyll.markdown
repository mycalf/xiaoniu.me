---
layout: post
title:  "Openbsd Install Jekyll"
date:   2019-1-16 12:14:59
categories: install
tags: jekyll openbsd
---

在未设置packages源的情况下，添加源：

{% highlight bash %}
export PKG_PATH=http://ftp.openbsd.org/pub/OpenBSD/`uname -r`/packages/`machine -a`/ 
{% endhighlight %}

安装Ruby：
{% highlight bash %}
pkg_add ruby
{% endhighlight %}

Ruby安装完成后，便可使用gem安装jekyll了：
{% highlight bash %}
gem25 install jekyll bundler
{% endhighlight %}

这里在Openbsd的packages中，gem编译成了gem25，jekyll、bundler同样会在不同版本中加入版本号。

{% highlight bash %}
jekyll serve
{% endhighlight %}
安装完成后，创建项目，使用jekyll serve开启jekyll的web服务。