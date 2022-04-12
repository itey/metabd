---
weight: 
title: "Immutable"
description: "Immutable 实现的原理是（持久化数据结构），也就是使用旧数据创建新数据时， 要保证旧数据同时可用且不变 。 同时为了 避免深拷贝把所有节点都复制一遍带来的性能损耗 ，Immutable 使用了（结构共享）， 即如果对象树中一个节点发生变化，只修改这个节点和受它影响的父节点，其它节点则进行共享。"
date: 2022-03-25T21:57:40+08:00
lastmod: 2022-03-25T16:45:40+08:00
draft: false
authors: ["Metabd"]
featuredImage: "528.jpg"
link: "https://www.immutable.com/"
tags: ["Immutable","数字收藏品"]
categories: ["navigation"]
navigation: ["数字收藏品"]
lightgallery: true
toc: true
pinned: false
recommend: false
recommend1: false
---
Immutable 实现的原理是（持久化数据结构），也就是使用旧数据创建新数据时， 要保证旧数据同时可用且不变 。 同时为了 避免深拷贝把所有节点都复制一遍带来的性能损耗 ，Immutable 使用了（结构共享）， 即如果对象树中一个节点发生变化，只修改这个节点和受它影响的父节点，其它节点则进行共享。
