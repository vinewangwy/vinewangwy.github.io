---
title: adonuxt和koa对比
date: 2020-03-13 14:41:40
categories: 前端
tags:
- node
---

最近分别接触了一下adonuxt和koa，做了CRUD的demo

koa
开发流程：
- 框架搭建
- 数据库建表
- sequelize从数据库导出表格到model
- 补全相关的增删查改逻辑
- 通过route配置接口内容
- 前端调用

adonuxt
adonis+nuxt的组合
开发流程：
- 框架搭建
- adonis make:migration 生成schema，在schema中使用knex建表（好处是方便以后可能存在的数据库迁移）
- adonis make:controller 生成controller，controller中自带增删查改方法，只需要在对应方法中梳理相关逻辑即可
- 通过route配置接口内容
- 前端调用

开发过程中用postman测试接口