## 题目描述

在 JIH 考察的地图中有 $n$ 个城市，被公路依次连成了一个环，JIH 想在这些城市中建一个玩具厂。

城市和公路都被编号为 $1$ 到 $n$，$i$ 号公路连接 $i-1$ 号城市与 $i$ 号城市（$1$ 号公路连接 $n$ 号城市与 $1$ 号城市），每个城市对玩具的需求为 $w_i$，每条公路的长度为 $d_i$。当 JIH 在第 $i$ 号城市建玩具厂时，JIH 需要将玩具运输到其他城市（当然 $i$ 城市除外）。设第 $i$ 号城市到第 $j$ 号城市的两条路径长度分别为 $l_1,l_2$，则将玩具运输到第 $j$ 号城市的费用为 $l_1\times l_2\times w_j$。总的运输费用为将玩具运到所有城市的运输费用的总和。

JIH 当然想要总的运输费用最少，所以他会选最优的城市建玩具厂，如果有多个最优的城市，小月会等概率的选取其中一个建玩具厂。

由于 JIH 的调查工作没做好，只知道 $1$ 到 $n-1$ 号城市的 $w_i$，而 $n$ 号城市的 $w_i$ 只知道它的取值范围 $[a,b]$，假设 $w_i$ 的值在实数区间 $[a,b]$ 上的概率是均匀分布的。

现在 JIH 只好去进行第二次调查，于是我们想知道每个城市建玩具厂的概率是多少。

## 输入格式

第一行三个正整数 $n,a,b$。

接下来 $n-1$ 行每行一个正实数 $w_{1\cdots n-1}$。

接下来 $n$ 行每行一个正实数 $d_{1\cdots n}$。

## 输出格式

$n$ 行，每行一个实数，表示在第 $i$ 个城市建厂的概率。

```input1
5 1 100
50
25
25
50
1
2
3
2
1
```

```output1
0.090
0.000
0.000
0.090
0.821
```

## 样例解释

当 $w_5<18.75$，将在 $1$ 或 $4$ 号城市建厂。

当 $w_5>18.75$，将在 $5$ 号城市建厂。

当 $w_5=18.75$，将在 $1,4$ 或 $5$ 号城市建厂。

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq 10^5$，$a\leq b\leq 10^4$，$w_i\leq 10^4$，$d_i\leq 10$。

