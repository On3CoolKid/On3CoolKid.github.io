---
title: butterfly设置全局背景
date: 2022-12-12 17:43:14
tags: Hexo
categories:
---

> 全局背景：去掉顶部横幅，设置的背景会充满整个网页

> Butterfly主题底部蓝色区域修改为透明色：

①Butterfly主题文件夹下_config.yml文件中：

```
footer_bg: false
```

②Butterfly主题文件夹下source->layout->footer.styl中将一下代码注释：

```
// background: $light-blue
```

