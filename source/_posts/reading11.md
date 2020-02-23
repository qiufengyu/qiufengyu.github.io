---
title: Leverage Long and Short-term Information in Content-aware Movie Recommendation
date: 2018-02-10 22:50:00
tags: [Recommender Systems, RNN]
categories: [Recommendation] 
---

由相关微信公众号推荐，也有一个[知乎专栏](https://zhuanlan.zhihu.com/p/32425103)，[arxiv 链接](https://arxiv.org/abs/1712.09059)。

本文在传统利用 RNN 解决 session-based recommendation 问题上，引入了一些用户和物品的静态信息，此为看点一。运用对抗网络训练模型，融合强化学习的思想，此为看点二。看点三略显平常，融合一些辅助信息缓解冷启动问题。

电影推荐系统，根据用户的口味生成一个候选推荐列表。目前主要有两种建模的立足点：长期静态模型和短期动态模型。前者从用户与电影的交互信息抽取出近似认为不会变化的用户和电影的特征，后者则是将用户兴趣和电影的信息在短期内进行一系列的调整与改变。本文提出了 LSIC 模型，使用对抗训练的方式，从数据中提取长、短期的特征：由生成器，结合强化学习的相关做法，根据用户的消费序列生成下一个可能的候选电影；而判别器负责区分生成器给出的结果和真实结果。此外，关于电影的一些外部信息也被引入，可以缓解冷启动问题。

<!-- more -->

{% pdf /pdf/reading11.pdf 1200px %}