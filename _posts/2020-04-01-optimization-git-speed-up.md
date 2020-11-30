---
layout: post
title: "【小技巧】加速 Git clone 速度"
date: 2020-04-01
description: "在国内使用 Git 克隆 GitHub 等网站的仓储的时候，总是速度太慢，该怎么办呢？"
image: https://cdn.jsdelivr.net/gh/zhanghecool/zhangrongyu/assets/images/optimization-git-speed-up.jpg
author: zhanghe
tags:
  - 优化
---

## 给 Git clone 加速

在国内使用 Git 克隆 GitHub 等网站的仓储的时候，总是速度太慢，该怎么办呢？

- 如果你刚好有 `ss`，请使用以下步骤给 `Git` 配置代理：
  修改 `Git` 全局配置文件 `.gitconfig`，Mac 和 Linux 在 `~` 下，在最下方增加如下代码：
  ```bash
  [http]
  [http "https://github.com"]
  [http "https://pigweed.googlesource.com"]
    proxy = socks5://127.0.0.1:1086
  ```

## 给 GitHub 静态资源找到家

把一下内容添加到 Hosts 里面。

```bash
199.232.68.133 raw.githubusercontent.com
199.232.68.133 user-images.githubusercontent.com
199.232.68.133 avatars2.githubusercontent.com
199.232.68.133 avatars1.githubusercontent.com
```
