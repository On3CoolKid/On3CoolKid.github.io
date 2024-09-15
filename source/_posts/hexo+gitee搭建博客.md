---
title: hexo+gitee搭建博客
date: 2022-11-14 19:56:14
tags: 
    - 博客搭建
    - Hexo
categories:
    - 博客搭建
---

> 友情链接1：https://www.bilibili.com/video/BV1mU4y1j72n?p=1&vd_source=a2a3ef0aedaa7e53345eb75da59a7c54
>
> ------
>
> 友情链接2：https://www.bilibili.com/video/av762277266/?vd_source=a2a3ef0aedaa7e53345eb75da59a7c54
 
## 1.准备工作

### 1.1安装node.js

> Node.js下载：【它让Javascript成为与PHP、Python、Perl、Ruby等服务端语言平起平坐的脚本语言。】）

https://nodejs.org/en/

> 安装完成后，命令行使用node-v和npm-v检查是否安装成功

### 1.2安装git并配置

https://git-scm.com/

### 1.3注册gitee账户，并新建一个仓库

https://gitee.com/

> 新建仓库时，仓库名称与gitee账户的名称一致

> 如图所示：

![02](img/Hexo/02.jpg)

> ——npm下载慢的话也可以下载淘宝下载源cnpm

```bash
npm install -g cnpm --registry=https://registry.npm.taobao.org
```

### 2.开始安装hexo

#### 2.1安装hexo

```
npm install -g hexo-cli
```

> 安装完成可输入hexo -v查看版本

#### 2.2新建一个文件夹，并初始化hexo

> 在博客文件夹根目录下，右键Git Bash Here

> 首先

```bash
hexo init myblog
```

> 然后

```bash
npm install
```

> 新建完成后，指定文件夹目录下有：
>
> - node_modules: 依赖包
> - public：存放生成的页面
> - scaffolds：生成文章的一些模板
> - source：用来存放你的文章
> - themes：主题
> - _config.yml: 博客的配置文件

- 

#### 2.3启动服务站点

```bash
hexo g 
hexo server
```

> 访问http://localhost:4000/ 至此hero就搭建好了。可以在本地访问了
