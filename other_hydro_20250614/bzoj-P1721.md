## 题目描述
Farmer Ron in Colorado is building a ski resort for his cows (though budget constraints dictate construction of just one ski lift). The lift will be constructed as a monorail and will connect a concrete support at the starting location to the support at the ending location via some number of intermediate supports, each of height 0 above its land. A straight-line segment of steel connects every pair of adjacent supports. For obvious reasons, each section of straight steel must lie above the ground at all points. Always frugal, FR wants to minimize the number of supports that he must build. He has surveyed the $n \ (2  \leq  n  \leq  5\times 10^3)$ equal-sized plots of land the lift will traverse and recorded the integral height $h \ (0  \leq  h  \leq  10^9)$ of each plot. Safety regulations require FR to build adjacent supports no more than $k \ (1  \leq  k  \leq  n - 1)$ units apart. The steel between each pair of supports is rigid and forms a straight line from one support to the next. Help FR compute the smallest number of supports required such that: each segment of steel lies entirely above (or just tangent to) each piece of ground, no two consecutive supports are more than $k$ units apart horizontally, and a support resides both on the first plot of land and on the last plot of land.

科罗拉州的罗恩打算为他的奶牛们建造一个滑雪场，虽然需要的设施仅仅是一部缆车。建造一部缆车，需要从山脚到山顶立若干根柱子，并用钢丝连结它们。你可以认为相对于地面，柱子的高度可以忽略不计。每相邻两根柱子间都有钢丝直接相连。显然，所有钢丝的任何一段都不能在地面之下。为了节省建造的费用，罗恩希望在工程中修建尽可能少的柱子。他在准备修建缆车的山坡上迭定了 $n$ 个两两之间水平距离相等的点，并且测量了每个点的高度 $h$。并且，按照国家安全标准，相邻两根柱子间的距离不能超过 $k$ 个单位长度。柱子间的钢丝都是笔直的. 罗恩希望你帮他计算一下，在满足下列条件的情况下，他至少要修建多少根柱子：首先，所有的柱子都必须修建在他所选定的点上，且每一段钢丝都必须高于地面或者正好跟地面相切。相邻两根柱子的距离不大于 $k$ 个单位长度。当然，在第一个点与最后一个点上一定都要修建柱子。
## 输入格式

第 $1$ 行：两个整数 $n$ 和 $k$，用空格隔开。

第 $2$ 到 $n+1$ 行：每行包括一个正整数，第 $i+1$ 行的数描述了第 $i$ 个点的高度。

## 输出格式

输出一个整数，即罗恩最少需要修建的柱子的数目。

```inout1
13 4
0
1
0
2
4
6
8
6
8
8
9
11
12
```
```output1
5
```
## 样例说明

罗恩最少要修建 $5$ 根柱子（分别在第 $1,5,7,9,13$ 个山坡上的点）。钢丝在 $1-5,5-7,7-9$ 以及 $12-13$ 这 $4$ 段上与地面相切。
## 数据规模与约定
对于 $100\%$ 的数据，$2 \leq n \leq 5\times 10^3$，$0 \leq h \leq 10^9$，$1 \leq k \leq n-1$。
## 题目来源
Gold