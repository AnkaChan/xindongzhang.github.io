---
layout: post
title: python深度学习框架
tags: python deep-learning
categories: 机器学习
---

## 1.基于theano
Theano 是一个python类库。他基于表示矩阵向量的numpy和包含大量数学功能的scipy，提供一种符号表示的数学公式。符号表示的数学公式的主要不同就是， 在建立公式的时候，你不需要知道公式里的自变量的值是什么。下面是一些基于theano类库的深度学习框架，其提供了更高级的访问，你不需要去了解其很多实现的细节：

* [keras](http://keras.io/) : 高度模块化的神经网络函数库。
* [Lasagne](https://github.com/Lasagne/Lasagne) : 基于theano的轻量级神经网络函数库。
* [Blocks](https://github.com/mila-udem/blocks) : 基于theano的神经网络函数库。
* [Pylearn2](https://github.com/lisa-lab/pylearn2) : 通用的机器学习函数库，其中包含一些深度学习的算法实现。

## 2.不基于theano
下面的一些深度学习框架没有基于theano：

* [libdeep-python](https://github.com/bashrc/libdeep-python) : 基于[libdeep](https://github.com/bashrc/libdeep)的python接口，可以进行相关深度学习算法的实现。
* [cxxnet](https://github.com/dmlc/cxxnet) : 百度的开源项目，具有“快速，简洁，分布式”计算能力，有python的接口可以进行调用。
* [caffe](http://caffe.berkeleyvision.org/) : 伯克利的开源项目，有python和matlab的调用接口。
* [neon](https://github.com/NervanaSystems/neon) : 用python实现的深度学习框架。
* [nolearn](https://github.com/dnouri/nolearn) : 对现有的几个深度学习框架提供了访问接口。


