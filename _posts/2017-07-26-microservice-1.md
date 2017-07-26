---
layout: post
title:  初探微服务架构之（一）
date:   2017-07-26 
category: 分布式
tags: springcloud
comments: false
---

* content
{:toc} 

本文对微服务架构和单体架构的特点进行了说明。







## 单体架构与微服务对比

### 什么是单体架构

- 一个归档包包含了应用所有功能的应用程序， 我们通常称之为单体应用。 
- 架构单体应用的架构风格， 我们称之为单体架构， 这是一种比较传统的架构风格。


### 单体架构存在的缺点

- 复杂性逐渐变高
- 技术债务逐渐上升
- 部署速度逐渐变慢
- 阻碍技术创新
- 无法按需伸缩

### 什么是微服务

- Martin Fowler：简而言之，微服务架构风格这种开发方法，是以开发一组小型服务的方式来开发一个独立的应用系统的。其中每个小型服务都运行在自己的进程中，并经常采用HTTP资源API这样轻量的机制来相互通信。这些服务围绕业务功能进行构建，并能通过全自动的部署机制来进行独立部署。这些微服务可以使用不同的语言来编写，并且可以使用不同的数据存储技术。对这些微服务我们仅做最低限度的集中管理。
- 可参照[Microservices](https://www.martinfowler.com/articles/microservices.html)

### 微服务具备的特性
- 每个微服务可独立运行在自己的进程里；
- 一系列独立运行的微服务共同构建起了整个系统；
- 每个服务为独立的业务开发，一个微服务一般完成某个特定的功能，比如：订单管理、用户管理等；
- 微服务之间通过一些轻量的通信机制进行通信，例如通过REST API或者RPC的方式进行调用。

### 微服务的优点
- 易于开发和维护
- 启动较快
- 局部修改容易部署
- 技术栈不受限
- 按需伸缩
- DevOps

### 微服务带来的挑战
- 运维要求较高
- 分布式的复杂性
- 接口调整成本高
- 重复劳动

### 微服务设计原则
- 单一职责原则
- 服务自治原则
- 轻量级通信原则
- 接口明确原则

### 微服务的开发框架
- [Spring Cloud](http://projects.spring.io/spring-cloud)
- [Dubbo](http://dubbo.io)
- [Dropwizard](http://www.dropwizard.io)
- Consl、etcd &etc.


----

> 作者[@MasterN05](http://MasterN05.github.io/)更多文章：[个人网站](http://MasterN05.github.io/) `|` [CSDN](http://blog.csdn.net/Agogwalker/) 
