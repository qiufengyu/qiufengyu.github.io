---
title: Outer Product-based Neural Collaborative Filtering
date: 2018-05-13 16:33:00
tags: [Recommender Systems, NCF, CNN]
categories: [Recommendation] 
---

在 NCF 模型中，引入 CNN 学习特征之间的交互和关联，学习一个更为强大的预测模型。本文指出了目前较为流行的各种 NCF 及其变体模型大多采用特征向量内积、拼接操作的局限性。为此，提出了一种基于外积的新的特征交互模型，通过特征交互操作得到一个特征矩阵，在此基础上应用 CNN 学习到特征中每一维的高阶相互关系。从实验中验证了这一观点，代码开源在 https://github.com/duxy-me/ConvNCF

<!-- more -->

{% pdf /pdf/reading16.pdf 1200px %}