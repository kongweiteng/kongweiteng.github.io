---
layout:     post
title:      "《Java并发编程的艺术"
subtitle:   "《Java并发编程的艺术》读后感-基础篇"
date:       2018-11-09 10:00:00
author:     "kwt"
header-img: "/static/img/home-bg-art.jpg"
catalog: true
tags:
    - java
    - concurrent
---
·
> “Yeah It's on. ”


## 开篇
本来想学习完正本书之后再写一篇笔记，用于加深印象，由于平时工作也不是很轻松，一本书读下来还确实需要不少时间，然而读到半本的时候感觉之前读过的章节忘了不少，
所以决定先把之前的东西总结和加深下记忆。

## 名词解释

#### 上下文切换
* 在单核处理器时代也是能够支持代码的多线程执行的，不多需要CPU不断地给每个线程分配CPU的时间片来实现单核对多线程的支持。时间片分给每个线程的时间很短，并且
还在不停的切换，才会让人感觉到是多个线程再同时工作，时间片一般是几十毫秒。
* 其实同理到了多核处理器的时候后，多个CPU在不停的切换，那就执行效率比单核服务器感觉强了很多。所以在使用多线程的时候，不仅仅是需要把代码写好，也要根据我们
生产服务器的配置，进行配置线程的数量，尽量能够往服务器在减少切换次数，并且能提高处理效率的方向设计就对了。


