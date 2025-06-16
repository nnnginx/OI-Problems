## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc002/tasks/agc002_b



## 题目大意
# [AGC002B] Box and Ball

## 题目描述

有 $n$ 个盒子。起初每个盒子里有 $1$ 个球， $1$ 号盒子里的球是红色的，其余都是白色的。

现在给定 $m$ 个操作，每次给出二元组 $(x_i,y_i)$ 表示从 $x_i$ 中随机拿出一个球放进 $y_i$。

求在操作结束后有多少个盒子里**可能**装着红色小球。

——翻译 By 冬天的雨

## 输入格式

第一行两个数，$n,m~(2\leqslant n\leqslant 10^5,1\leqslant m\leqslant 10^5)$

然后 $m$ 行，每行两个数 $x_i,y_i$，保证 $1\leqslant x_i,y_i\leqslant n$ 且 $x_i\neq y_i$

## 输出格式

一个数表示所求答案。

