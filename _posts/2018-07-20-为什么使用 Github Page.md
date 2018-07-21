---
layout: post
title:  "为什么使用 Github Page?"
date:   2018-07-20
---

创建个人博客有很多选择，都有一些我不喜欢的点：

- 公众号：不能随时修改
- 简书：在本地 typora 编辑好之后，插入的图片无法直接复制到网站的编辑器，得重新手动导入图片。
- hugo/hexo：需要配置服务器，域名登记，需要时间。
- jekyll：对接 github page，配置简单。而且使用标准的 markdown，之后可以迁移到其他博客系统也很方便。但是 github 网络可能不稳定，同步到github、打开博客网页的速度无法保证。
- ghost：动态博客，有本地编辑器，支持直接插入图片。但是我不想用 ghost 的编辑器，我只想用我熟悉的 Typora。

Jekyll 是我最能接受的选择。

我创建 github page 的方法步骤：

1. git clone 我喜欢的主题 http://jekyll-new.joelglovier.com 到本地
2. 更改配置
   - CSS 样式
   - 时间格式，我喜欢 `%Y-%m-%d` 格式
   - _config.yml
   - 删除 _posts 目录下默认的文章
   - 更改 _includes/footer.html, _includes/header.html 文件
   - 删除 _assets 目录下不必要的文件
   - 删除不必要的其他页面
   - 只需要留下这些文件和目录：_assets, css, _posts, _includes, _layouts, index.html, _config.yml, CNAME
3. 在 github 创建一个新的 repository，名称为 jasonzhouu.github.io，jasonzhouu 是我的 github 账户名，github page 规定必须以自己的账户名 + github.io 的格式
4. 将本地更改好配置的目录添加 remote, 并 `git push`