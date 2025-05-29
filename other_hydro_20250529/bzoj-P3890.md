## 题目描述

Bessie and her sister Elsie want to travel from the barn to their favorite field, such that they leave at exactly the same time from the barn, and also arrive at exactly the same time at their favorite field. The farm is a collection of $n$ fields numbered $1$..$n$, where field $1$ contains the barn and field $n$ is the favorite field. The farm is built on the side of a hill, with field $X$ being higher in elevation than field $Y$ if $X < Y$. An assortment of $m$ paths connect pairs of fields. However, since each path is rather steep, it can only be followed in a downhill direction. For example, a path connecting field $5$ with field $8$ could be followed in the $5 \to 8$ direction but not the other way, since this would be uphill. It might take Bessie and Elsie different amounts of time to follow a path; for example, Bessie might take $10$ units of time, and Elsie $20$. Moreover, Bessie and Elsie only consume time when traveling on paths between fields -- since they are in a hurry, they always travel through a field in essentially zero time, never waiting around anywhere. Please help determine the shortest amount of time Bessie and Elsie must take in order to reach their favorite field at exactly the same moment.

**翻译：**

Bessie 和 Elsie 想从农场的田地 $1$ 到田地 $n$。农场由 $n$ 块编号 $1\cdots n$ 的田地构成。

农场建在山上，所以如果 $X<Y$，则满足第 $X$ 块田地的高度高于第 $Y$ 块田地。在农场中，有 $m$ 条道路将不同的田地连接起来。

不过，由于山路陡峭，这些小路只能沿着**从高到低**的方向走。例如，一条连接第 $5$ 块田地和 $8$ 块田地的小路只能沿着 $5\to 8$ 的方向走，而不能沿着其他方向。两块田地之间最多只有一条小路。

Bessie 和 Elsie 走同一条小路可能会花费不同的时间。比如，通过同一条小路，Bessie 可能会耗费 $10$ 个单位的时间，而 Elsie 会耗费 $20$ 个单位的时间。

此外，她们只会在通过小路时耗费时间。在穿过田地时不会耗费时间，也不会停下来等待。

问： Bessie 和 Elsie 同时出发并且同时到达田地 $n$ 的最短的时间。

## 输入格式

The first input line contains $n$ and $m$, separated by a space.

Each of the following $m$ lines describes a path using four integers $a,b,c,d$, where $a$ and $b$ (with $a < b$) are the fields connected by the path, $c$ is the time required for Bessie to follow the path, and $d$ is the time required for Elsie to follow the path.

第一行两个整数 $n,m$，用空格分开。

接下来 $m$ 行，每行四个整数 $a,b,c,d$，其中 $a,b(a<b)$ 表示两块用这条小路连接的田地，$c$ 表示 Bessie 通过这条小路的时间， $d$ 表示 Elsie 通过这条小路的时间。

## 输出格式

A single integer, giving the minimum time required for Bessie and Elsie to travel to their favorite field and arrive at the same moment. If this is impossible, or if there is no way for Bessie or Elsie to reach the favorite field at all, output the word `IMPOSSIBLE` on a single line.

一个整数，表示她们同时出发并同时到达的最短时间。如果无法同时到达，输出 `IMPOSSIBLE`。

```input1
3 3
1 3 1 2
1 2 1 2
2 3 1 2
```

```output1
2
```

## 样例说明

Bessie is twice as fast as Elsie on each path, but if Bessie takes the path $1\to 2 \to 3$ and Elsie takes the path $1\to 3$ they will arrive at the same time.

Bessie 在每一条路都比 Elsie 快两倍。

若 Bessie 经过 $1\to 2\to 3$ 的路线，Elsie 经过 $1\to 3$ 的路线，她们可以同时到达。

## 数据规模与约定

 对于 $100\%$ 的数据，$1 \le n \le 100$，$m \le \frac{n\times (n-1)}{2}$，$1\le c,d\le 100$。

## 题目来源

Silver