# AT_joi2007ho_e 最軽量のモビール

## 题目描述

有一个由锤子、棒子、绳子组成的结构，最上边的棒子被吊了起来，其他的棒子都被吊在另一个棒上。每个棒子的两边都悬有两根绳子，要么挂锤子，要么挂其他的棒子。

在这个结构中，每个棒子两端各自悬挂的锤子质量之和都要与两端分别到棒子悬挂点的距离成反比（即让棒子保持平衡）。计算时，棒子和绳子的质量忽略不计。

即，若一根棒子的悬挂点到左右两端的距离比为 $a:b$，这根棒子两端所挂的锤子质量之和为 $c:d$，则需要满足 $ad=bc$。

现在，这个结构已经确定下来，唯一没有确定的是结构中各个锤子的质量（但你需要保证它们都是正整数）。请你帮忙求出使该结构平衡需要悬挂的锤子质量之和的最小值。

## 输入格式

第一行输入一个整数 $n$。

第二行到第 $(n+1)$ 行，第 $(i+1)$ 行输入编号为 $i$ 的棒子的信息：四个正整数 $p,q,r,b$，表示棒子的悬挂点到两端点的距离比为 $p:q$，左端悬挂的物体编号为 $r$，右边悬挂的物体编号为 $b$。若需要悬挂锤子，则编号为 $0$，否则编号为棒子的编号。

## 输出格式

一行一个正整数，所需悬挂的锤子质量之和的最小值。**末尾换行。**

### 输入输出样例

#### 输入 #1
```
1
6 9 0 0
```
#### 输出 #1
```
5
```
#### 输入 #2
```
4
3 2 0 4
1 3 0 0
4 4 2 1
2 2 0 0
```

#### 输出 #2
```
40
```

## 说明/提示

样例解释参见[官方文档](https://www2.ioi-jp.org/joi/2006/2007-ho-prob_and_sol/2007-ho.pdf#page=13)。

#### 数据规模与约定

- $1\le n\le 100$；
- 设答案为 $w$，所有 $p,q$ 中最大值为 $L$，则 $wL\lt 2^{31}$。