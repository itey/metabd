---
weight: 
title: "多链技术-EKT(EKT)"
description: "EKT是一个去中心化云计算区块链网络，具有高性能、资源隔离特性以及更完善的治理和发展结构"
date: 2022-03-25T21:57:40+08:00
lastmod: 2022-03-25T16:45:40+08:00
draft: false
authors: ["Metabd"]
featuredImage: "duolianjishu-ektekt.webp"
link: ""
tags: ["数字代币","多链技术-EKT(EKT)"]
categories: ["navigation"]
navigation: ["数字代币"]
lightgallery: true
toc: true
pinned: false
recommend: false
recommend1: false
---
1.简介?EKT是一个去中心化云计算区块链网络，具有高性能、资源隔离特性以及更完善的治理和发展结构。在EKT的网络中，节点根据类型进行划分，专业化记账节点（全节点）能够运行在服务器集群之上，提高整个区块链网络性能；“多主链”结构，有效实现资源隔离、“一链一场景”；设立代币持有人的委托票选制度，保障网络高效治理及良性发展。多链是平行 EKT所在的链是记录所有链和token信息的。EKT主链维护一套统一的用户系统。基于这套用户系统，无论是主链、多链还是 DApp 应用，都可以快速的利用主链已有的用户体系进行开发并获取用户。也极大的降低了用户在不同DApp 间的切换成本。另外用户可以修改公私钥对以及使用的加密算法，这使得 EKT 的用户体系的安全度会一直跟随时代的发展。即使量子计算机普及，用户也可以相应的把算法更换为抗量子攻击的新算法。EKT的token链是一个纯粹的token，不是应用链，并有专门的dapp链。EKT设计了一套独特的多链架构。在这套多链架构中，除了EKT 的主链外还支持多条并行的主链。每条主链中都会有一个主币。不同的主链可以采用不同的共识机制，默认的共识机制为DPoS。开发者可以通过主链提供的Consensus接口创建并完成自己节点的部署。??2.项目介绍?EKT是一个模块化的区块链底层框架，将构建一个基于多链架构的公有链生态系统，致力于成为支持大量应用落地的商用公链。能够为企业提供易用、灵活且高效的通用型基础技术，共同推动区块链应用场景落地。与传统的侧链架构不同的是，在EKT多链系统中，所有的链都无需同步主链数据，可以完全独立。同时，我们还提供相同链的跨合约调用以及跨不同链的合约调用。在EKT中，默认共识机制为DBFT，智能合约的开发语言是JavaScript，并将陆续支持其他主流语言。项目特点多链架构与跨链协议：
研发独特的多链架构，除 EKT主链外同时支持多条并行主链，每条主链有一个主币。不同主链可采用不同的共识机制，默认共识机制为 DPOS。 通过跨链报文协议，使资产跨公链自然流通。智能合约新语言：
EKT提供一套全新的智能合约开发语言 AWM，使开发者方便地根据业务需求定制自己的智能合约。智能合约的运行环境为 AWM VM，利用该虚拟机进行本地调试，能够极大提高开发效率。DPOS+Paxos共识算法：
基于DPOS + Paxos 的共识机制，使得公链中用户数量越多，理论TPS越高，并可以趋于无限大。另外，开发者只需关心业务逻辑，进行基本的学习后短时间内就可以快速上手创建自己的区块链世界的DApp。应用场景多信任主体：区块链是信任机器，应用环境最好是相互之间没有天然信任关系，需要通过区块链来搭建信任。多方协作：如果该场景协作方多，对账成本高，区块链底层的共享账本之上搭建的智能合约能够降低对账成本，从而提升效率。中低频交易：区块链目前的并发性和扩展性还不足以应用于大规模高频交易。在多链多共识的机制下，EKT区块链利用跨链技术的优势，对多条链的应用场景进行整合并统一进行管理，形成多共识应用场景生态。EKT区块链的多链结构能够满足应用场景的使用多样性，这增加了多功能平台的多重整合的可能，同时，多链结构和跨链价值交换又能保持整个生态系统的良性运转。在多个代币形成的架构中，主链将维持着所有代币的平衡和使用，使得所有代币都能正常的运转，带动子链生态的和谐发展。技术概况在 EKT 区块链网络中，“主链”构成了信息主干道，不同的母链之间通过链路由协议交换信息。同时，一个主链上承载着不同的同构子链，这些子链是某个垂直领域或多个异业集群的分布式账本实现。子链间的通信则由跨链通信协议实现。通过区块链的分片，提高区块链系统的交易处理能力。相较于一条单独的区块链系统，链集群系统可以通过连接多条子链的方式在交易处理能力上直线增长。交易的请求通过链路由的分配进入不同子链，可以有效规避针对一条子链的集中请求。此外，可以在链路由上部署同构子链的不同节点数的集群，对于同构链而言，多节点数量的集群会有相对较高的安全性，少节点集群的处理速度则更快。并且，根据节点数量，地理位置，业务分类等不同需求，部署不同的链集群，对应不同需求将请求分发到合适的集群之中处理，帮助链网络根据业务需求灵活部署，为用户提供更高质量的区块链服务。??3.评述?EKT创建了一个全新的区块链底层架构，拆分Token和Dapp，保证分布式应用开发的简易性、迭代效率和安全性。将Bancor协议融合进公链架构，新发行的通证将获得稳定的流通。开发者只需关注DApp的业务逻辑，其他的一切都由EKT公链来完成。总而言之，EKT以基础型区块链技术赋能实体经济，是基于多链架构的公有链生态系统。相关链接：
https://ekt8.io/
http://www.qukuaiwang.com.cn/szhb/2773.html###
http://www.bite5.com/index.php/viewnews-255
https://bihu.com/article/1835155747
