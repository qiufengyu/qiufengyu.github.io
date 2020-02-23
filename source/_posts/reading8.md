---
title: Recurrent Recommender Networks
date: 2017-12-24 01:19:00
tags: [Recommender Systems, RNN]
categories: [Recommendation] 
---

推荐系统通常认为用户信息、商品的属性是静态的，而现实中存在时间动态性。当用户的喜好发生改变或者受到外部环境因素的影响，此时的特征都存在一定的偏差。本文提出的 **循环推荐网络** （Recurrent Recommender Networks，RRN）能够预测用户 **将来** 的行为轨迹，即通过 LSTM 刻画除了传统低阶矩阵分解的特征，更突出了动态的变化特征。这一模型是十分紧凑（参数规模更小）的，因为通过网络学习的目的不是隐藏状态，而只是状态转移函数。（<u>注：目前还不能理解，请看后文。</u>）

<!-- more -->

{% pdf /pdf/reading8.pdf 1200px %}