## 题目描述

这里有 $n$ 座城镇，和城镇之间的 $m$ 条巴士单行线（没有中间停靠站），城镇从 $1$ 到 $n$ 标号。

一个旅行者在 $0$ 时刻位于 $1$ 号城镇想要到达 $p$ 号城镇。他将乘坐巴士在 $t$ 时刻到达 $p$ 号城镇，如果他早到了，他必须等待。

对于任意一个巴士路线 $i$，我们知道其中的起点城镇 $s_i$ 和目标城镇 $t_i$。我们也同样知道路线的出发时间和到达时间，但仅仅是近似值：我们知道巴士在时间范围 $[a_i, b_i]$ 内离开起点城镇 $s_i$，且在时间范围 $[c_i, d_i]$ 内到达目标城镇 $t_i$（端点值包括在内）。

旅行者不喜欢等待，因此他要寻找一个旅行计划使得最大等待时间尽量小，同时保证绝对不会错过计划中的任何一辆巴士（意思是，每次他换乘巴士，他需要下车的巴士的最晚到达时间不会迟于他需要搭乘的下一辆巴士的最早出发时间）。

当计算等待时间时，我们必须假设最早可能到达的时间和最晚可能出发的时间。

编写一个程序，寻找一个最为合理的搭车计划。

## 输入格式

The input file name is `TRIP.IN`.

The first line contains the integer numbers $n,m,p$ , and $t$ . 

The following $m$ lines describe the bus routes. 

Each line contains the integer numbers $s_i, t_i, a_i, b_i, c_i, d_i$, where $s_i$ and $t_i$ are the source and destination towns of the bus route $i$, and $a_i, b_i, c_i, d_i$ describe the departure and arrival times as explained above ).

## 输出格式

只需要包含一个数——最合理搭车方案的最长可能等待时间。

如果不可能保证在 $t$ 时刻到达城市 $p$，那么输出 `-1`。



```input1
3 6 2 100
1 3 10 20 30 40
3 2 32 35 95 95
1 1 1 1 7 8
1 3 8 8 9 9
2 2 98 98 99 99
1 2 0 0 99 101
```



```output1
32
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq 5\times 10^4$，$1\leq m\leq 10^4$，$1\leq p\leq n$，$0\leq t\leq 10^9$，$1\leq s_i,t_i\leq n$，$0\leq a_i\leq b_i < c_i \leq d_i\leq 10^9$。

