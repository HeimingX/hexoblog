---
title: python中RuntimeWarning overflow encountered in exp
date: 2016-04-30 22:50:12
categories: Python
tag: python
description: 如题~
---

python中numpy.exp()和scipy.exp()函数参数取一个很大的值（2500）时，会出现上面的溢出问题，在[stackoverflow](http://stackoverflow.com/questions/9559346/deal-with-overflow-in-exp-using-numpy)上提供了两个解决方案：1. 安装一个bigfloat库 2. 用numpy.seterr来控制异常的抛出。目前采用了第一种方法解决。

# Bigfloat下载
[Unofficial Windows Binaries for Python Extension Packages](http://www.lfd.uci.edu/~gohlke/pythonlibs/#bigfloat)

# windows上whl文件安装
[windows下安装easy_install, pip 及whl文件安装方法](http://www.cnblogs.com/wu-wenmin/p/4250330.html)
