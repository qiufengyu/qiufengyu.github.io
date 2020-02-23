---
title: RNNs in Sequential Recommender Systems
date: 2017-12-09 15:00:00
tags: [Recommender Systems, RNN, Sequential]
categories: [Recommendation] 
---

在 ICLR-2018 公开的投稿论文中，发现了一篇[用 RNN 做 Session-based Recommendation](https://openreview.net/forum?id=ryCM8zWRb) 的文章，在目前盲审阶段得到了 6、4、8 的分数，据我推测很可能是 ICLR-2016 中提出 Session-based Recommendation 的同一作者团队在之前模型上提出的改进。在这里，我更关注了该文的参考文献，了解 RNN 在推荐系统领域的应用历程。先是一篇短文，A Dynamic Recurrent Model for Next Basket Recommendation，发表于 SIGIR-16。之后是发表在 RecSys-2017 的文章，Sequential User-based Recurrent Neural Network Recommendations，利用 RNN 对用户建模进行推荐。

从用户和商品之间的交互信息中，我们可以提取出用户的喜好特征，传统模型得到的是一个全局性（general interests）的信息。如果按时间顺序考虑用户的交互过程，利用 Markov Chain 的假设，得到用户的一个局部特征。将全局和具有时间动态性的局部特征结合起来，就可以进行更精准的推荐。

<!-- more -->

{% pdf /pdf/reading7.pdf 1200px %}
