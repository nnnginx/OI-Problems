# AT_relay_h 早起き

## 题目描述

高桥君最近几天的生活被记录为一个长度为 $2N$ 的数列：

- $a_1, b_1, a_2, b_2, \ldots, a_N, b_N$

这个数列表示从某个时刻 $T$ 开始，高桥君的生活模式是这样的：

- 他先睡了 $a_1$ 秒，
- 然后醒来 $b_1$ 秒，
- 然后继续睡 $a_2$ 秒，
- 以此类推……
- 最终他睡了 $a_N$ 秒，
- 然后再醒来 $b_N$ 秒。

在这段记录中，高桥君总共醒来 $N$ 次。

高桥君想知道在这 $N$ 次醒来中，他有多少次是“早起”的。

在这里，“早起”定义为在凌晨 $4$ 点到早上 $7$ 点之间醒来。如果醒来时间刚好是凌晨 $4$ 点或早上 $7$ 点，同样算作早起。

只要在同一时间段里醒来多次，每次都算作单独的早起。

然而，高桥君已经忘记了初始时刻 $T$。

请计算出，在最多的情况下，高桥君在这 $N$ 次醒来中的早起次数。

一天有 $86400$ 秒，而凌晨 $4$ 点到早上 $7$ 点之间的时间段一共有 $10800$ 秒。

## 输入格式

输入通过标准输入，格式如下：

> $N$ $a_1$ $b_1$ $a_2$ $b_2$ $\ldots$ $a_N$ $b_N$

## 输出格式

输出最多可能的早起次数。

## 输入输出样例 #1

### 输入 #1

```
3
28800 57600
28800 57600
57600 28800
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
10
28800 57600
4800 9600
6000 1200
600 600
300 600
5400 600
6000 5760
6760 2880
6000 12000
9000 600
```

### 输出 #2

```
5
```

## 说明/提示

- $1 \leq N \leq 10^5$
- $1 \leq a_i, b_i \leq 10^5$
- $a_i, b_i$ 均为整数。

 **本翻译由 AI 自动生成**