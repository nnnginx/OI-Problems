# AT_k2pc001_h1 紅茶(Tea)

## 题目描述

一天，$\mathrm{kagamiz}$ 一边喝红茶，一边尝试解答如下的问题：

当由两个正整数所组成的正整数组以如下方式排列时，$(m,n)$ 是这个数列里的第几组？

$$(1,1),(2,1),(1,2),(3,1),(2,2),(1,3),(4,1),(3,2),(2,3),(1,4),(5,1),\cdots$$

这个问题对他来说太简单了，所以他更深入地考虑了以下这个问题：

当上述数列中的 $i$ 个组为 $(a_i,b_i)$，第 $j$ 个组为 $(a_j,b_j)$ 时，$(a_i+a_j,b_i+b_j)$ 是这个数列里的第几组？

你的任务就是帮助他解答这个问题。

## 输入格式

输入仅一行，为两个**正**整数 $i,j$。

## 输出格式

输出为一个正整数，表示当上述数列中的第 $i$ 个组为 $(a_i,b_i)$，第 $j$ 个组为 $(a_j,b_j)$ 时，$(a_i+a_j,b_i+b_j)$ 是这个数列里的第几组。

## 说明/提示

对于所有测试数据，$1\leq i,j\leq10^8$，且 $i,j$ 可能相等。