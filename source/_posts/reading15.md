---
title: NAIS - Neural Attentive Item Similarity Model for Recommendation
date: 2018-04-29 22:22:00
tags: [Recommender Systems, Attention, Similarity]
categories: [Recommendation] 
---

基于物品的协同过滤方法，结合 Attention。基于用户可能会喜欢相似、相关历史物品的假设，从而具有更好的解释性，在实时推荐的情境下，也可以进行高效地推荐。这种模型的关键在于如何衡量物品的相似度，较为传统的有余弦距离、皮尔逊相关系数，但是这种通用的方法并不一定适合推荐系统的场景。为此，一些工作会设计一个和推荐系统相关的损失函数，从用户、物品的角度来学习物品的隐藏表示。这些方法通常是线性的，所以本文提出一种基于注意力网络的非线性方法，能够获取到每个历史物品对用户当前喜好预测的重要性。NAIS 模型较 FISM（曾经的 state-of-the-art）有了性能上的提升，只是增加了一部分 attention 网络的参数规模。此外，NAIS 开创了神经网络对基于物品的协同过滤算法的时代，具有启发意义。

<!-- more -->

{% pdf /pdf/reading15.pdf 1200px %}



