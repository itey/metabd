---
weight: 
title: "纳世-NULS(NULS)"
description: "纳世链（NULS）是一个面向定制化服务的区块链基础设施，一个全球化的开源社区"
date: 2022-03-25T21:57:40+08:00
lastmod: 2022-03-25T16:45:40+08:00
draft: false
authors: ["Metabd"]
featuredImage: "nashi-nulsnuls.webp"
link: ""
tags: ["数字代币","纳世-NULS(NULS)"]
categories: ["navigation"]
navigation: ["数字代币"]
lightgallery: true
toc: true
pinned: false
recommend: false
recommend1: false
---
1.简介纳世链（NULS）是一个面向定制化服务的区块链基础设施，一个全球化的开源社区项目。NULS采用微服务思想，实现高度模块化的底层架构，运用模块仓库、智能合约和跨链等技术，同时结合链工厂快速搭链的能力，降低区块链开发成本，推动区块链商业应用落地。NULS提出模块化思维与多链并行的微服务架构，秉承以“链”为核心的发展理念，打造核心产品“链工厂”。基于NULS，用户可以灵活选择网络模块、共识模块、存储模块、账本模块、智能合约等核心功能模块创建NULS链网中新的区块链，也可以通过很少的编程工作通过智能合约来定义自己的业务逻辑。?2.项目介绍纳世链（NULS）是一个提供可定制化服务的区块链基础设施，是全球性区块链开源社区项目。纳世链（NULS）采用微服务思想，实现高度模块化的底层架构，运用智能合约和跨链等技术，同时结合链工厂快速搭链的能力，降低区块链开发成本，推动区块链商业应用落地。应用场景提供灵活易用的区块链基础设施：
NULS 为开发者和用户提供了丰富多样的模块。开发者和用户无需研究密码学、共识机制、存储方式等底层技术细节，直接根据其业务从链工厂的模块仓库挑选所需模块并进行参数配置，即可快速搭建出一条区块链，从而降低区块链商用成本。支持海量的区块链应用场景：
在应用层面，可以预期基于区块链的应用将逐渐进入机构甚至个人的工作和生活，NULS 通过模块化提供了快速搭链的能力，通过跨链技术提供了不同区块链之间的数据和资产的流通能力，通过智能合约提供了图灵完备的可编程能力，可支持未来各种各样的应用场景。驱动区块链商用落地：
商业应用对性能的要求极高，NULS 致力于解决现有区块链的性能受限问题，采用平行扩展技术，通过链工厂搭建多条独立的链，将业务分发到各链，链与链之间使用跨链技术进行通信，以满足千万级 TPS 需求。技术概况微服务架构：
NULS 率先布局微服务架构，在区块链底层基础设施设计中引入微服务思想把软件拆分为多个可独立部署的服务，NULS 将这种软件工程中先进的设计思想引入到模块设计中，目的是让每个模块可以像独立的程序一般灵活，同时单个模块的开发可以支持多种编程语言。这种架构下模块之间的耦合度更小，多语言开发让代码的贡献以及用户使用的便利性都得到极大地提升，同时每个模块也更易于扩展，且模块支持分布式部署，这让模块的热插拔也变得更容易，我们把这整个架构设计称之为 NULS 2.0。同时链工厂和跨链也会在这个架构上进行设计。NULS 的微服务架构设计方案分为三层：
第一层为微服务基础架构层；
第二层为区块链基础服务层；
第三层为 DApp 应用层。此构架使得开发者可以在第二层上开发更高级的应用系统（比如交易所的分布式系统，数据服务系统都可以构建在第二层之上）。构建在 NULS 体系上的，不仅仅是多个链和多个 DApp，还可以是非区块链的其他大中小型互联网。模块化：
商业应用千变万化、技术升级日新月异，NULS 社区承认技术的升级和商业应用逻辑的发展不可预测，吸纳了 Linux 内核设计的模块化思想，开发了多个功能模块，集合组成了模块仓库。NULS 设计遵循“一切皆为模块”的原则，用模块化支持技术更新和应用适配。共识机制——POC：
NULS 的模块化设计，支持共识机制在内的所有核心功能模块的替换与插拔。NULS主网默认采用信用共识机制 POC(Proof-Of-Credit)。节点信用达标的情况下，锁定一定数量的 NULS 即可加入共识，共识节点重新排序后每轮轮流出块，退出共识时锁定的NULS解锁。1、共识进入与退出机制
任何人都可以随时加入 NULS 的共识之中，只要满足条件，遵守规则，即可持续获得 NULS Token 奖励。POC 的加入分为硬性指标和软性指标。硬性指标指的是信用分值必须达到一定标准线，排除掉一部分曾经作恶的节点。软性指标指的是必须锁定一定数量的 NULS 作为保证金，为杜绝节点的泛滥，同时让整个系统更加公平，锁定 NULS 的数量除了有一个最低值的限制外，任何人可自由选择，锁定的 NULS 数量会和最终的奖励挂钩。2、信用评级
在 NULS 网络中，信用是账户在系统中的诚信系数，所有账户的信用会在区间[-1,1]内，通过信用评级算法公式自动计算。信用评估公式：
信用基数=能力系数+责任系数
能力系数：根据历史出块数量计算
责任系数：根据违规情况和出块正确性计算3、共识奖励
为了整个 NULS 网络的平衡与公平，共识奖励根据所有共识节点所提交保证金与共识节点信用综合计算。4、通用共识机制
NULS 是一套通用的区块链底层基础设施，在其主网上不运行任何应用业务，所有应用业务均由平行的区块链运行。通过 NULS 的链工厂产品，能快速地部署基于模块仓库的区块链，且可灵活定制各种运行参数，包括是否支持基础Token、加密算法、共识机制、存储机制等。NULS 定义了通用共识模块，以提供接口兼容不同的共识机制。NULS 社区会陆续开发 POW、DPOS、POS、PBFT、POOL 验证池等共识机制，以供用户自由选择。NULS 智能合约：
NULS 内置 NVM 作为智能合约模块的虚拟机，从模块结构上看，NULS 智能合约模块处于对外服务模块（如 RPC 模块）和底层设施模块（如网络模块、存储模块、账户模块等）之间，账户模块、网络模块等其他模块为智能合约提供底层支撑。智能合约由上层应用定义，由解释器解释，由存储模块存储，由 NVM 运行。NULS 智能合约解释器将支持多种高级编程语言。应用开发者可以使用自己熟悉的语言设计 NULS 智能合约。跨链：
基于 NULS 模块仓库实现的区块链（生态内的区块链），可以通过模块选择的方式，添加跨链模块，实现底层上和 NULS 的互通。针对以太坊和比特币等，遵循协议跟 NULS 不同的公有链，需要通过特殊的机制实现协议的转换，将其他公有链的协议和 NULS 跨链协议做适配，达到统一协议通讯的目的。所有区块链都只和 NULS 主网通信，交易的验证由 NULS 主网负责，各平行链信任 NULS 主网的验证结果。各区块链上的资产，可以通过跨链的方式，流通到 NULS 生态中任意一条接受外链资产转入的链上，且仅需花费很小的代价。NULS 的跨链技术有如下特点：
1、NULS 主网使用 POC 共识机制，结合拜占庭容错机制实现跨链交易的确认和打包，做到去中心化、性能和安全性的兼顾；
2、NULS 主网上的每个节点都会连接多个区块链的多个节点，因为协议是统一定义的 NULS 跨链协议，所以可以实现单个节点同时连接不同的区块链上的多个节点；
3、NULS 主网提供链管理机制，用来管理所有在 NULS 主网上登记的对等区块链。登记的内容包括链信息、资产信息、跨链保证金等内容；
4、当一条区块链上收到其他链的资产时，需要在本链产生对应的资产。不同区块链上的 Token，都以资产的方式在其他链上存储；
5、一条区块链中转入其他链资产的明细会在 NULS 主网中存储，该资产转出这条区块链时，会进行验证，不允许非法的资产从该区块链中产生，对有恶意的区块链，会通过社区机制进行处理，如：暂停跨链、中止跨链、没收保证金等；
6、NULS 主网将提供 API 使用手册，任一开发者都可以根据手册开发自己的钱包、浏览器、轻钱包等工具；
7、NULS 主网中提供协议供应用扩展，可以使用该协议进行 DApp 的开发和跨链协议的优化。?3.评述纳世链（NULS）是一个提供可定制化服务的区块链基础设施，是全球性区块链开源社区项目。纳世链（NULS）采用微服务思想，实现高度模块化的底层架构，运用智能合约和跨链等技术，同时结合链工厂快速搭链的能力，降低区块链开发成本，推动区块链商业应用落地。NULS是全球性区块链开源社区项目，是一个提供可定制化服务的区块链基础设施。NULS 制定了一套工业化区块链技术标准，遵循热插拔、模块化、平行扩展原则，提供可升级的共识、网络、账本、账户、区块管理、链管理、交易管理、事件总线等功能模块。基于NULS搭建区块链，如同把CPU、硬盘、内存、主板组装成电脑一样，使用者可自由选择共识、网络、账本、账户等模块，组装成为适合自己需求的链。这条链不限于公链，亦可以是联盟链或者私链。相关链接：https://www.nuls.io/zh/
https://www.nuls.io/wp-content/uploads/2019/10/NULS_Whitepaper_zh_2.0.pdf
https://info.binance.com/cn/currencies/nuls
http://www.qukuaiwang.com.cn/szhb/2486.html###?*以上内容由1234btc官方整理，如若转载，请注明出处。
