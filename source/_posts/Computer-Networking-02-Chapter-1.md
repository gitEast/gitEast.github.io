---
title: 'Computer Networking 02: Chapter 1'
date: 2023-10-28 13:09:03
categories:
  - 'ComputerNetworking'
tags:
  - 'Computer Networking: A Top-Down Approach'
  - '理论基础'
---

> 本章内容太多了，我决定等之后回过头来再做。（也许没有之后）

## 一、基础阅读

非常惭愧，作为一个已经二十四岁的成年人，仍需锻炼基础阅读。

该部分将放置于[本篇最后](#Vocabulary)。

## 二、检视阅读

### 2.1 这一章在讲什么？

介绍 Computer Network。

### 2.2 作者是借怎样的整体架构来陈述他对这个主题的理解？

总分总架构。

1. Computer Network 的基本组成部分：核心术语 —— Protocol
2. 从网络的边缘深入至中心
3. 网络的连接：Internet is a network of networks.
4. 更加深入、抽象的认识
   1. 延迟、丢失与吞吐量
   2. 分层模型
   3. 不同类型的网络攻击
5. 计算机网络的简短历史
6. 总结与期望

## 三、分析阅读

### 3.1 架构纲要

#### 3.1.1 哪一类：实用性 VS 理论性

#### 3.1.2 使用一个单一的句子或最多几句话(一小段文字)来概括内容

#### 3.1.3 将重要篇章列举出来，说明它们如何按照顺序组成一个整体架构

1. today's Internet is the largest engineered system, 引出通过本书来学习 Internet。
2. a broad overview of computer network and the Internet
3. structure the overview:
   1. introduce some basic terminology and concepts
   2. examine the basic hardware and software components
      1. network's edge:
         - end systems
         - applications
      2. network's core
         - links and switches that transport data
         - access networks and physical media
   3. Internet is a network of networks: these networks connects with each other
4. broader and more abstract view
   1. delay, loss and throughput of data
   2. key architecture principles: protocol layering and service models
   3. many different types of attacks
5. a brief of computer networking

#### 3.1.4 找出作者要问的问题

### 3.2 诠释内容

#### 3.2.1 找出关键字，透过它们与作者达成共识

1. 第一节
   - end system
   - packet switch
   - communication link
   - ISP Internet Service Provider
   - TCP/IP
   - protocol: A protocol defines the format and the order of messages exchanged between two or more communicating entities, as well as the actions taken on the transmission ad/or receipt of a message or other events.
2. 第二节
   - end system, host
   - access network
     - Home Access
     - Access in the Enterprise(Home)
     - Wide-Area Wireless Access
   - guided media
   - unguided media
   - packet switch
   - store-and-forward transmission
   - queuing delay
   - packet loss
   - forwading table
   - routing protocol
   - packet switching
   - circuit switching
3. 第三节
4. 第四节
   - processing delay
   - queuing delay => packet loss
   - transmission delay
   - propagation delay
   - end-to-end delay
   - throughput
   - server
   - client
   - Layered Architecture
     - Application Layer
       - HTTP
       - DNS
       - message
     - Transport Layer
       - TCP
       - UDP
       - segment
     - Network Layer
       - IP
       - datagram
     - Link Layer
       - Ethernet
       - WiFi
       - frame
     - Physical Layer
   - encapsulation => de-encapsulation
   - attacks

#### 3.2.2 将一本书中最重要的句子圈出来，找出其中的主旨

#### 3.2.3 从相关文句的关联中，设法架构出其基本论述

#### 3.2.4 找出作者的解答：已解决、未解决、无法解决

### 3.3 批评式阅读

## Vocabulary

| word                  | meaning                                                    | 原文                                                               |
| --------------------- | ---------------------------------------------------------- | ------------------------------------------------------------------ |
| arguably              | adv. 可能，大概 I think it is true.                        | is arguably the largest engineered system                          |
| tablet                | n. 掌上电脑                                                | laptops, tablest, and smartphones                                  |
| surveillance          | n. 监视，盯梢                                              | surveillance systems                                               |
| thermostat            | n. 温度自动调节器，恒温器                                  | eye glasses, thermostats, and cars                                 |
| diverse               | adj. 多种多样的，形形色色的                                | so many diverse components and uses                                |
| resounding            | adj. 响亮的，洪亮的                                        | a resounding YES!                                                  |
| insight               | n. 洞察力，深刻见解                                        | giving you the principles and practical insights                   |
| cover a lot of ground | 涉及面广                                                   | cover a lot of ground in this introductory chapter                 |
| introductory          | adj. 引导的，序言的                                        | this introductory chapter                                          |
| structure             | v. 组织，构成                                              | structure our overview of computer networks                        |
| terminology           | n. 术语                                                    | some basic terminology and concepts                                |
| throughput            | n. an amount of work done in a particular period of time   | delay, loss, and throughput of data                                |
| quantitative          | adj. 定量的                                                | simple quantitative models                                         |
| propagation           | n. 繁殖，传播                                              | propagation delay                                                  |
| queue                 | v. 排队                                                    | queuing delay                                                      |
| architectural         | adj. relating to architecture                              | the key architectural principles                                   |
| namely                | adv. 即，也就是说 more detail or be more exact             |                                                                    |
| vulnerable            | adj. 易受到攻击的，脆弱的                                  | be vulnerable to many different types of attacks                   |
| nuts and bolts        | 螺母和螺钉，基本组成部分                                   | the nuts and bolts of the Internet                                 |
| in terms of           | used to describe which particular area of a subject        | describe the Internet in terms of a networking infrastructure      |
| infrastructure        | n. 基础设施                                                | infrastructure that provides services to distributed applications  |
| distributed           | adj. 分布式的                                              | distributed applications                                           |
| figure                | n. (书 or 文件中常带有编号的)图，表                        |                                                                    |
| illustrate            | v. (尤指用例子)说明，阐述                                  | using Figure 1.1 to illustrate our discussion                      |
| primarily             | adv. mainly                                                |                                                                    |
| furthermore           | adv. 此外，而且                                            | Furthermore, ...                                                   |
| appliance             | n. 装置，器械，家用电器                                    | home appliances                                                    |
| jargon                | n. 行话，行业术语                                          | in Internet jargon                                                 |
| estimate              | n. 估计，估算，估价                                        | by some estimates                                                  |
| coaxial               | n. 同轴的，共轴的                                          | coaxial cable                                                      |
| spectrum              | n. 光谱，波谱，声谱，频谱                                  | radio spectrum                                                     |
| segment               | v. 分离，分割                                              | segment the data                                                   |
| reassemble            | v. 再集合，使重聚                                          | they are reassembled into the original data                        |
| flavor                | n. 特色，风味，味道                                        | in many shapes and flavors                                         |
| prominent             | adj. very well known and important                         | the two most prominent types                                       |
| ultimate              | adj. 最终的                                                | the ultimate destinations                                          |
| sequence              | n. 一连串 a series of related things                       | the sequence of communication links and packet switches            |
| traverse              | v. 穿越，穿过                                              | traversed by a packet                                              |
| predict               | v. 预言，预计                                              | predict that ...                                                   |
| transportation        | n. 运输，运送，输送                                        | transportation networks of highways, roads and intersections       |
| intersection          | n. 十字路口，交叉路口                                      | highways, roads and intersections                                  |
| factory               | n. 工厂                                                    | a factory                                                          |
| cargo                 | n. （大型交通工具装载的）货物                              | a large amount of cargo                                            |
| warehouse             | n. 仓库，货仓                                              | warehouse located thousands of kilometers away                     |
| fleet                 | n. 车队，船队，海军                                        | a fleet of trucks                                                  |
| truck                 | n. 卡车，货车                                              | a fleet of trucks                                                  |
| sheepment             | n. 运输的货物，运输，装运                                  | a shipment of urgent medical supplies                              |
| analogous             | adj. 相似的，类比的                                        | packets are analogous to trucks                                    |
| residential           | adj. 居民区的                                              | residential ISPs                                                   |
| corporate             | adj. (大)公司的                                            | corporate ISPs                                                     |
| broadband             | n. 宽带                                                    | residential broadband access                                       |
| tier                  | n. one of several layers or levels                         | these lower-tier ISPs                                              |
| conform               | v. 顺从，遵从                                              |                                                                    |
| convention            | n. 约定，协定                                              | conform to certain naming and address conventions                  |
| collectively          | adv. 集体地，全体地，共同地                                | are collectively known as TCP/IP                                   |
| interoperate          | v. (多个系统)协调运作                                      | systems and products that interoperate                             |
| hence                 | adv. 因此，所以 that is the reason or explanation for      | hence the name                                                     |
| precursor             | n. 先驱，先兆                                              | the precursor to the Internet                                      |
| video conferencing    | 视频会议、电视会议                                         |                                                                    |
| recommendation        | n. 推荐，介绍                                              | location-based recommendation systems                              |
| facilitate            | v. to make something possible or easier                    | facilitate the exchange of data among end systems                  |
| sink                  | n. 水槽                                                    | the sink of data 数据的汇聚                                        |
| humanity              | people in general (统称)人，人类                           | may greatly benefit humanity                                       |
| instruct              | v. (正式地)命令，指示                                      | one end system instruct the Internet to deliver data               |
| seal                  | v. 密封，封上                                              | seal the envelope                                                  |
| scale                 | n. 大小，规模 -> 秤                                        | body scale 体重秤                                                  |
| buzzword              | n. 时髦词语                                                | another important buzzword in computer networking                  |
| execute               | v. to do or perform something, especially in a planned way | execute protocols                                                  |
| dictate               | v. 规定，要求                                              |                                                                    |
| initiate              | v. 开始，创始                                              | initiate communication with someone else                           |
| implicitly            | adv. 含蓄地，不明言地                                      | Implicitly, ...                                                    |
| cordial               | adj. friendly, but formal and polite                       | take a cordial "Hi" response                                       |
| indication            | n. 表示，显示，暗示                                        | an indication that one can ...                                     |
| proceed               | v. to continue as planned                                  | one can proceed and ask for the time of day                        |
| drone on              | 喋喋不休 to talk for a long time in a boring way           | is droning on about protocols                                      |
| conventional          | adj. 传统的，常规的                                        | a set of conventional actions                                      |
| capable               | adj. 有能力的，熟练的，能干的                              | other network-capable device                                       |
| scenario              | n. 可能发生的事态，设想                                    | the scenario is illustrated                                        |
| extensive             | adj. covering a large area, having a great range           | make extensive use of protocols                                    |
| intellectually        | adv. 理智地，运用智力地                                    | complex and intellectually deep                                    |
| equivalent            | adj. 等值的，相等的，等同的                                | is equivalent to ...                                               |
| present               | v. to give, provide, or make something known               | present a high-level overview of the Internet                      |
| delve                 | v. to search, especially as if by digging                  | delve a bit more deeply into the components of the Internet        |
| interchangeably       | adv. 可互换的                                              | use the terms hosts and end systems interchangeably                |
| informally            | adv. 非正式地，随意地                                      | Informally, clients tend to be desktops                            |
| whereas               | con. 尽管，但 compared with tha fact that                  |                                                                    |
| distribute            | v. 分发，分散                                              | distribute Web pages                                               |
| reside                | v. to live, have your home, or stay in a place             | reside in large data centers                                       |
| continent             | n. 洲，大陆                                                | Google has 19 data centers on four continents                      |
| massive               | adj. vary large in size, amount, or number                 | Alibaba have built massive data centers                            |
| internally            | adv. 内心地，内在地                                        | data centers internally include complex computer networks          |
| concreteness          | n. 具体化                                                  | describe in the context of Amazon for concreteness                 |
| commerce              | n. 商业，商务，贸易，交易                                  | e-commerce                                                         |
| purchase              | n. something that you buy, the act of buying sth           | purchase information                                               |
| parallel              | adj. 同时发生的，平行的                                    | parallel computing infrastructures                                 |
| processing            | n. 处理，审批                                              | data processing tasks                                              |
| computation           | n. 计算                                                    | collectively perform massively distributed computations            |
| blade                 | n. 刀身，刀片，支架                                        |                                                                    |
| resemble              | v. to look like or be like someone or something            |                                                                    |
| commodity             | n. 商品，货物                                              | commodity hosts                                                    |
| stack                 | v. to arrange things in an ordered pile                    | the hosts are stacked                                              |
| rack                  | n. 架子，置物架                                            | are stacked in racks                                               |
| sophisticated         | adj. 精于世故的，老练的，复杂的                            |                                                                    |
| evolve                | v. 使发展，使进化                                          | sophysticated and evolving data center network designs             |
| household             | n. a group of people, often a family                       | the households in Europe                                           |
| prevalent             | adj. 流行的，盛行的，普遍的                                | the two most prevalent types                                       |
| multiplexer           | n. 多路选择器                                              | a digital subscriber line access multiplexer                       |
| tone                  | n. 声调                                                    | high-frequency tones                                               |
| simultaneously        | adv. 同时地                                                | carries both data and traditional telephone signals simultaneously |
| multiplexing          | n. 多路                                                    | this technique of frequency-division multiplexing                  |
| splitter              | n. 分割器                                                  | a splitter separates the data and telephone signals                |
| aggregate             | adj. 合计的，总数的                                        |                                                                    |
| asymmetric            | adj. 不对称的，不匀称的                                    | be asymmetric                                                      |
| purposefully          | adv. 有目的地                                              | may purposefully limit a residential rate                          |
| maximum               | adj. 最大的，最高的，顶点的                                | the maximum rate                                                   |
| gauge                 | n. 内径，口径                                              | the gauge of the twisted-pair line                                 |
| expressly             | adv. for a particular purpose                              | Engineers have expressly designed DSL                              |
| junction              | n. 联结点，枢纽，交叉口                                    | neighborhood-level junctions                                       |
| external              | ajd. of, on, for, or comming from the outside              | is an external device                                              |
| allocate              | v. 分配，分派，拨给                                        | the downstream channel typically allocated a higher rate           |
| respectively          | adv. 分别                                                  |                                                                    |
| contracted            | adj. 缩小的                                                | lower contracted data rates                                        |
| impairment            | n. 损伤，损耗                                              | media impairments                                                  |
| coordinate            | v. 协调，使相互配合                                        | coordinate transmissions                                           |
| collision             | n. 碰撞，冲突                                              | avoid collisions                                                   |
| potentially           | can potentially provide                                    |
| gigabit               | n. 吉比特 1,000,000,000 bits                               | the gigabits per second range                                      |
| dedicated             | adj. 专门的，专用的                                        | dedicated optical fiber to a neighborhood splitter                 |
| conversion            | n. 转化，改变，转变                                        | conversion between optical and electrical signals                  |
| replicate             | v. 使复现，重复，复制                                      | all packets are replicated at the splitter                         |
| -prone                | suffix. 较常碰到...问题的                                  | failure-prone                                                      |
| beam                  | n. 光线，光束                                              | beam-forming technology                                            |
| corporate             | adj. relating to a large company                           | on corporate and university campuses                               |
| campus                | n. (大学)校园，校区                                        | on corporate and university campuses                               |
| colloquially          | adv. 口语地，通俗地                                        | more colloquially known as WiFi                                    |
| roaming               | n. 漫游                                                    | a roaming laptop                                                   |
| telephony             | n. the activity or process of communicating by phone       | cullular telephony                                                 |
| investment            | n. 投资                                                    | make enormous investments in sth                                   |
| indicate              | v. to show, point, or make clear in another way            | indicate the physical media used                                   |
| kick                  | v. 踢，踹                                                  | gets kicked around 被踢来踢去                                      |
| thereafter            | adv. 之后，以后                                            |                                                                    |
| propagate             | v. 传播，散播                                              | propagate electromagnetic waves                                    |
| electromagnetic       | adj. 电磁的                                                | propagate electromagnetic waves                                    |
| pulse                 | n. 脉冲                                                    | optical pulses                                                     |
| terrestrial           | adj. relating to the earth                                 | terrestrial radio spectrum 地面无线电频谱                          |
| solid                 | adj. not liquid or gas 固态的                              | a solid medium                                                     |
| minor                 | adj. 次要的，轻微的                                        |                                                                    |
| magnitude             | adj. 巨大的                                                | magnitude heigher than                                             |
| handset               | n. 手机，移动电话                                          | telephone handset                                                  |
| insulate              | v. 使隔热，使隔音，使绝缘                                  | two insulated copper wires                                         |
| spiral                | n. 螺旋形                                                  | in a regular spiral pattern                                        |
| emerge                | v. 出现，浮现，露出                                        | fiber-optic technology emerged in the 1980s                        |
| disparage             | v. 贬斥，贬低                                              | many people disparaged twisted pair                                |
| dial-up               | adj. 拨号上网的                                            | dial-upo modem technology                                          |
| conductor             | n. 导体                                                    | two copper conductors                                              |
| concentric            | adj. (指圆)同心的，同轴的                                  | the two conductors are concentric rather than parallel             |
| construction          | n. 构造                                                    | with this construction                                             |
| insulation            | n. 隔音，隔热，绝缘                                        | special insulation                                                 |
| couple                | v. to join or combine                                      | cable television systems are coupled with caple                    |
| tremendous            | adj. 巨大的，极好的                                        | support tremendous bit rates                                       |
| immune                | adj. 不受影响的                                            | are immune to electromagnetic interference                         |
| interference          | n. 干涉，干预，干扰                                        | electromagnetic interference                                       |
| attenuation           | n. 衰减                                                    | signal attenuation                                                 |
| tap                   | v. 窃听                                                    | are very hard to tap                                               |
| long-haul             | adj. 长途的，远途的                                        | long-haul guided transmission media                                |
| elsewhere             | adv. 在别处                                                |                                                                    |
| exclusively           | adv. only                                                  | use fiber optics exclusively                                       |
| the backbone of sth   | 主要成分，支柱，中枢                                       | in the backbone of the Internet                                    |
| hinder                | v. 阻碍，妨碍                                              | the high cost of optical devices has hindered their deployment     |
| carrier               | n. 搬运人，运送人，运输工具                                |                                                                    |
| specification         | n. 标准，规格，规范                                        | these specifications are often referred to as OC-n.                |
| terrestrial           | adj. relating to the earth                                 | terrestrial radio channels                                         |
| electromagnetic       | adj. 电磁的                                                | electromagnetic spectrum                                           |
| spectrum              | n. 光谱，波谱，声谱，频谱                                  | electromagnetic spectrum                                           |
| penetrate             | v. 穿透，进入，渗入                                        | penetrate walls                                                    |
| fade                  | v. 使褪色，使衰弱，使变暗                                  | shadow fading 阴影衰弱                                             |
| obstruct              | v. 阻塞，堵塞，阻碍                                        | around/through obstructing objects                                 |
| satellite             | n. 人造卫星                                                | satellite radio channels                                           |
| band                  | n. a particular range of values, numbers, etc              | on one frequency band                                              |
| geostationary         | adj. 静止的                                                | geostationary satellites                                           |
| orbit                 | v. 绕轨道运行                                              | low-earth orbiting satellites                                      |
| permanently           | adv. always and for ever                                   | Geostationary satellites permanently remain above the same spot    |
| spot                  | n. a particular place                                      | the same spot                                                      |
| stationary            | adj. not moving, or not changing                           |                                                                    |
| presence              | n. the fact that someone or something is in a place        | this stationary presence                                           |
| introduce             | v. 采用                                                    | introduce a substantial signal propagation delay                   |
| substantial           | adj. 巨大的                                                | a substantial signal propagation delay of 280 milliseconds         |
| nevertheless          | adv. despite what has just been said or reffered to        |                                                                    |
