## 题目描述

Farmer John has built a new long barn, with $n \ (2  \leq  n  \leq  10^5)$ stalls. The stalls are located along a straight line at positions $x_1,\dots ,x_n \ (0  \leq  x_i  \leq  10^9)$. His $c \ (2  \leq  c  \leq  n)$ cows don't like this barn layout and become aggressive towards each other once put into a stall. To prevent the cows from hurting each other, FJ want to assign the cows to the stalls, such that the minimum distance between any two of them is as large as possible. What is the largest minimum distance?

农夫 John 建造了一座很长的畜栏，它包括 $n$ 个隔间，这些小隔间依次编号为 $x_1,\dots ,x_n$。但是，John 的 $c$ 头牛们并不喜欢这种布局，而且几头牛放在一个隔间里，他们就要发生争斗。为了不让牛互相伤害。John 决定自己给牛分配隔间，使任意两头牛之间的最小距离尽可能的大，那么，这个最大的最小距离是什么呢？

## 输入格式

* Line $1$: Two space-separated integers: $n$ and $c$.
* Lines $2\dots n+1$: Line $i+1$ contains an integer stall location,$x_i$.

* 第一行：空格分隔的两个整数 $n$ 和 $c$。
* 第二行至第 $n+1$ 行：$i+1$ 行指出了 $x_i$ 的位置。

## 输出格式

* Line $1$: One integer：the largest minimum distance.

* 第一行：一个整数，最大的最小值。

```input1
5 3
1
2
8
4
9
```

```output1
3
```

## 样例说明

把牛放在 $1$，$4$，$8$ 这样最小距离是 $3$。

## 数据规模与约定
对于 $100\%$ 的数据，$2 \le n \le 10^5$，$0 \le x_i \le 10^9$，$2 \le c \le n$。
## 题目来源

Gold