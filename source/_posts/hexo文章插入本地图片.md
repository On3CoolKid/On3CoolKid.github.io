---
title: hexo文章插入本地图片
date: 2022-11-26 21:50:04
tags: Hexo
categories:
type:
---

## 1.通过相对地址（推荐）

> 在themes（主题）文件夹下的的img文件夹下（themes->butterfly->source->img）创建一个postimg文件夹，（由于_config.yml文件夹中的图片都是通过相对地址引入的，所以可以通过这种方式引入图片，同时引入的这些图片也会存在public中，并上传到Gitee仓库中），或者也可以创建多个图片文件夹，对引入的这些图片进行分类。

> 图片引入格式如下：

```
![xxx](/img/postimg/xxx.jpg)
```

## 2.通过下载插件（不太推荐）

### 2.1进入博客根目录，安装插件

```bash
npm install https://github.com/CodeFalling/hexo-asset-image –save
```

### 2.2修改_config.yml文件

> 进入博客根目录将_config.yml文件下的post_asset_folder:改为true

> 此时，运行`hexo new "XXX"`，生成XXX.md博文时就会在`/source/_posts`目录下生成XXX（与文章同名）的文件夹，将你想在XXX博文中插入的照片放置到这个同名文件夹中即可，图片的命名随意。

### 2.3在typora中引入图片

> 图片（假设图片后缀为JPG格式）命名格式如下：

```
![xxx](xxx.jpg)
```

> 如果图片的名称为123.jpg，则：

```
![123](123.jpg)
```

### 2.4注意

> 如果md文档改名，对应的目录也要改名，否则会出现图片不显示的情况。

> 友情链接：https://blog.csdn.net/fitnig/article/details/106522811

## 3.其他方式（不推荐）

> 这种方式简单来说就是~
>
> 必须先hexo d上传图片到仓库里，然后通过http方式引入图片

> 直接上链接https://blog.csdn.net/weixin_44381143/article/details/104552433
