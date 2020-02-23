---
title: Joint Deep Modeling of Users and Items Using Reviews for Recommendation
date: 2018-06-10 16:37:00
tags: [Recommender Systems, Deep Learning]
categories: [Recommendation] 
---

Github 前阵子出了个 Repository Recommendation 的功能，偶然看到这篇文章及其扩展的一个开源实现，本周阅读这篇基础文章，下一阶段再精读改进模型的文章。

用户的评论中通常蕴含大量有用的信息，而这些信息在推荐系统中的使用程度很低，但却是一定程度上能够缓解冷启动问题，提升推荐性能的一部分。本文提出了一个深度模型，从评论中联合学习物品的属性和用户的行为。本文提出的 DeepCoNN 模型，有两个平行的神经网络，其中一个对于用户所写的评论分别学习用户的行为数据，另一个则是对物品的所有评论中习得物品的属性信息，最后通过一个“共享层”把这两部分网络特征融合在一起。从而，用户和物品的各自的表示能够以一种类似于分解模型的方式交互。在多个实验数据中，DeepCoNN 均打败了其他方法和模型。

<!-- more -->

{% pdf /pdf/reading18.pdf 1200px %}