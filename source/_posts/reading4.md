---
title: Opinion Recommendation using Neural Memory Model
date: 2017-10-28 23:00:00
tags: [Recommender Systems, Joint Model, Neural Memory Model]
categories: [Recommendation] 
---

本文提出并解决了一个全新的任务：观点推荐，即在当前有用户、物品的历史交互记录中，用户对购买或使用过的服务的 **打分信息** 和与之对应的 **评论** ，现在需要对用户没有买过的商品 **生成可能的评论** 和 **预测一个打分**。这个问题的本质是一个基于多元数据的多任务联合学习（multi-task joint learning），而这正是神经网络模型的强项。本文中，作者使用了一个单层神经网络对用户和商品建模，挖掘他们之间的关联；同时使用了一个深度记忆网络模型来生成具有用户个性特征的商品模型，从而将个性化的打分信息和评论融合在一起，构成一个联合模型。

<!-- more -->

{% pdf /pdf/reading4.pdf 1200px %}
