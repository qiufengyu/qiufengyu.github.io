---
title: 基于深度学习的混合协同过滤模型在推荐系统中的应用
date: 2017-09-30 23:00:10
tags: [Recommender Systems, Deep Learning, Collaborative Filtering]
categories: [Recommendation] 
---

协同过滤算法在实际的推荐系统中有着广泛的应用，却也面临着许多问题。给定的用户-物品的打分矩阵通常是十分稀疏的，效果并不理想。因而，现在开始加入更为丰富的辅助信息来缓解数据稀疏和冷启动问题。目前通过学习用户和商品的隐含表示的模型对打分信息和外部信息的利用还不够充分，本文通过深度学习方法，从打分矩阵和辅助信息中，学习了用户和商品的隐含表示，基于此提出一种混合协同过滤模型。通过在 MovieLens 和 BookCrossing 数据集上的实验验证其有效性。

<!-- more -->

{% pdf /pdf/reading2.pdf 1200px %}