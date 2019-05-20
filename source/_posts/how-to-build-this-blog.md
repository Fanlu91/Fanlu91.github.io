---
title: 博客搭建记录-从写作环境到持续集成部署
date: 2018-12-21 17:01:12
tags:
- hexo
- gitlab
- ci/cd
- blog
---

# 背景
近期工作不忙，陆续花了几天时间搭建这个博客，最初期望是：
- 利用已有的腾讯云vps和域名
- 可以在*任意环境*编写markdown文件
- 提交git后直接能够查看（网页）
- 支持统计/评论
- 支持https
- 尽量简介/美观

# 实践
经过调研和尝试，目前基本满足了自己的全部需求。本地完成文本编写push到gitlab，后者自动调用CICD，连接服务器，调用hexo进行渲染和重新部署，并同步推送至github.io。

- 框架 Hexo
- 环境和服务
  - 腾讯云 / github page
  - hexo server
  - nginx做反向代理实现https
- 仓库 gitlab
- 持续集成 gitlab CI
- 文章编写 vscode 

# 扩展能力
- 使用google analysis/baidu站长统计
- 添加disqus评论
- google adsense

