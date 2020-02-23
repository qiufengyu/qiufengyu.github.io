---
title: Session-based Recommendations with Recurrent Neural Networks
date: 2017-11-11 23:00:00
tags: [Recommender Systems, RNN]
categories: [Recommendation] 
---

本文将 RNN 应用在推荐系统任务中，解决实际应用的传统推荐算法过度依赖用户做出的最后一个行为（点击、打分）数据，而在之前与之相关的行为数据则明显利用不足，经典的矩阵分解算法就捉襟见肘了。目前，通常采用折中的方法，即基于最近邻，推荐最相似的物品。本文认为，对于用户所有行为（称为一个 session ）进行建模，可以提高推荐的准确率。根据实际情况，对传统 RNN 进行改进，使之适合任务，从实验中验证了任务导向的模型设计的作用。

<!-- more -->

{% pdf /pdf/reading5.pdf 1200px %}
