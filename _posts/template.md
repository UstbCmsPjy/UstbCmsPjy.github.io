---
layout: post
title: template page
categories: [cate1, cate2]
description: some word here
keywords: keyword1, keyword2
---

# Openphase

OpenPhase的源码真的是挺难读的，它是一整套完全的很成熟的求解相场模型的框架，其模块化完成度很高(尤其设计的数据结构面面俱到，号称能处理所有类型的数据)，所以用它来解方程时写的代码很少，但带来一个问题是你必须先读懂它：高度集成的代码让初学者“一进去就出不来”(从而迷失在各个类中)或“压根进不去”(一行代码就完成一个大功能，根本不知道怎么入手)。

## ProjectInput.opi文件

此文件中的参数是通过Settings类的ReadInput函数读入。
针对本例，读入的重要参数有：

- 晶粒个数是2: Ngrans=2
- 相的个数是2: Nphses=2
- 格点数目为：Nx=64, Ny=1, Nz=64
- 网格间距为：dx=1.0
- 界面宽度占格点的数目为：iWidth=0
- 系统实际温度：T=500
- OpenMP线程个数：nOMP=2

