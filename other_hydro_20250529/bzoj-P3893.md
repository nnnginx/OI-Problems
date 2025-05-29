[](/d/bzoj/p/3826)

## 题目描述

The cows are out exercising their hooves again! There are $n$ cows jogging on an infinitely-long single-lane track. Each cow starts at a distinct position on the track, and some cows jog at different speeds. With only one lane in the track, cows cannot pass each other. When a faster cow catches up to another cow, she has to slow down to avoid running into the other cow, becoming part of the same running group. The cows will run for $T$ minutes. Please help Farmer John determine how many groups will be left at this time. Two cows should be considered part of the same group if they are at the same position at the end of $T$ minutes.

**翻译：**

在一条无限长的跑道上有 $n$ 头牛，每头牛有自己的初始位置及奔跑的速度。牛之间不能互相穿透。当一只牛追上另一只牛时，它不得不慢下来，成为一个群体。求 $T$ 分钟后一共有几个群体。 

## 输入格式

The first line of input contains the two integers $n$ and $T$. The following $n$ lines each contain the initial position and speed of a single cow. Position is a nonnegative integer and speed is a positive integer; both numbers are at most $1$ billion. All cows start at distinct positions, and these will be given in increasing order in the input.

第一行两个整数 $n,T$，如题所示。

接下来 $n$ 行每行包含一个非负整数 $x_i$ 和一个正整数 $v_i$，表示第 $i$ 头牛的初始位置和速度。

保证开始时牛站在不同的位置上，并且输入按照位置递增的顺序排列。

## 输出格式

A single integer indicating how many groups remain after $T$ minutes.

输出一个整数，即 $T$ 分钟后有几个群体。

```input1
5 3
0 1
1 2
2 3
3 2
6 1
```

```output1
3
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n \le 10^5$，$1 \le T \le 10^9$，$0\le x_i \le 10^8$，$1\le v_i\le 10^8$。

## 题目来源

Silver