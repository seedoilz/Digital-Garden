---
aliases:
  - Dependecy Injection
title: DI
date created: 2024-03-05 16:03:00
date modified: 2024-03-20 11:03:09
tags:
  - code/web
---
### 概念
指[[Spring]]创建对象的过程中，将对象依赖属性通过配置进行注入

#### 实现方式
- 第一种：set注入
- 第二种：构造注入
所以结论是：[[IoC]] 就是一种控制反转的思想， 而 DI 是对[[IoC]]的一种具体实现。

Bean管理说的是：Bean对象的创建，以及Bean对象中属性的赋值（或者叫做Bean对象之间关系的维护）。