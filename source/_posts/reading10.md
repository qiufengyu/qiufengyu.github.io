---
title: ATRank, An Attention-based User Behavior Modeling Framework for Recommendation
date: 2018-01-21 21:00:00
tags: [Recommender Systems, User Modeling]
categories: [Recommendation] 
---

在推荐系统或是社交网络中的用户建模中，可以通过他一系列的行为事件来建模。这些行为可以通过特征表示学习得到，把这些不同事件聚合起来，就能得到一个用户的表示。在人类有限的本能中，尚不明确这些融合方式的机理，因此很难全面地抓住用户的个性化特征，即这些特征向量之间的运算没有直观的解释。近期的研究中，开始用 RNN 模型来解决序列化推荐和预测，可仍然局限于这些有限的数据中，每一个事件都被通俗地编码成一个特征，我们认为只是简单的信息加和，没有利用信息之间的更新、推理等更为丰富的特征处理。例如，在当前事件的预测上，可能会失去和本次行为十分相关的历史行为的关系，而引入与当前事件没什么关系的其他噪音事件信息。

本文提出一种基于 Attention 机制的 ATRank 模型。用户的异构行为信息被映射到多个隐式语义空间中，由 self-attention，选出对当前事件的决策最具有影响的一些行为信息，从而在 Attention 时得以区别对待。ATRank 在实验中显示，训练更快，效果更好。此外，ATRank 还能对行为的类别进行预测，也比一些相关的优化模型表现好。

<!-- more -->

{% pdf /pdf/reading10.pdf 1200px %}