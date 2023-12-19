---
title: Computer-Networking-04-Chapter-3
date: 2023-12-05 21:57:06
  - 'ComputerNetworking'
tags:
  - 'Computer Networking: A Top-Down Approach'
  - '理论基础'
---

## 一、基础阅读

该部分将放置于[本篇最后](#Vocabulary)。

## 二、检视阅读

### 2.1 这一章在讲什么？

传输层能为应用层提供的服务及其协议实现。

### 2.2 作者是借着怎样的整体架构来陈述他对这个主题的理解？

渐进式，由简单模型到复杂模型。

## 三、分析阅读

### 3.1 架构纲要

#### 3.1.1 哪一类：实用性 VS 理论性哪一类：实用性 VS 理论性

兼具。

#### 3.1.2 使用一个单一的句子 or 最多几句话来概括内容。

IP => UDP: 多路复用/解复用 => TCP: 可靠传输服务 + 拥塞控制 + 流量控制 => QUIC

#### 3.1.3 将重要篇章列举出来，说明它们如何按照顺序组成一个整体架构

- 重要篇章
  - 3.2 Multiplexing and Demultiplexing
  - 3.4 Principles of Reliable Data Transfer
  - 3.5 Connection-Oriented Transport: TCP
    - 3.5.3 Round-Trip Time Esimation and Timeout
    - 3.5.4 Reliable Data Transfer
    - 3.5.5 Flow Control
  - 3.6 Principles of Congestion Control

由简单到复杂，先原理后实现

#### 3.1.4 找出作者要问的问题

### 3.2 诠释内容

### 3.2.1 找出关键字，透过它们与作者达成共识

- GBN(Go-Back-N) 与 SR(Selective Repeat)
- RTT(round-trip time)
- flow control
- congestion control

### 3.2.2 将本章中最重要的句子圈出来，找出其中的主旨

### 3.2.3 从相关文句的关联中，设法架构出其基本论述

1. 传输层使用网络层提供的服务，向应用层提供服务。
2. 网络层服务加上多路复用/解复用技术，大体就是 UDP 了。
3. 在 UDP 的基础上，TCP 增加三次握手、流水线传送、超时重传、对接收到的包向发送方发送确认包、拥塞时降低发送频率功能。
4. 这两种协议各有各的优点，UDP 迅速，而 TCP 则保证数据的正确性、完整性。
5. 对于拥塞控制，基本有三个阶段：慢启动、拥塞避免、快速回复。其中，慢启动与拥塞避免有具体规定，而快速回复则推荐而不强行要求。

### 3.2.4 找出作者的解答：已解决、未解决、无法解决

### 3.3 批评式阅读

## Vocabulary

| word             | meaning                                                            | 原文                                                              |
| ---------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------- | --------------------------------------- |
| reside           | v. to live, have your home, or stay in a place                     | Residing between the application and network layers               |
| critical         | adj. of the greatest importance                                    | the critical role of providing communication services             |
| pedagogic        | adj. 教学法的，教育学的                                            | the pedagogic approach                                            |
| as usual         | 照常，按照惯例                                                     |                                                                   |
| emphasis         | n. the particular importance or attention                          | particular emphasis will be given to ...                          |
| examine          | v. to look at or consider carefully and in detail                  | examining the first critical function of transport layer          |
| confront         | v. to face, meet, or deal with ...                                 | confront one of the most fundamental problems                     |
| corrupt          | v. 损坏，破坏（电脑上的资料）                                      | may lose and corrupt data                                         |
| realistic        | adj. 现实的，实事求是的，务实的                                    | complicated and realistic                                         |
| scenario         | n. a description of possible actions or events                     | a series of increasingly complicated scenarios                    |
| embody           | v. to represent a quality or an idea exactly                       | how these principles are embodied in TCP                          |
| consequence      | n. （常指不好的）结果，后果                                        | the causes and consequences of congestion                         |
| obtain           | v. 得到，获得                                                      | obtain a solid understanding of the issues                        |
| solid            | adj. giving confidence or support                                  | a solid understanding                                             |
| terminology      | n. 术语                                                            | known as transport-layer segments in Internet terminology         |
| encapsulate      | v. to express or show the most importance facts                    | the segments is encapsulated within a network-layer packet        |
| extract          | v. to remove or take out sth                                       | extract the transport-layer segment from the datagram             |
| invoking         | adj. 调用的                                                        | provide transport-layer services to the invoking application      |
| whereas          | conj. compared with the fact that; but                             | Whereas a transport-layer protocol provides ...                   |
| distinction      | n. a difference between two similar things                         | this distinction is subtle but important                          |
| subtle           | adj. not loud, bright, noticeable or bovious in any way            | this distinction is subtle but important                          |
| aid              | n. help or support                                                 | examine this distinction with the aid of a household analogy      |
| respective       | adj. 各自的                                                        | do their work within their respective homes                       |
| involve          | v. 涉及，使参与                                                    | they are not involved                                             |
| vice versa       | adverb. 反过来也一样                                               | He doesn't trust her, and vice versa                              |
| saga             | n. a long complicated series of related events                     | continue with our family saga                                     |
| substitute       | n. 替代品，替代物                                                  | substitute for them                                               |
| occasionally     | adv. sometimes but not often                                       | occasionally lose letters                                         |
| constrain        | v. to control and limit something                                  | are clearly constrained by sth                                    |
| bound            | n. 界限                                                            | a maximum bound                                                   |
| underlying       | adj. positioned under the surface of sth                           | the underlying network-layer protocol                             |
| nevertheless     | adv. 尽管如此，不过                                                | Nevertheless,                                                     |
| corresponding    | adj. similar to, connected with, or caused by sth else             | offer the corresponding service                                   |
| garble           | v. to make words unclear and difficult to understand               | loses, garbles or duplicates packets                              |
| duplicate        | v. to make an exact copy of sth                                    | loses, garbles or duplicates packets                              |
| encryption       | n. （对电子信息的）加密                                            | use encryption to guarantee that ...                              |
| intruder         | n. 不速之客，闯入者，入侵者                                        | application messages are not read by intruders                    |
| confidentiality  | n. the state of being confidential 秘密性，机密性                  | guarantee the confidentiality of transport-layer segments         |
| distinct         | adj. clearly separate and different                                | two distinct transport-layer protocols                            |
| specify          | v. 具体说明，明确指出                                              | must specify one of these two transport protocols                 |
| literature       | n. 文献资料                                                        | the Internet literature(for example, the RFCs)                    |
| reserve          | v. to keep sth for a particular purpose or time                    | reserve the term datagram for the network-layer packet            |
| proceed          | v. to continue as planned                                          | before proceeding with our brief introduction                     |
| integrity        | n. the quality of being whole and complete                         | guarantee the integrity of the data                               |
| glimpse          | n. 一瞥，一见                                                      | take a glimpse at the IP service model                            |
| intact           | adj. complete and in original state                                | data will arrive intact to the destination process                |
| foremost         | adj. most important or best; leading                               | First and foremost, ...                                           |
| sequence         | n. 一连串，一系列，顺序，次序                                      | sequence numbers                                                  |
| swamp            | v. 淹没，充斥                                                      | swamp the links and routers                                       |
| excessive        | adj. too much                                                      | an excessive amount of traffic                                    |
| strive           | v. 努力，奋斗，力争                                                | TCP strives to give each connection an equal share bandwidth      |
| traverse         | v. to move or travel through an area                               | traverse a congested link                                         |
| regulate         | v. 调节，控制，管理                                                | regulate the rate                                                 |
| investigate      | v. （尤指为揭开真相）调查，审查                                    | These topics are investigated                                     |
| multiplexing     | n. 多路复用                                                        |                                                                   |
| demultiplexing   | n. 解复用                                                          | multiplexing and demultiplexing                                   |
| concrete         | adj. clear and certain, or real and existing                       | In order to keep the discussion concrete, ...                     |
| emphasize        | v. to show that sth is very important                              | we emphasize that ...                                             |
| however          | adv. in whatever way                                               | we emphasize, however, that                                       |
| corresponding    | adj. connected with, or caused by sth else                         | the corresponding process's socket                                |
| carrier          | n. a person or thing that carries sth                              | the mail carrier 邮递员                                           |
| indicate         | v. to show, point, or make clear in another way                    | indicate the socket                                               |
| restricted       | adj. limited, especially by offical rules, laws, etc               | are restricted                                                    |
| percisely        | adv. exactly 精确地，准确地，确切地                                | we can now percisely describe sth                                 |
| sebsequently     | adv. after something else                                          | all subsequently arriving segments                                |
| respectively     | adv. 分别                                                          | have their own unique IP address respectively                     |
| instructive      | adj. giving useful or intrresting information                      | it's instructive to say a few additional words                    |
| spawn            | v. 使产生，使突然增长                                              | spawn a new process for each connection                           |
| correspondence   | n. a connection between two things                                 | a one-to-one correspondence                                       |
| severely         | adv. very seriously                                                | can severely impact the performance                               |
| impact           | v. to have an influence on sth                                     | can severely impact the performance                               |
| trict            | n. an effective or quick way of doing sth                          | a number of operating system tricks                               |
| mitigate         | v. to make sth less harmful, unpleasant, or bad                    | mitigate the problem                                              |
| no-frills        | adj. 朴实无华的，只提供最起码必需品的                              | design a no-frills, bare-bones transport protocol                 |
| bare             | adj. 最基本的                                                      | bare-bones                                                        |
| bone             | n. 骨头                                                            | design a no-frills, bare-bones transport protocol                 |
| vacuous          | adj. not expressing or showing intelligent throught                | use a vacuous transport protocol                                  |
| throttle         | v. to prevent sth from succeeding                                  | throttle the transport-layer TCP sender                           |
| excessively      | adv. in a way that is too much                                     | become excessively congested                                      |
| regardless       | adv. despite, not being affected by sth                            | regardless of how long reliable delivery takes                    |
| blast            | v. 爆炸，炸毁，产生巨大噪声，抨击                                  | UDP just blasts away                                              |
| formal           | adj. public or official, in appearance or by name only             | without any formal preliminaries                                  |
| preliminary      | n. 开端活动，初步行动                                              | without any formal preliminaries                                  |
| devote           | v. 奉献给，将...用于                                               |                                                                   |
| induce           | v. 导致，诱使                                                      | the high loss rates induced by the uncontrolled UDP senders       |
| dramatically     | adv. suddenly or obviously                                         | dramatically decrease their rates                                 |
| crowd            | v. 令某人不舒服 by standing to close or watching                   | the crowding out of TCP sessions                                  |
| propose          | v. 提出，建议，提议                                                | many researchers have proposed new mechanisms                     |
| non-trivial      | adj. 非常重要的，棘手的                                            | this is a non-trivial task                                        |
| constraint       | n. 限制，束缚，约束                                                |                                                                   |
| impose           | v. 推行，强制实行，强加于                                          | the constraints imposed by TCP's congestion-control mechanism     |
| explicit         | adj. clear and exact                                               | an explicit length value                                          |
| introduce        | v. to put sth into use, operation, or a place                      | errors have been introduced into the segments                     |
| complement       | n. 补语                                                            |                                                                   |
| redundant        | adj. unnecessary because it is more than is needed                 | be redundant or of little value                                   |
| appropriate      | adj. suitable or right for a particular situation                  | This is appropriate.                                              |
| occur            | v. to exist or be present in, among, etc                           | the problem occurs at the transport layer                         |
| indeed           | adv. really or certainly, often used to emphasize sth              | Indeed, ...                                                       |
| exploit          | v. to use sth in a way that helps you                              | TCP exploits many of the principles 、                            |
| abstraction      | n. 抽象，空泛                                                      | the service abstraction                                           |
| corrupt          | v. （计算机上的信息）被破坏的，有错误的                            | transferred data bits are corrupted                               |
| flip             | v. 使快速翻转；迅速翻动                                            | flip from 0 to 1                                                  |
| vice versa       | adv. 反之亦然                                                      | flipping from 0 to 1, or vice versa                               |
| precisely        | adv. exactly                                                       | This is precisely the service model offered by TCP                |
| more generally   | 换言之，更一般地说                                                 | More generally, the layer ...                                     |
| incrementally    | adv. 渐进地，循序渐进地                                            | we will incrementally develop the protocol                        |
| underlying       | adj. positioned under the surface of sth                           | the underlying channel can corrupt bits                           |
| assumption       | n. sth that you accept as true without question or proof           | one assumption we'll adopt is that ...                            |
| generic          | adj. 一般的，普通的，通用的                                        | the generic term "packet" is perhaps more appropriate here.       |
| unidirectional   | adj. 单向的                                                        | unidirectional data transfer                                      |
| conceptually     | adv. in a way that relates to ideas or principles                  | the case is conceptually no more difficult                        |
| tedious          | adj. boring                                                        | is considerably more tedious to explain                           |
| nonetheless      | adv. despite what has just been said or done                       |                                                                   |
| forth            | adv. (from a place) out or away; 从某时向前                        | packest back and forth                                            |
| flawless         | adj. perfect or without mistakes                                   | a flawless, reliable data transfer protocol                       |
| trivial          | adj. a trivial problem is easy to solve                            | The protocol itself is trivial.                                   |
| finite           | adj. having a limit or end                                         | finite-state machine                                              |
| definition       | adj. a description of the features and limits of sth               | the finite-state machine(FSM) definitions                         |
| diagram          | n. 图，图解，示意图                                                | we'll see more complicated state diagrams.                        |
| explicitly       | adv. in a way that is clear and exact                              | to explicitly denote the lack of an action or event               |
| in practice      | 在实践中                                                           |                                                                   |
| procedure        | n. (计算机的)应用程序                                              | a procedure call by the upper-layer application                   |
| dictate          | v. 口述，口授                                                      | dictate a long message over the phone                             |
| scenario         | n. a description of possible actions or events in the future       | In a typical scenario, ...                                        |
| garbled          | adj. 含糊不清的，引起误解的                                        | hear a garbled sentence                                           |
| fundamentally    | adv. in a basic and important way                                  | Fundamentally, ...                                                |
| capability       | n. the ability to do sth                                           | Fundamentally,three additional capabilities are required          |
| presence         | n. the fact that sth or someone is in a place                      | handle the presence of bit errors                                 |
| explicit         | adj. clear and exact                                               | provide explicit feedback to someone                              |
| indicate         | v. to show, point or make clear in another way                     | a value of 1 cound indicate an ACK                                |
| employ           | v. to use sth                                                      | a data transfer protocol employ error detection.                  |
| leftmost         | 左边                                                               |                                                                   |
| rightmost        | 右边                                                               |                                                                   |
| correspond       | v. to match or be similar or equal                                 |                                                                   |
| fatal            | adj. 致命的                                                        | a fatal flaw                                                      |
| flaw             | n. 错误，缺点，缺陷，瑕疵                                          | a fatal flaw                                                      |
| account for      | 考虑                                                               | account for the possibility                                       |
| proceed          | v. to continue as planned                                          | before proceeding on, you should ...                              |
| innocuous        | adj. completely harmless                                           | is as innocuous as it may seem                                    |
| oversight        | n. 失察，疏忽，疏漏                                                | out slight oversight                                              |
| a priori         | 由因及果的，由一般到具体的，演绎的                                 | a priori                                                          |
| suffice          | v. to be enough                                                    | a 1-bit sequence number will suffice                              |
| modulo           | prep. 【数】对...取模                                              | modulo-2                                                          |
| arithmetic       | n. 算数                                                            | modulo-2 arithmetic                                               |
| mirror images    | 镜像                                                               |                                                                   |
| subtle           | adj. not loud, bright, noticeable, or obvious in any way           | one subtle change between A and B is ...                          |
| not-uncommon     | adj. 并不少见                                                      | a not-uncommon event in today's computer networks                 |
| concern          | n. sth that is important to you, or the fact of being important    | two additional concerns must now be addressed                     |
| forthcoming      | adj. produced, supplied, or given                                  | no reply is forthcoming 没有回复                                  |
| indeed           | adv. really or certainly, 经常用于强调                             | this protocol does indeed work                                    |
| moreover         | adv. 此外，而且，再者                                              | Moreover, the protocol should ...                                 |
| judiciously      | adv. 明断地，明智而审慎地                                          | judiciously choose a time value                                   |
| viewpoint        | n. a point of view 思考的角度，着眼点                              | from the sender's viewpoint                                       |
| panacea          | n. sth that will solve all problems                                | retrasmission is a panacea                                        |
| countdown        | n. the act of counting backwards to zero 倒计时                    | a countdown timer                                                 |
| interrupt        | v. 打断                                                            | interrupt the sender after a given amount of time has expired     |
| expire           | v. 到期，期满，结束                                                | amount of time has expired                                        |
| bracket          | n. 括号                                                            |                                                                   |
| assemble         | v. 集合，聚集，收集                                                | assemble the key elements of a data transfer protocol             |
| crucial          | adj. extremely important or necessary                              | play a crucial and necessary role                                 |
| pipeline         | n. 管道，管线                                                      |                                                                   |
| premature        | adj. 过早的，不成熟的，仓促的                                      | premature timeout                                                 |
| appreciate       | v. to understand a situation and realize that it's important       | to appreciate the performance impact of this behavior             |
| impact           | n. (尤指新事物的) 巨大影响，强大作用                               | the performance impact of this stop-and-wait behavior             |
| approximately    | adv. 大约，大概，左右                                              | The delay is approximately 30 milliseconds                        |
| emerge           | v. to appear by coming out of sth or out from behid sth            | with the last bit of the packet emerging at the receiver          |
| simplicity       | n. the fact that sth is easy to understand or todo                 | assuming for the simplicity                                       |
| utilization      | n. the act of using sth in an effective way                        | the utilization of the sender(or the channel)                     |
| fraction         | n. 分数，极小的部分                                                | the fraction of the time                                          |
| dismal           | adj. very bad                                                      | a rather dismal sender utilization                                |
| fortune          | n. a large amount of money                                         | pay a fortune for a gigabit capacity link                         |
| graphic          | adj. very clear and powerful                                       | this is a graphic example                                         |
| neglect          | v. 疏于照管，忽视，疏忽                                            | neglect lower-layer protocol-processing times                     |
| accentuate       | v. 着重，强调，使明显，使突出                                      | accentuate the poor performance                                   |
| essentially      | adv. 本质上，根本上，基本上                                        | the utilization of the sender is essentially tripled              |
| visualize        | v. 使形象化，使能被看见                                            | packets can be visualized as filling a pipeline                   |
| in-transit       | adj. 在途                                                          | the many in-transit sender-to-receiver packets                    |
| minimally        | adv. in a way that is very small in amount                         | Minimally, the sender will ...                                    |
| awesome          | adj. causing feelings of great admiration, respect, or fear        | an awesome interactive animation                                  |
| interval         | n. a period between two events or times                            | four intervals in the range of sequence numbers                   |
| permissible      | adj. allowed                                                       | the range of permissible sequence numbers for transmitted         |
| impose           | v. 推行，强制实行                                                  | one reason to impose a limit on the sender                        |
| specification    | n. a detailed description                                          | the extended FSM specification                                    |
| invocation       | n. 援引，引用，调用                                                | Invocation from above                                             |
| implicit         | adj. suggested but not communicated directly                       | an implicit indication that the window is full                    |
| indication       | n. a sign that sth exists, is true, or is likely to happen         | an implicit indication that the window is full                    |
| presumably       | adv. used to say what you think is the likely situation            | The uppper layer would presumably have to try again later         |
| semaphore        | n. 旗语                                                            | a semaphore or a flag                                             |
| cumulative       | adj. increasing by one addition after another                      | a cumulative acknowledgment                                       |
| outstanding      | adj. not yet paid, solved, or done                                 | there are no outstanding, unacknowledged packets                  |
| portion          | n. a part or share of sth larger                                   | the data portion of the packet                                    |
| justification    | n. a good reason or explanation for sth                            | there is some justification for doing so.                         |
| cumulative       | adj. 累加的                                                        | the use of cumulative acknowledgments                             |
| garbled          | adj. （话 or 信息）含混不清的，引起误解的                          | might be lost or garbled                                          |
| respectively     | adv. 分别                                                          | pkt4 and pkt5, respectively                                       |
| procedure        | n. 应用程序                                                        | in the form of various procedures                                 |
| simulated        | adj. 模拟的，模仿的                                                | in a simulated, but realistic, network setting                    |
| incorporate      | v. to include sth as part of sth larger                            | the GBN protocol incorporates almost all of the techniques        |
| reiterate        | v. to say sth again, once or several times                         | the reiterated words                                              |
| suspect          | v. to think or believe sth to be true or probable                  | packets that it suspects were received in error                   |
| itemize          | v. 逐个记载，详细列出                                              | itemize the various actions                                       |
| mimic            | v. (为逗乐而)模仿，学...的样子                                     |                                                                   |
| consecutively    | adv. 连贯地，连续地，不间断地                                      | any previously buffered and consecutively numbered packets        |
| identical        | adj. exactly the same, or very similar                             | an identical view of what has been received correctly             |
| coincide         | v. to be the same or similar                                       | the sender and receiver windows will not always coincide          |
| figurative       | adj. 比喻的                                                        | a figurative curtain between the sender and the receiver          |
| curtain          | n. 帘状物，幕状物                                                  | a figurative curtain between the sender and the receiver          |
| manifestation    | n. a sign of sth existing or happening                             | One manifestation of packet reordering                            |
| spontaneously    | adv. 自发的，自然的                                                | spontaneously emit these packets                                  |
| approximately    | adv. 大约，左右，大概                                              | a maximum packet lifetime of approximately three minutes          |
| sequence         | n. 一连串，一系列，顺序，次序                                      | sequence and ackowledgement numbers                               |
| preliminary      | adj. 初步的，起始的，预备的                                        | send some preliminary segments to each other                      |
| parameter        | n. 界定因素，界限，范围，规范                                      | establish the parameters of the ensuing data transfer             |
| ensuing          | adj. happening after sth and because of it                         | establish the parameters of the ensuing data transfer             |
| circuit-switched | 电路交换                                                           | in a circuit-switched network                                     |
| oblivious        | ajd. not conscious of sth, especially what is happening around you | the routers are completely oblivious to TCP connections           |
| inform           | v. to tell someone about particular facts                          |                                                                   |
| suffice          | v. to be enough                                                    | For now it suffices to know that ...                              |
| grab             | v. to take hold of sth or someone suddenly and roughly             | TCP will grab chunks of data from the send buffer                 |
| specification    | n. a detailed description of how sth should be done, made, etc     | the TCP specification                                             |
| be laid back     | 悠闲的                                                             | is laid back about specifying when TCP should send buffered data  |
| specify          | v. to explain or describe sth clearly and exactly                  | about specifying ...                                              |
| propose          | v. 建议，提议，提出                                                | Approaches have also been proposed for discovering the path       |
| entrench         | v. 使根深蒂固                                                      | as it is well entrenched                                          |
| pair             | v. 与 ... 配对                                                     | TCP pairs each chunk of client data with a TCP header             |
| thereby          | adv. as a result of this action                                    | thereby forming TCP segments                                      |
| allocate         | v. 分配，分派，拨给，划拨                                          | no buffers or vairables are allocated to the connection           |
| explicit         | adj. clear and exact                                               | explicit congestion notification                                  |
| urgent           | adj. 紧急的，急迫的                                                | be marked as "urgent"                                             |
| fanciful         | adj. not likely to succeed or happen in the real world             | for a fun and fanciful look at TCP header fields                  |
| implicitly       | adv. in a way that is suggested but not communicated directly      | implicitly number each byte in the data stream                    |
| tricky           | adj. 难办的，难对付的                                              | these are a little trickier than ...                              |
| impost           | v. to officially force a rule, tax to be obeyed or received        | do not impose any rules here                                      |
| bulk             | n. sth or someone that is very large; large size or mass           | the bulk data transfer applications                               |
| vulnerable       | adj. 易受伤的，易受影响（or 攻击）的，脆弱的                       | make Telnet vulnerable to eavesdropping attacks                   |
| eavesdrop        | v. 偷听                                                            | make Telnet vulnerable to eavesdropping attacks                   |
| dual             | adj. with two parts, or combining two things                       | It serves a dual purpose.                                         |
| piggyback        | v. 沾光，搭便车                                                    | is said to be piggybacked                                         |
| sole             | adj. being one only; single                                        | Its sole purpose is to ...                                        |
| onward           | adj. moving forward to a later time or a more distant place        | wait for bytes 80 onward                                          |
| conceptually     | adv. in way that relates to ideas or principles                    | this is conceptually simple                                       |
| recommendation   | n. 推荐；介绍；提议；意见                                          | the current IETF recommendations for managing TCP timers          |
| fluctuate        | v. （尤指持续）波动，起伏不定                                      | the SampleRTT values will fluctuate from segment to segment       |
| fluctuation      | n. 波动，涨落，起伏不定                                            | because of this fluctuation                                       |
| atypical         | adj. different from all others of the same type                    | any given SampleRTT value may be atypical                         |
| exponential      | adj. (增长率)越来越快的，呈几何数(增长)的                          | an exponential weighted moving average                            |
| decay            | v. 腐蚀，使衰败，使衰弱                                            | decay exponentially fast as the updates proceed                   |
| derive           | v. 从...得到                                                       | derive the exponential term in EstimatedRTT                       |
| variation        | n. a change in amount or level                                     | the variation in the SampleRTT are smoothed out                   |
| smooth           | v. to move your hands across sth in order to make it flat          | the variations are smoothed out in the computation                |
| variability      | n. 多变性                                                          | have a measure of the variability of the RTT                      |
| deviate          | v. 脱离，出格，违背规则                                            | how much SampleRTT typically deviates from EstimatedRTT           |
| trigger          | v. to cause sth to start                                           | trigger retransmission of that segment before timeout             |
| premature        | adj. 过早的，不成熟的，仓促的                                      | avoid a premature timeout                                         |
| integrity        | n. 完整性                                                          | guarantee the integrity of the data in the datagrams              |
| assume           | v. to accept sthe to be true without question or proof             | it was conceptually easier to assume that ...                     |
| overhead         | n. 开支                                                            | require considerable overhead                                     |
| ensuing          | adj. happening after sth and because of it                         |
| expiry           | n. 到期，结束                                                      | the expiration interval for this timer                            |
| subtlety         | n. a small but important detail                                    | this highly simplified version has many subtleties                |
| depict           | v. to represent or show sth in a picture or story                  | Figure 3.34 depicts the first scenario                            |
| intact           | adj. complete and in the original state                            | both segments arrive intact at B                                  |
| comprehensive    | adj. complete and including everything that is necessary           | More comprehensive forms of TCP congestion control                |
| persistently     | adv. happening repeatedly or for a long time                       | if the sources continue to retransmit packets persistently        |
| striking         | adj. very unusual or easily noticed，引人注目的                    | there are some striking differences between TCP and Go-Back-N.    |
| respective       | adj. 各自的，分别的，各个的                                        | their respective timeouts                                         |
| generic          | adj. 一般的，普通的，通用的                                        | TCP looks a lot like our generic SR protocol                      |
| categorize       | v. to put people or things into groups with the same features      | is probably best categorized as a hybrid of GBN and SR protocols  |
| associated       | adj. connected                                                     | the associated application process                                |
| instant          | n. an extremely short period of time                               | at the instant the data arrives                                   |
| eliminate        | v. to remove or take away someone or sth                           | aliminate the posibility of sth                                   |
| throttle         | v. to press 某人's throat very tightly so that they cannot breathe | a TCP sender can also be throttled due to congestion              |
| savvy            | n. proctival knowledge and ability                                 | the savvy reader 专业读者                                         |
| informally       | adv. in a way that is not formal or official                       | Informally, ...                                                   |
| distinct         | adj. cleary noticeable; that certainly exists                      | maintain a distinct receive window                                |
| investigate      | v. (尤指为揭开真相)调查，审查                                      | Let's investigate the receive window                              |
| permit           | v. to allow sth                                                    | TCP is not permitted to overflow the allocated buffer             |
| minor            | adj. 较不重要的，次要的，轻微的                                    | There is one minor technical problem                              |
| thrilling        | adj. extremely exciting                                            | this topic may not particularly thrilling                         |
| perceive         | v. 认为，看待，视为                                                | can significantly add to perceived delays                         |
| incredibly       | adv. extremely                                                     | including the incredibly popular SYN flood attact                 |
| exploit          | v. to use sth in a way that helps you                              | exploit vulnerabilities in TCP connection management              |
| vulnerability    | vulnerability                                                      | 脆弱性，脆弱之物                                                  | exploit vulnerability in TCP management |
| randomize        | v. 使...随机化                                                     | randomize the choice of the `client_isn`                          |
| vulnerable       | adj. 易受伤的，易受影响的，脆弱的                                  | make TCP vulnerable to a denial-of-service attack                 |
| grant            | v. to give or allow someone sth, usually in an official way        | this connection-granted segment                                   |
| aspect           | n. one part of a situation, problem, subject, etc                  | several aspects of the TCP three-way handshake                    |
| belayer          | n. 保护着                                                          | a rock climber and a belayer                                      |
| rope             | n. 粗绳，缆绳，绳索                                                | handle the climber's safety rope                                  |
| ascent           | n. the act of climbing or moving upwards                           | before the climber begins ascent                                  |
| issue            | v. to produce or provide sth official                              | the client application process issues a close command             |
| transition       | n. 转变，过渡                                                      | transitions through various TCP states                            |
| explanatory      | adj. 解释的，说明的                                                | The transitions are self-explanatory.                             |
| pathological     | adj. (行为)无法控制的，病态的，非理智的                            | what happens in certain pathological scenarios                    |
| destined         | adj. travelling or being sent to somewhere                         | the segments destined to the host                                 |
| intervening      | adj. 发生于其间的                                                  | the segment was blocked by an intervening firewall                |
| manipulate       | v. 操控，控制，操纵                                                | manipulate TCP connection-management segments                     |
| reclaim          | v. to take back something that was yours                           | reclaim the allocated resources                                   |
| denial           | n. 拒绝                                                            | Denial of Service attack                                          |
| deluge           | n. a very large amount of rain or water                            | this deluge of SYN segments                                       |
| legitimate       | adj. allowed by law; reasonable and acceptable                     | a legitimate user                                                 |
| craft            | v. (运用技巧)制作某物                                              | this carefully crafted initial sequence number                    |
| bogus            | adj. false, not real, or not legal                                 | allocate any resource in response to the original bogus SYN       |
| symptom          | n. (疾病的)症状                                                    | a symptom of network congestion                                   |
| manifest         | v. to show sth clearly, through signs or actions                   | how network congestion is manifested                              |
| utilize          | v. to use sth in an effective way                                  | resources are not fully utilized                                  |
| infinite         | adj. without limits; extremely large or great                      | a router with infinite buffers                                    |
| finite           | adj. having a limit or end                                         | a router with finite buffers                                      |
| overhead         | n. 开支，开销                                                      | ignoring the additional overhead                                  |
| plot             | v. to mark or draw sth on a piece of paper of a map                | Figure 3.44 plots the performance of host A's connection          |
| steady           | adj. 稳步的，持续的，有规律的                                      | a steady-state rate                                               |
| unbounded        | ajd. 极大的，无限的                                                | the average number of quequed packets is unbounded                |
| aggregate        | adj. total                                                         | at an aggregate throughput                                        |
| standpoint       | n. 观点，立场                                                      | it is far from ideal from a delay standpoint                      |
| appreciate       | v. to understand a situation and realize that is important         | to appreciate what is happening here                              |
| compensate       | v. 补偿，赔偿                                                      | in order to compensate for dropped packets                        |
| prematurely      | adv. 过早地，不成熟地，仓促地                                      | the sender may time out prematurely                               |
| versus           | prep. (尤指进行选择时)与...相比                                    | Figure 3.46 shows the throughput versus offered load              |
| asymptotic       | adj. 渐进的，渐近线的                                              | the throughput will have an asymptotic value                      |
| overlapping      | adj. 交叠的，部分重叠的，叠盖的                                    | each over overlapping two-hop paths                               |
| approximately    | adv. 大概，大约，左右                                              | the throughput approximately equals the offered load              |
| imply            | v. to involve sth or make it necessary 必然包含                    | This, in turn, implies that ...                                   |
| evident          | adj. easily seen or understood                                     | be evident                                                        |
| accurately       | adv. 准确地，精确地，正确地                                        | more accurately, equally bad off                                  |
| explicit         | adj. clear and exact                                               | provide no explicit support                                       |
| assistance       | n. help                                                            | provide explicit assistance                                       |
| regard           | v. 考虑，思考，将...认为，看待                                     | provide feedback to hosts regarding network congestion            |
| indication       | n. 表示，表明                                                      | an indication of network congestion                               |
| indicator        | n. 指标                                                            | as an indicator of increased network congestion                   |
| proposal         | n. a suggestion, sometimes a written one                           | a more recent proposal for TCP congestion control                 |
| assist           | v. to help                                                         | network-assisted congestion control                               |
| sophisticated    | adj. 精密的，复杂的，高级的                                        | more sophisticated feedback                                       |
| choke            | n. 阻塞                                                            | a choke packet                                                    |
| essentially      | adv. 本质上，根本上，基本上                                        | essentially saying, "I'm congested!"                              |
| flavor           | n. a particular quality or character                               | look at newer flavors of TCP                                      |
| perceive         | v. 察觉，注意到，意识到                                            | as a function of perceived network congestion                     |
| track            | n. 踪迹，足迹                                                      | keep track of an additional variable                              |
| impose           | v. 推行，强制实行                                                  | impose a constraint on the rate                                   |
| constraint       | n. 限制，约束，束缚                                                | impose a constraint on the rate                                   |
| opposed          | adj. rather that                                                   | as opposed to flow control                                        |
| henceforth       | adv. starting from this time                                       | let us henceforth assume that ...                                 |
| solely           | adv. only and not involving anyone or anything else                | the amount of the unacknowledged data is solely limited by `cwnd` |
| negligible       | adj. too slight or small in amount to be of importance             | loss and packet transmission delays are negligible                |
| excessive        | adj. too much                                                      | when there is excessive congestion, ...                           |
| optimistic       | adj. 乐观的，积极的                                                | consider the more optimistic case                                 |
| hence            | adv. that is the reason or explanation for                         | and hence its transmission rate                                   |
| coordinated      | adj. 协调一致的                                                    | Are TCP senders explicitly coordinated                            |
| interpret        | v. to decide what the intended meaning of sth is                   | is interpreted as an implicit "loss event"                        |
| quadruply        | adv. 四倍                                                          | the quadruply ACKed segment                                       |
| probe            | v. (用工具)探测，探查                                              | Bandwidth probing                                                 |
| onset            | ｎ．(指不愉快的事情)的开始，发作                                   | congestion onset begins                                           |
| asynchronously   | adv. not at the same time or speed                                 | each sender acts asynchronously from other senders                |
| celebrated       | adj. famous for some special quality or ability                    | the details of the celebrated TCP congestion-control algorithm    |
| mandatory        | adj. 强制的，必须履行的，法定的                                    | mandatory components of TCP                                       |
| reckless         | adj. 莽撞的，轻率的，不顾后果的                                    | it might be a bit reckless to keep doubling `cwnd`                |
| surpass          | v. to do or be better than                                         | reach or surpass the value of `ssthresh`                          |
| trace            | v. 找源头                                                          | trace it roots to ...                                             |
| conservative     | adj. 保守的，守旧的                                                | a more conservative approach                                      |
| drastic          | adj. (尤指行动)严厉的，猛烈的，激烈的                              | TCP's behavior should be less drastic                             |
| halve            | v. 使减半，把 ...二等分                                            | TCP halves the value of `cwnd`                                    |
| assist           | v. to help                                                         | network-assisted                                                  |
| variation        | n. 变种，变体，变化了的东西                                        | a number of variations of TCP congestion control protocols        |
| intuition        | n. 直觉，直觉力                                                    |
| capable          | adj. 有能力的，熟练的，能干的                                      | capable of taking action in response to ...                       |
| besides          | prep. in addition to; also                                         |                                                                   |
| Vegas            | n. 一种拥塞控制算法                                                | TCP Vegas                                                         |
| incorporate      | v. to include sth as part of sth larger                            | incorporate mechanisms that ...                                   |
| pervasive        | adj. present or noticeable in every part of a thing or place       | Web traffic is so pervasive                                       |
| fraction         | n. 分数                                                            | it gets a larger fraction of the bandwidth                        |
| pump             | v. to force liquid or gas to move somewhere                        | applications can pump their audio and video into the network      |
| occasionally     | adv. sometimes but not often                                       | occasionally lose packets                                         |
| grinding         | adj. 赤贫的困境                                                    | a grinding halt                                                   |
| halt             | n. 停止，停下，中止                                                | a grinding halt                                                   |
| abundant         | adj. more than enough                                              | have abundant transmission capacity                               |
| elegant          | adj. (想法，计划 or 办法)巧妙的，简捷的，简练的                    | provide an elegant and intuitive explanation                      |
| converge         | v. 会合，聚集，集中                                                | TCP congestion control converges to provide ...                   |
| emanate          | v. 表现，显示                                                      | emanate from the origin                                           |
| intersection     | n. 相交，交点                                                      | the intersection of the equal bandwidth shared line and B         |
| factor           | n. 系数                                                            | decrease their windows by a factor of two.                        |
| vector           | n. 矢量，向量                                                      | a vector starting at B and ending at the origin                   |
| -dimensional     | suffix. 维度，维数                                                 | in the two-dimensional space                                      |
| portion          | n. a part or share of sth larger                                   | obtain very unequal portions of link bandwidth                    |
| identify         | v. to recognize a problem, fact... and to show that it exists      | experience has indentified circumstances                          |
| circumstance     | n. a fact or event that makes a situation the way it is            | experience has indentified circumstances                          |
| evolve           | v. (使)逐步发展，逐步演变，进化                                    | functionality has continued to evolve                             |
| culmination      | n. 高潮                                                            | as a nice culmination of our study                                |
| authentication   | n. 验证，认证                                                      | authentication and encryption                                     |
| pioneer          | v. to be one of the first people to do sth                         | pioneer the notion of ...                                         |
| impact           | v. to have an influence on sth                                     | a lost segment only impacts those stream ...                      |
| timescale        | n. the period of time over which sth happens                       | TCP or UDP update timescales                                      |
| frill            | n. (衣服等的)饰边，褶饰                                            | a no-frills service                                               |
| blissfully       | adv. without knowing any of the unpleasant facts about sth         | is blissfully unaware of TCP's complexity                         |
| imperative       | adj. extremely important or urgent                                 | 拥塞控制 is imperative for the well-being of the network          |
| gridlocked       | adj. 交通严重堵塞的                                                | a network can easily become gridlocked                            |
| strive           | v. (尤指长期 or 不畏艰难地)努力，奋斗，力争                        | strive to give each connection an equal share of the bandwidth    |
| latency          | n. 潜在因素，潜伏                                                  | on latency                                                        |
| intensive        | adj. involving a lot of effort in a short period of time           | it remains an area of intensive research                          |
| wrap up          | to complete sth successfully                                       | to wrap up this chapter                                           |
| partition        | v. 分隔，隔开                                                      | a computer network can be partitioned into the edge and the core  |
