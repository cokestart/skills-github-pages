---
layout: home
title: 我的技术博客 - 学习与成长的记录
subtitle: 记录前端开发学习历程，分享技术心得与生活感悟
author: 前端学习者
avatar: https://picsum.photos/id/64/40/40  # 替换为你的头像链接
last_updated: 2025-12-06  # 自动更新首页显示的最后更新时间
---

<!-- 欢迎模块内容（会被 home 模板的 "欢迎模块" 渲染） -->
## 欢迎来到我的技术小站

你好！我是一名正在学习前端开发的程序员，这个博客是我记录学习过程的地方。在这里，我会分享：

- 前端开发基础知识（HTML/CSS/JavaScript）
- GitHub Pages 搭建与美化教程
- 学习过程中遇到的问题及解决方案
- 一些实用的开发工具和资源推荐
- 偶尔的生活随感和学习心得

无论你是刚入门的新手，还是有经验的开发者，都欢迎在这里交流学习！如果你有任何问题或建议，欢迎在留言板告诉我~

{% include tag_list.html tags="#技术博客,#前端开发,#学习记录,#GitHub Pages,#交流学习" %}


<!-- 最新文章模块（Jekyll 会自动读取 _posts 目录下的文章） -->
## 最新文章

{% for post in site.posts limit:5 %}  <!-- 显示最新5篇文章 -->
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}

<!-- 更多文章链接 -->
[查看全部文章 →](/posts)


<!-- 技术栈模块（可手动维护进度） -->
## 我的技术栈与学习进度

| 技术         | 掌握进度 |
|--------------|----------|
| HTML/CSS     | 75%      |
| JavaScript   | 55%      |
| GitHub Pages | 80%      |
| Jekyll       | 40%      |
| Markdown     | 90%      |
| React        | 10%      |

{% include tag_list.html tags="#HTML/CSS,#JavaScript,#GitHub Pages,#Jekyll,#Markdown,#React" %}


<!-- 学习生活记录（相册） -->
## 学习生活记录

学习之余，也会记录一些有趣的瞬间：

{% include gallery.html 
   images="https://picsum.photos/id/0/300/200,https://picsum.photos/id/180/300/200,https://picsum.photos/id/24/300/200,https://picsum.photos/id/42/300/200"
   captions="我的学习小角落,调试成功的代码,正在阅读的技术书,咖啡与代码更配哦"
%}


<!-- 留言板模块（需要配合 Jekyll 留言功能插件，如 jekyll-disqus） -->
## 留言板

欢迎留下你的想法和建议，一起交流学习~

{% include disqus_comments.html %}  <!-- 若使用 Disqus 评论系统 -->
<!-- 或使用 GitHub Issues 作为留言板：{% include github_comments.html %} -->
