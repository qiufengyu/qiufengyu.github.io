---
title: Embedding-based News Recommendation for Millions of Users
date: 2018-05-27 23:49:00
tags: [Recommender Systems, Embedding, News]
categories: [Recommendation] 
---

为了做好新闻推荐这件事情，就需要了解新闻的内容和用户喜好之间的关系。协同过滤等基于 ID 的算法局限性在于新闻这一类的对象，保质期很短，难以实时地更新。若利用新闻文本的内容，则是一种类似信息检索的方法，就需要为特定用户从阅读记录中生成个性化的 query。从这两种方法出发，本文提出了一种 3 层结构的基于 embedding 表示方法的新闻推荐方法：为新闻生成表示、为用户生成表示以及生成推荐新闻列表。这一框架在 Yahoo 日本新闻平台上进行了离线和在线测试，在推荐性能和推荐的效率上都取得了令人满意的结果。

<!-- more -->

{% pdf /pdf/reading17.pdf 1200px %}