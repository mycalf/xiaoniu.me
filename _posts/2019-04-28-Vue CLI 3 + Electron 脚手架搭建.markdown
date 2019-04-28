layout: post
title:  Vue CLI 3 + Electron 脚手架搭建
date: 2019-04-28 16:37:55
tags: Vue Electron

# Vue CLI 3 + Electron 脚手架搭建

替换npm源至国内源：

```
npm config set registry https://registry.npm.taobao.org/
```



设置ELECTRON_MIRROR源，加速electron-chromedriver下载速度：

```
npm config set ELECTRON_MIRROR http://npm.taobao.org/mirrors/electron/
```



安装 vue cli 3：

```
npm install -g @vue/cli
```



创建VUE项目：

```
vue create my-project
```



进入新建的VUE项目后，添加Electron插件：

```
vue add electron-builder
```



运行项目：

```
npm run electron:serve
```

