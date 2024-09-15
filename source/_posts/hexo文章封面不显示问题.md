---
title: hexo文章封面不显示问题
date: 2022-11-18 01:00:25
tags: Hexo
categories:
---

## 1.未配置就新建文章

> 在没有设置butterfly中的_config.yml文件的文章封面，就hexo new 文章。

## 2.插入以下代码

> 在每篇文章中插入以下代码，图片就可以显示出来了

```html
<meta name="referrer" content="no-referrer" />
```



