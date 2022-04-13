---
weight: 
title: "阿童木-Cosmos(ATOM)"
description: "ATOM（Cosmos）-阿童木：Cosmos是一个并行网络，各链由诸如Tendermint共识提供支持"
date: 2022-03-25T21:57:40+08:00
lastmod: 2022-03-25T16:45:40+08:00
draft: false
authors: ["Metabd"]
featuredImage: "atongmu-cosmosatom.webp"
link: ""
tags: ["数字代币","阿童木-Cosmos(ATOM)"]
categories: ["navigation"]
navigation: ["数字代币"]
lightgallery: true
toc: true
pinned: false
recommend: false
recommend1: false
---
一、ATOM（Cosmos）-阿童木项目简介：?Cosmos是一个并行网络，各链由诸如Tendermint共识提供支持。在cosmos生态系统中各空间可以相互通信、交易、互操作。Cosmos的愿景是打破区块链之间的障碍，创建一个区块链互联网，成为各种实际使用场景的优先选择平台。这一实现伴随着一系列系统工具的开发，包括Tendermint，Cosmos SDK、IBC，Hub和Zone之间的通信，通过IBC协议实现。以太坊所采用的Go-Ethereum是单片技术堆栈范畴，对其特性的一些升级、以及定制性的提升，是2014成立的Tendermint最早的切入点。Tendermint BFT是一种解决方案，它将区块链的网络层和共识层打包，开发人员只需专注于应用层而无需在意底层协议，这一对开发者友好的设计在公链泛滥的当今看起来并无新意，但如果考虑这一设想最早出现在2014年底，就能自然而然明白cosmos的前瞻性了。此外，Tendermint 共识算法的主要好处就是它具有安全简易的轻客戸端，这一点使其成为手机和物联网用例的理想工具。Tendermint 轻客戸端只需和验证组的变化保持一致，然后验证最新区块中预先提交的+?，来确定最新情况。 总而言之，跨链不是comos的全部，Tendermint技术在开发时间的节省上也下了很大的功夫，Tendermint BFT的属性适用公链、私链，Tendermint BFT仅处理区块链的网络和共识，节点传播事务和验证器就一组事务达成一致，以附加到区块链，每秒可处理数千事务。?COSMOS建立在Tendermint的BPOS+PBFT的共识机制上。该机制涉及验证人与提议人。PBFT则用来确认区块的有效性，抵押代币的数量决定验证人投票的权重过程中的权力，BPOS用来分配验证人的权力。每轮的提议人会从验证人顺序列表中按照其选票比例来选择确定。Tendermint采用由绝对多数的选票三分之二选定的最优拜占庭容错算法。??二、Cosmos SDK?? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ? ?图1 Cosmos SDK功能SDK在Tendermint BFT的基础上，进一步缩短第三方开发者的研发周期，首先，它允许开发人员在Golang上移植任何现有的区块链代码库，Ethermint面向以太坊网络。所有现有的工具（Truffle，Metamask等）都与Ethermint兼容，无需额外工作即可移植智能合约。cosmos SDK基于两个主要原则，在此基础上进一步规范了框架：??模块化： Tendermint团队构建了Cosmos Hub所需的基础模块。任何开发人员在构建自己的应用程序时都可以使用这些模块。并可以为Cosmos SDK创建一个模块。
??安全边界：限制模块之间的安全边界，使开发人员能够更好地处理模块的可组合性，同时，限制恶意或意外交互的范围。Cosmos SDK的详情可以在官网进行查阅，提供了用于构建命令行界面（CLI），REST服务器和各种其他常用的实用程序库。??三、IBC?在cosmos网络中，区块链之间的连接通过区块间通信协议（IBC）协议实现。IBC利用Tendermint共识，允许异构链将值（即token）或数据相互转移。异构链的特点是具有不同的层，各区块链由一组验证器维护，这些验证器称为矿工。在各自的网络中，共识、应用层皆有不同，为了与IBC兼容，需要遵循一些共识层的要求。IBC允许异构区块链相互传递令牌和数据，这意味着具有不同应用程序和验证器集的区块链是可互操作的。链A上的一个帐户想要发送10个令牌到链B时，系统将连续地进行跟踪，将允许每个链跟踪另一个链的验证器集。且每一条链都运行另一条链的轻客户端。启动IBC传输时，IBC协议中的两个关键信息分别是IBCBlockCommitTx和IBCPacketTx，前者记录发送方所在的最新区块信息；后者是跨链交易本身的信息，执行时通过提及跨链指令存入outgoing队列；从outgoing队列取出交易信息，提交到Hub，由Hub执行后续步骤，以实现跨链交易。在此过程中，ATOM被锁定（绑定）在链A上，然后将10个ATOM的证据从链A转发到链B，并在链B上针对链A的有效性进行验证，如果有效，则在链B上创建10个ATOM凭证。在链B上创建的ATOM不是真正的ATOM，类似的机制用于在ATOM返回其原始链时解锁ATOM。在IBC的设计原理上，通过直接连接可以将网络中的每个区块链彼此串联起来。但这种情况需要面临二次增长的不可控性，为了解决这个问题，Cosmos提出了一种模块化架构，在网络中具有两类区块链：枢纽Hub和区域Zone。前者专门设计用于将区域连接在一起。当区域与枢纽建立IBC连接时，它可以自动访问（即发送和接收）与其连接的每个其他区域。因此，每个区域只需要与一组受限的枢纽建立有限数量的连接。还可以防止区域内的双重支出。空间内部所有代币的转移将通过Cosmos Hub，Hub将完成各空间代币持有总量的记录，以及各空间的隔离，并囊括用户数据报协议（UDP）、传输控制协议（TCP）。Hub与各空间的状态变化会保持信息通信的一致，通过发布梅克尔证明（Merkle-proof）来说明信息已经被传送或接收。Cosmos将在发布时提供良好的垂直可扩展性，在完成IBC模块后，将实施水平可扩展性解决方案。在Cosmos Network中推出的第一个Hub是Cosmos Hub。其令牌称为ATOM。Cosmos 中的验证人类似于提供机器的矿工，非验证人将ATOM权益代币委托用于投票。以此实现一定的ATOM奖励分配，当验证人被攻击或作恶时，系统采用一定的机制进行惩罚和削弱。??四、Cosmos可解决的区块链问题?1、可扩展性
工作量证明协议缓慢，昂贵，不可扩展且对环境有害。
Tendermint BFT解决了这个问题。
Tendermint BFT是拜占庭式容错共识引擎，可为Cosmos权益证明提供支持。2、易用性
区块链应用程序很复杂，开发人员很难理解。
Cosmos SDK修复了此问题。
Cosmos SDK是用于构建可互操作的，特定于应用程序的区块链的模块化框架。3、互通性
区块链经济孤立无援，彼此之间无法转移资产。
IBC协议解决了这个问题。
区块链间通信（IBC）是一种类似于TCP / IP的区块链消息传递协议。??五、主要特点和里程碑?Tendermint Core:?“Tendermint Core”是一款即用型区块链引擎，配备 Cosmos 实用拜占庭容错共识协议。内核可用于搭建公共或私有区块链。共识机制提供即时结算和安保；优先保障安全，其次才是网络活跃度。Cosmos SDK:?作为便利工具包，Cosmos SDK 有助开发者搭建应用专属的区块链。跨链通信:?为了向开发者提供更多搭建区块链的工具，Cosmos 项目的下一个目标是提高不同区块链之间的互操作能力，实现跨链和跨层交易。借助分区组合，用户得以在 IBC 兼容链组成的代币生态系统内自由交易。相关链接：
https://cosmos.network/intro
https://www.dprating.com/rating/report/114
https://cosmos.network/resources/whitepaper
