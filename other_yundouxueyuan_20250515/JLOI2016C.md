## 题目描述

小 R 和 B 神正在玩一款游戏。这款游戏的地图由 $n$ 个点和 $n - 1$ 条无向边组成，每条无向边连接两个点，且地图是连通的。换句话说，游戏的地图是一棵有 $n$ 个节点的树。

游戏中有一种道具叫做侦查守卫，当一名玩家在一个点上放置侦查守卫后，它可以监视这个点以及与这个点的距离在 $d$ 以内的所有点。这里两个点之间的距离定义为它们在树上的距离，也就是两个点之间唯一的简单路径上所经过边的条数。

在一个点上放置侦查守卫需要付出一定的代价，在不同点放置守卫的代价可能不同。现在小 R 知道了所有 B 神可能出现的位置，请你计算监视所有这些位置的最小代价。

## 输入格式

第一行包含两个正整数 $n$ 和 $d$，分别表示地图上的点数和侦查守卫的视野范围。约定地图上的点用 $1$ 到 $n$ 的正整数编号。
第二行包含 $n$ 个正整数，第 $i$ 个正整数表示在编号为 $i$ 的点放置侦查守卫的代价 $w_i$。保证 $w_i \leq 1000$。
第三行包含一个正整数 $m$，表示 B 神可能出现的点的数量。保证 $m \leq n$。
第四行包含$m$ 个正整数，分别表示每个 B 神可能出现的点的编号，从小到大不重复地给出。
接下来 $n - 1$ 行，每行包含两个整数 $u, v$，表示在编号为 $u$ 的点和编号为 $v$ 的点之间有一条无向边。

## 输出格式

输出一行一个整数，表示监视所有 B 神可能出现的点所需要的最小代价。

```input1
12 2
8 9 12 6 1 1 5 1 4 8 10 6
10
1 2 3 5 6 7 8 9 10 11
1 3
2 3
3 4
4 5
4 6
4 7
7 8
8 9
9 10
10 11
11 12
```

```output1
10
```

## 数据范围与提示

| Case \# | $n$ | $d$ | 附加限制 |
| :------:|:---:|:---:|:---: |
| 1       | $\leq 20$       | $\leq 5$  | - |
| 2, 3    | $\leq 500\,000$ | $= 1$     | -  |
| 4, 5    | $\leq 500\,000$ | $\leq 20$ | $n = m$ |
| 6, 7, 8 | $\leq 10\,000$  | $\leq 20$ | - |
| 9, 10   | $\leq 500\,000$ | $\leq 20$ | - |



