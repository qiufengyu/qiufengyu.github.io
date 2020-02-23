---
title: TransNets - Learning to Transform for Recommendation
date: 2018-06-24 15:04:00
tags: [Recommender Systems, Deep Learning]
categories: [Recommendation] 
---

本文是 DeepCoNN 模型的改进。深度学习及相关模型在推荐系统任务中，比传统方法都要更优秀。目前推荐系统中，会融合很多的外部信息，如用户评论等，而 NLP 相关技术的发展更是受到了神经网络的大增益，DeepCoNN 模型借助神经网络从评论文本中获得用户、物品的表示。但是 DeepCoNN 模型在预测用户给目标商品的打分时，更多的是利用了用户的评论信息，本质上是一个根据评论文本预测打分的“情感分类”的问题，而不是推荐问题。本文提出的 TransNets 模型，扩展了 DeepCoNN，引入了一个额外的隐藏层来表示用户、物品，使之与训练集的评论文本类似，从而获得更为出色的推荐性能。

<!-- more -->

{% pdf /pdf/reading19.pdf 1200px %}