---
title: Ask the GRU, Multi-task Learning for Deep Text Recommendations
date: 2017-11-25 23:45:00
tags: [Recommender Systems, RNN, Multi-task Learning]
categories: [Recommendation] 
---

从日常生活的需求上来说，学术论文、电影简介、新闻博客等的推荐，都与文本有关。从文本中提取特征，融合到推荐系统中最常用的分解模型中是一种很自然的想法，这也使得那些冷启动的物品具有较好的特征表示。之前的工作主要有使用 **主题模型** 或者是相关文本的 **平均词向量** 来表示物品特征向量，本文提出的方法则是通过深度 RNN （GRU）网络把物品相关的文本映射为特征向量。在学术论文推荐的实验中具有更高的准确率；在冷启动场景下，能够缓解协同过滤模型的数据稀疏问题，也超过了 state-of-the-art。作者认为这得益于多任务学习，因为处理文本的网络的学习过程是 **物品推荐** 和子问题 **分类问题** 的结合。

<!-- more -->

{% pdf /pdf/reading6.pdf 1200px %}
