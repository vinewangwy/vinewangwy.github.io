---
title: 搭建hexo博客并记录相关命令
tags:
- 博客
- hexo
categories: 个人
---
2019.11.16
第一篇文章

立个flag
每月更新一篇

## 记录hexo命令
### 启动服务器本地测试
{% codeblock %}
hexo s
{% endcodeblock %}

### 发布到github
{% codeblock %}
hexo clean && hexo g && hexo d -g
{% endcodeblock %}

### 新建文章
{% codeblock %}
hexo new [layout] <title>
{% endcodeblock %}

### 新增文章的分类和标签
{% codeblock %}
---
title: Hello World
tags: //标签
- 博客 
- hexo
categories: 个人 //分类
---
{% endcodeblock %}