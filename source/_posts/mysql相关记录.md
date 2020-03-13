---
title: mysql相关记录
date: 2020-02-11
tags: mysql
categories: 前端
---

{% asset_img test.jpg %}

## 启动数据库
{% codeblock %}
mysql.server start
{% endcodeblock %}

## 连接数据库
{% codeblock %}
mysql -u root -p 123456 //密码
{% endcodeblock %}

## 可通过brew安装
{% codeblock %}
brew install mysql@5.6
{% endcodeblock %}
默认安装最新版本，所以需要注明版本号

## 可通过docker安装
{% codeblock %}
docker pull mysql:5.7
{% endcodeblock %}

## 查看镜像
{% codeblock %}
docker images
{% endcodeblock %}

## 运行mysql容器
{% codeblock %}
docker run -itd --name mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123456 mysql:5.7
{% endcodeblock %}

## 查看当前运行的容器状态
{% codeblock %}
docker ps
{% endcodeblock %}

## 运行mysql
{% codeblock %}
docker start mysql
{% endcodeblock %}