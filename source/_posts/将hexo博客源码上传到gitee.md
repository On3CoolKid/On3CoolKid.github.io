---
title: 将hexo博客源码上传到gitee
date: 2022-11-16 00:25:48
tags: 博客搭建
categories:
---
>我通过这个方法成功将代码推到source分支里了，方面有点笨，但不会出错。

## 1.进入gitee仓库

首先在gitee仓库中master分支下创建source分支，再把source设置为默认分支

## 2.拉取source分支下的代码

输入以下命令拉取source分支下的代码（为了使本地仓库分支变为source），并剪切.git文件夹到hexo博客根目录中---此时的本地分支为source

```bash
git clone https://github.com/1CSH1/1CSH1.github.io.git
```

（git clone 默认是克隆Head指向的branch，默认是master分支，如果是多分支，我们可以单个克隆分支项目。git clone -b template <https://github.com/iview/iview-admin.git>  //clone template分支）

## 3.输入命令来上传hexo博客的源代码

此时已经有一个仓库在hexo博客的根目录了，因此依次输入以下命令来上传hexo博客的源代码

```bash
git remote add origin https://gitee.com/xxx/xxx
git add .
git commit -m "source"
git push origin source
```

## 4.示例图

如图所示，博客源代码已经上传到仓库的source分支

![01](img/Hexo/01.jpg)
