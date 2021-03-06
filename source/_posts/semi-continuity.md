﻿---
title: 半连续
date: 2016-04-29 15:24:45
categories: [Mathematics]
tag: [mathematics]
description: 关于半连续的一些概念及性质
---

# 概念
半连续（semi-continuity）是对函数连续性的一种描述，与连续相比更弱一些。主要有两种半连续：上半连续（upper semi-continuous）和下半连续（lower semi-continuous）。

# 定义

**上半连续**
$$\lim \sup_{x\to x_0} f(x) \leq f(x_0)$$
这里的$\lim \sup$表示极限上界，就是说函数$f(x)$在趋向于$x_0$时，函数的极限上界要小于等于$f(x_0)$,可以借助下图来理解。

![upper semi-continuity](https://upload.wikimedia.org/wikipedia/commons/c/c0/Upper_semi.svg)
可以看出，由于函数是分段的，从左侧趋向于$x_0$时（取不到），必定会小于$f(x_0)$，而从右侧趋向于$x_0$时是可以取到$f(x_0)$的，那么等号成立。


**下半连续**
$$\lim\inf_{x\to x_0} f(x) \geq f(x_0)$$
同理，这边的$\lim \inf$表示极限下界。

![lower semi-continuity](https://upload.wikimedia.org/wikipedia/commons/b/b0/Lower_semi.svg)
这里的分析与上半连续一致，不赘述了。

# 性质
1. 一个函数是连续的当且仅当他是上半连续的和下半连续的
2. 两个上半连续的实值函数相加还是上半连续的；如果两个函数都是非负的，那么两者的乘积为上半连续
3. 一个上半连续的函数乘以一个负数，变为下半连续
4. 如果$C$是一个紧凑的空间（比如一个闭合的，有界的空间），且$f : C \to [-\infty, \infty)$是上半连续的，那函数$f$在$C$上必定取到最大值；
同理，对于在$f : C \to (-\infty, \infty]$是下半连续的，那么函数在$C$上必定能取得最小值
5. 假设$f_i : X \to [-\infty, \infty]$ 是一个下半连续函数，且每个 $ f_i $ 的定义域 $ I $ 都是非空的，那么定义函数 $f$ （追点取极值）
	
	$$f(x) = \sup_{i\in I} f_i(x), x\in X$$
	那么函数$f$也是下半连续的。
6. 一个函数$f : \mathbf R^n \to \mathbf R$是下半连续的当且仅当它的上境界是闭合的

# reference
1. [wiki semi-continuity](https://en.wikipedia.org/wiki/Semi-continuity)
