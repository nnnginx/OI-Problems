## 题目描述

轮状病毒有很多变种，所有轮状病毒的变种都是从一个轮状基产生的。一个 $n$ 轮状基由圆环上 $n$ 个不同的基原子
和圆心处一个核原子构成的，$2$ 个原子之间的边表示这 $2$ 个原子之间的信息通道。如下图所示：

![](./552/file/pic2.png)

$n$ 轮状病毒的产生规律是在一个 $n$ 轮状基中删去若干条边，使得各原子之间有唯一的信息通道，例如共有 $16$ 个不同的 $3$ 轮状病毒，如下图所示：

![](./552/file/pic1.png)

现给定 $n$，编程计算有多少个不同的 $n$ 轮状病毒。

## 输入格式

第一行有一个正整数 $n$。

## 输出格式

计算出的不同的 $n$ 轮状病毒数输出。

```input1
3
```

```output1
16
```

## 数据范围

对于 $100\%$ 的数据，$1 \le n \le100$。