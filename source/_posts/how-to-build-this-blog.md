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
经过调研和尝试，目前基本满足了自己的全部需求。本地完成文本编写push到gitlab，后者自动调用CICD，连接服务器，调用hexo进行渲染和重新部署，并同步推送至 github.io。

## 框架 Hexo
一款比较流行基于NodeJS的博客框架。
- 使用了 Next主题
最初直接pull了Next主题到文件路径，如果不打算在主题上进行太多编辑问题不大，否则不太适合版本维护，后面使用了submodule的方式进行管理
  ```
  //查看并去掉之前已经添加进git索引的next文件目录
  git ls-files --stage themes/next/
  git rm --cached themes/next/
  //通过git submodule方式重新添加
  git submodule add https://github.com/Fanlu91/hexo-theme-next.git themes/next/
  ```
  git submodule问题参考了 
  https://git-scm.com/book/zh/v1/Git-%E5%B7%A5%E5%85%B7-%E5%AD%90%E6%A8%A1%E5%9D%97
  https://codeday.me/bug/20170623/27343.html
## 环境和服务
  - 腾讯云 / github page
  - hexo server
  - nginx做反向代理实现https
## 部署
- 仓库 gitlab
- 持续集成 gitlab CI
## 其他
- 文章编写 vscode 安装md预览插件

# 待扩展能力
- 使用google analysis/baidu站长统计
- 添加disqus评论
- google adsense
  


