## 题目描述

John 养了一只叫 Joseph 的奶牛。一次她去放牛，来到一个非常长的一片地，长度为 $l$，上面有 $n$ 块地方长了茂盛的草。我们可以认为草地是一个数轴上的一些点。Joseph 看到这些草非常兴奋，它想把它们全部吃光。于是它开始左右行走，吃草。John 和 Joseph 开始的时候站在 $p$ 位置。Joseph 的移动速度是一个单位时间一个单位距离。不幸的是，草如果长时间不吃，就会腐败。我们定义一堆草的腐败值是从 Joseph 开始吃草到吃到这堆草的总时间。Joseph 可不想吃太腐败的草，它请 John 帮它安排一个路线，使得它吃完所有的草后，总腐败值最小。John 的数学很烂，她不知道该怎样做，你能帮她么？

## 输入格式

* Line $1$: Two space-separated integers: $n$ and $l$.
* Lines $2\dots n+1$: Each line contains a single integer giving the position $p$ of a clump.

## 输出格式

* Line $1$: A single integer: the minimum total staleness Bessie can achieve while eating all the clumps.

```input1
4 10
1
9
11
19
```
```output1
44
```

## 样例解释

INPUT DETAILS:

Four clumps: at $1,9,11$, and $19$. Bessie starts at location $10$.

OUTPUT DETAILS:

Bessie can follow this route:  

* start at position $10$ at time $0$.
* move to position $9$, arriving at time $1$.
* move to position $11$, arriving at time $3$.
* move to position $19$, arriving at time $11$.
* move to position $1$, arriving at time $29$.

giving her a total staleness of $1+3+11+29 = 44$. There are other routes with the same total staleness, but no route with a smaller one.

## 数据范围

对于所有数据，$n\le 10^3$，$1 \le  p \le  10^6$。
