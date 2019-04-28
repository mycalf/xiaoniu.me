---
layout: post
title:  Vue CLI 3 + Electron 脚手架搭建
date: 2019-04-28 16:37:55
tags: Vue Electron
---


替换npm源至国内源：

{% highlight text %}
npm config set registry https://registry.npm.taobao.org/
{% endhighlight %}



设置ELECTRON_MIRROR源，加速electron-chromedriver下载速度：

{% highlight text %}
npm config set ELECTRON_MIRROR http://npm.taobao.org/mirrors/electron/
{% endhighlight %}



安装 vue cli 3：

{% highlight text %}
npm install -g @vue/cli
{% endhighlight %}



创建VUE项目：

{% highlight text %}
vue create my-project
{% endhighlight %}



进入新建的VUE项目后，添加Electron插件：

{% highlight text %}
vue add electron-builder
{% endhighlight %}



运行项目：

{% highlight text %}
npm run electron:serve
{% endhighlight %}

