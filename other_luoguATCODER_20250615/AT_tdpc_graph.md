# AT_tdpc_graph グラフ

## 题目描述

# 图
## 问题描述
有一个由 $ N $ 个结点组成的有向图。当 $ g_{i,j}\ =\ 1 $ 时，从结点 $ i $ 到结点 $ j $ 有一条有向边。最初，所有结点都涂成白色。 Sunuke 君可以执行两次以下操作。
选择一个结点并沿着该结点的有向边访问几个结点。同一个结点可以重复多次。
将所有多次通过的结点涂成黑色。
求出两次操作后，涂成黑色的顶点数的最大值。

## 输入格式

输入以以下格式给出：

 $ N $ 
 
 $ g_{1,1}\ \ \ ...\ \ \ g_{1,N} $ 
 
 $ ...\ \ \ \ \ \ ...\ \ \ \ \ ...$ 
 
 $ g_{N,1}\ \ \ ...\ \ \ g_{N,N} $

## 输出格式

将答案输出为一行。
## 数据限制
- $ 1\ \leq\ N\ \leq\ 300 $
- $ 0\ \leq\ g_{i,j}\ \leq\ 1 $
- $ g_{i,i}\ =\ 0 $