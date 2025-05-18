## 题目描述
Farmer John has recently been experimenting with cultivating different types of grass on his farm, realizing that different types of cows like different types of grass. However, he must be careful to ensure that different types of grass are planted sufficiently far away from each-other, in order to prevent them from being inextricably mixed.


FJ's farm consists of $N$ fields ($1 \leq N \leq 200,000$), where $M$ pairs of  fields are connected by bi-directional pathways ($1 \leq M \leq 200,000$).  Using these pathways, it is possible to walk from any field to any other field. Each pathway has an integer length in the range $1 \ldots 1,000,000$. Any pair of fields will be linked by at most one direct pathway.


In each field, FJ initially plants one of $K$ types of grass ($1 \leq K \leq N$). Over time, however, he might decide to switch the grass in some field to a different type. He calls this an "update"  peration. He might perform several updates over the course of time, which are all cumulative in nature.


After each update, FJ would like to know the length of the shortest path between two fields having different grass types. That is, among all pairs of fields having different grass types, he wants to know which two are closest. Ideally,

this number is large, so he can prevent grass of one type from mixing with grass of another type. It is guaranteed that the farm will always have at least two fields with different grass types.


In 30 percent of the input cases, each field will be directly connected to at most 10 pathways.




## 输入格式
The first line of input contains four integers, $N$, $M$, $K$, and $Q$, where $Q$ is the number of updates ($1 \leq Q \leq 200,000$).

The next $M$ lines describe the paths; each one contains three integers $A$, $B$, and $L$, indicating a path from field $A$ to field $B$ (both integers in the range $1 \ldots N$) of length $L$.

The next line indicates the initial type of grass growing in each field ($N$ integers in the range $1 \ldots K$).

Finally, the last $Q$ lines each describe an update, specified by two integers $A$ and $B$, where the grass in field $A$ is to be updated to type $B$.


## 输出格式
For each update, print the length of the shortest path between two fields with different types of grass, after the update is applied.


## 题目大意
### 题目描述

Farmer John 最近在他的农场尝试种植不同类型的草，发现不同类型的奶牛喜欢不同类型的草。然而，他必须小心确保不同类型的草种植得足够远，以防止它们不可分割地混合在一起。

FJ 的农场由 $N$ 块田地组成（$1 \leq N \leq 200,000$），其中 $M$ 对田地通过双向路径连接（$1 \leq M \leq 200,000$）。使用这些路径，可以从任何田地走到任何其他田地。每条路径的长度是一个在 $1 \ldots 1,000,000$ 范围内的整数。任何一对田地之间最多只有一条直接路径。

在每块田地中，FJ 最初种植了 $K$ 种草中的一种（$1 \leq K \leq N$）。然而，随着时间的推移，他可能会决定将某块田地的草更换为另一种类型。他称这种操作为“更新”操作。他可能会在一段时间内执行多次更新，这些更新都是累积性质的。

每次更新后，FJ 想知道种植不同草类型的两块田地之间的最短路径长度。也就是说，在所有种植不同草类型的田地对中，他希望知道哪两块田地最接近。理想情况下，这个数字应该较大，以便他可以防止一种类型的草与另一种类型的草混合。保证农场中始终至少有两块田地种植不同的草类型。

在 30% 的输入案例中，每块田地最多直接连接 10 条路径。

### 输入格式

输入的第一行包含四个整数 $N$、$M$、$K$ 和 $Q$，其中 $Q$ 是更新的次数（$1 \leq Q \leq 200,000$）。

接下来的 $M$ 行描述路径；每行包含三个整数 $A$、$B$ 和 $L$，表示从田地 $A$ 到田地 $B$（两者都是 $1 \ldots N$ 范围内的整数）的长度为 $L$ 的路径。

接下来的一行表示每块田地最初种植的草类型（$N$ 个 $1 \ldots K$ 范围内的整数）。

最后，最后的 $Q$ 行每行描述一个更新，由两个整数 $A$ 和 $B$ 指定，表示将田地 $A$ 的草更新为类型 $B$。

### 输出格式

对于每次更新，输出更新后种植不同草类型的两块田地之间的最短路径长度。

```input1
3 2 3 4
1 2 3
2 3 1
1 1 2
3 3
2 3
1 2
2 2
```

```output1
1
3
3
1
```

