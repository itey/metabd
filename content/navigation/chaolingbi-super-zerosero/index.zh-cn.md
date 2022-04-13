---
weight: 
title: "超零币-Super Zero(SERO)"
description: "Super Zero（SERO）是一个支持图灵完备智能合约的隐私数字货币，同时也是一个允许开发者自行发布匿名数字资产的隐私保护平台，可以让去中心化应用具有隐私保护功能"
date: 2022-03-25T21:57:40+08:00
lastmod: 2022-03-25T16:45:40+08:00
draft: false
authors: ["Metabd"]
featuredImage: "chaolingbi-super-zerosero.webp"
link: ""
tags: ["数字代币","超零币-Super Zero(SERO)"]
categories: ["navigation"]
navigation: ["数字代币"]
lightgallery: true
toc: true
pinned: false
recommend: false
recommend1: false
---
一、项目简介?Super Zero（SERO）是一个支持图灵完备智能合约的隐私数字货币，同时也是一个允许开发者自行发布匿名数字资产的隐私保护平台，可以让去中心化应用具有隐私保护功能。SERO是区块链行业发展的一个里程碑，SERO通证支持Token、Ticket和Package，不但可以作为匿名数字资产，也能用于保存有隐私需求的复杂数据结构，让未来区块链技术可以更多的商用化，同时保证商业敏感信息不在区块链上泄露。??二、SERO技术应用?1、共识机制
SERO共识当前采用Pow+Pos混合共识机制，通过激励持币用户作为PoS节点，相比于有硬件投入的PoW节点，将会获得更多的在线节点，会更有效的位置区块拓扑网络的稳定性。在PoW+PoS机制下，PoW算力负责出块，而PoS通过权益投票机制决定区块的合法性。这样，每个区块的生成，是由矿工和持币者共同参与完成，两者互相制衡，避免了任何一方的垄断现象。另外，通过PoS的投票机制，可以有效抑制区块网络硬分叉现象。PoS部分在PoW产生块后，会再通过确定性的随机函数选择投票者，需要有2/3的投票被确认才能出块，这个过程完全随机了，验证节点想要作恶需要占据2/3以上的票池份额和51%的PoW算力，极大的提高了作恶成本。SERO在研究各类共识的基础上，后续提出了?己的主链共识引擎SE-Random。SE-Random 共识引擎的设计思路受到最新一代共识研究Algorand和Ourboros的启发，只需要验证节点很少的计算开销，整个区块链网络产?分叉概率极小，并能实现近乎无限的扩展性。2、扩容机制
Plasma是一个激励和强制智能合约执?的框架。Plasma由两个核心部分构成:重组所有区块链计算为一组MapReduce函数，和一个可选的方法，在现存的区块链上，以不鼓励区块扣留的Nakamoto共识原则，来实现一个Pos的代币押金机制。3、虚拟机
SERO链的虚拟机设计为满足BASE(Basically Available， Soft state，Eventual consistency)理念的最终一致性?案，此虚拟机称为MEVM虚拟机。4、抗量子计算
SERO体系会根据项目进度和量子计算机实用化的发展适时引入抗量子计算暴力破解的加密算法，比如基于格的码系统(Lattice-based cryptography)，基于编码的密码系统(code based cryptosystems)和多元密码(multivariate cryptography)等。??三、SERO支持智能合约发行和操作匿名资产原理?根据资产流出记录方式的不同，区块链系统演化出两种不同的记账实现，分别称之为UTXO模式和ACCOUNT模式。这两种模式分别对应比特币和以太坊的模式。而SERO则采用更为复杂的混合模式。SERO将UTXO和ACCOUNT模式混合应用，在需要支持隐私保护的地方采用UTXO模式，在需要运行智能合约的地方采用ACCOUNT模式。SERO通过交易、共识、以及Pedersen Commitment算法，将这两种模式无缝的整合到一起，使智能合约能发挥令人惊讶的能力。??四、SERO发行匿名Token的原理?每种Token都有一个币名，SERO系统初始化后，默认只有一个被注册的币名SERO。在智能合约发行匿名Token的时候，必须向SERO系统注册一个全局唯一的字符串作为该Token的币名。币名可以极大的提高发行资产的可读性。SERO的智能合约可以任意发行匿名Token。当然，前提是你需要一个从未注册过的币名。一旦匿名Token发行成功，智能合约可以将Token以普通交易的形式发送到某个普通账户的暂存地址PKr，这时这些被发送的Token将以UTXO的形式脱离智能合约账户，并且与SERO币一样，进入用户的个人账户中，从而被SERO的隐私机制所保护。相关链接：
https://www.dprating.com/zh/rating/report/138
https://sero.cash/cn/details.php?id=54
