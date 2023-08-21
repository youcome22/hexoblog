---
# Post Front-matter 用於頁面配置
title: 文章标题
date: 
updated: 
tags: 
categories: 
keywords: 
description: 
top_img: /img/page.jpg
comments: true
cover: /img/favicon.png
toc:
toc_number:
toc_style_simple:
copyright:
copyright_author: youcome
copyright_author_href: www.baidu.com
copyright_url: 
copyright_info: 无
mathjax: false
katex: false
aplayer: 
highlight_shrink: true
aside: true
abcjs: false
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

## Quick Start

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)

# Hexo+butterfly主题

Hexo是一个快速, 简洁且高效的博客框架，让上百个页面在几秒内瞬间完成渲染。

部署环境（本地）：

- Git
- Node.js（Node.js 版本需不低于 8.10，建议使用 Node.js 10.0 及以上版本）
- Hexo
- butterfly主题
- GitHub

## Hexo一键部署

```js
$ npm install hexo-cli -g
$ hexo -v
$ hexo init blog
$ cd blog
$ npm install
$ hexo server

$npm install 安装相关依赖
```

| 常用命令      | 简写   | 中文含义                     |
| :------------ | :----- | :--------------------------- |
| hexo server   | hexo s | 本地启动                     |
| hexo generate | hexo g | 生成静态文件                 |
| hexo deploy   | hexo d | 部署网站                     |
| hexo clean    |        | 清除缓存和已经生成的静态文件 |

https://hexo.io/zh-cn/

## butterfly 主题

安装 butterfly

```
git clone -b master https://github.com/jerryc127/hexo-theme-butterfly.git themes/butterfly
```

安装 pug 以及 stylus 的渲染器

```
npm install hexo-renderer-pug hexo-renderer-stylus --save
```

应用主题

修改 Hexo 根目錄下的 _config.yml，把主題改為 butterfly

```
theme: butterfly
```

https://butterfly.js.org/

## 一键部署GitHub

安装 hexo-deployer-git (https://github.com/hexojs/hexo-deployer-git)

```
$ npm install hexo-deployer-git --save
```

1. 修改配置

```
deploy:
  type: git
  repo: <repository url> #https://bitbucket.org/JohnSmith/johnsmith.bitbucket.io
  branch: [branch]
  message: [message]
```

| 参数      | 描述                                                         | 默认                                                         |
| :-------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| `repo`    | 库（Repository）地址                                         |                                                              |
| `branch`  | 分支名称                                                     | `gh-pages` (GitHub) `coding-pages` (Coding.net) `master` (others) |
| `message` | 自定义提交信息                                               | `Site updated: {{ now('YYYY-MM-DD HH:mm:ss') }}`)            |
| `token`   | 可选的令牌值，用于认证 repo。用 `$` 作为前缀从而从环境变量中读取令牌 |                                                              |

生成站点文件并推送至远程库。执行 `hexo clean && hexo deploy`。



# Hugo

# Typecho

# WordPress

WordPress是一种使用PHP语言开发的博客平台，用户可以在支持PHP和MySQL数据库的服务器上架设属于自己的网站。

# VuePress

VuePress 是基于Vue开发的平台，功能上实现了GitBook功能。