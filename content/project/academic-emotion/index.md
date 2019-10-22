---
title: 在线学习平台中的学业情绪分析服务
summary: 针对mooc平台中大量学生对课程的评论进行学业情绪分析，从而支持平台的迭代优化和教学的优化
tags: 
- 情绪分析
- 文本挖掘
- 在线学习
- AIED
date: "2019-09-13T18:46:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/meflyup
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---
### 简介 
互联网+教育的快速发展，为学生提供了越来越多的在线学习环境。在这样的环境中，学生通常也能够开展学习反馈评论。这些反馈文本中蕴含着丰富的学业情绪信息。针对这些反馈文本的学业情绪分析对教师、学生以及教学管理人员都有重要意义。
传统的学业情绪分析方法主要是通过问卷调查以及使用访谈的方式来分析学生的学业情绪，这样的学业情绪分析方法难以大规模适用于网络学习环境中。近年来，随着以深度学习为代表的人工智能的突破，推动了情绪和情感分析技术的发展，情绪和情感分析在各行业中取得了广泛的应用。
本文总结了学业情绪的相关研究，以及常用的情感分析方法，围绕学业情绪分析问题，提出基于深度学习模型的学业情绪分析方法。首先，本文通过设计分布式爬虫程序，获取互联网中学业情绪反馈文本，并设计学业情绪语料库标注系统，构建学业情绪分析语料库。然后在学业情绪分析语料库的基础上，基于词向量工具word2vec 设计学业情绪词汇分类算法，自动化构建学业情绪分析词典。
再者，结合学业情绪词典和深度学习网络模型构建基于方面的学业情绪识别模型：在学生反馈文本的句子方面分类上，本文采用深度学习模型卷积神经网络（CNN）对学生反馈文本的训练，构建学生反馈文本方面分类模型。在学业情绪分析上，本文对长短期记忆网络（LSTM）进行改造，在LSTM 的基础上融合注意力模型，相对于传统机器学习模型，有效提高了学业情绪识别的准确率。最后，本文基于方面学业情绪分析方法，设计和开发学生反馈文本学业情绪分析服务系统，方便学生、教师以及教学管理人员快速分析文本学业情绪。论文的主要贡献主要有以下三点：

- 构建一套教育领域学业情绪分析资源：通过设计语料标注系统，构建带有学业情绪标注的语料库和自动化构建学业情绪词典。
- 针对学生反馈文本提出方面学业情绪分析方法：改进的深度学习网络模型相较于传统机器学习的方法，提高了方面学业情绪的准确率。
- 针对学生反馈文本开发一套学业情绪分析服务系统。学业情绪分析服务系统的核心为基于文本方面的学业情绪分析方法，不仅能快速识别学生反馈文本中的学业情绪，还能为使用人员提供数据可视化分析服务。

