---
title: 'Blog Post number 1'
date: 2021-10-20
permalink: /posts/2012/08/sgd and adam/
tags:
  - 优化器
  - SGD
  - ADAM
---

深度学习二分类问题，选择使用已经训练好的resnet。

![在这里插入图片描述](../picture/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBA5YmN56iL5Ly86ZSm6J2I6J2I,size_20,color_FFFFFF,t_70,g_se,x_16.png)
在用Adam微调模型时，发现性能很差。
![在这里插入图片描述](../picture/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBA5YmN56iL5Ly86ZSm6J2I6J2I,size_20,color_FFFFFF,t_70,g_se,x_16-1720630100860-1.png)
在用SGD（随机梯度下降）时，效果很好。

原因在于是二分类问题，数据的分布好计算，更适合SGD，而对于Adam更适合计算复杂分布的数据