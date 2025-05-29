## 题目背景
搬运自 <http://czoj.com.cn/p/955>。数据为民间数据。

## 题目描述
小 Y 有一个 $n\times n$ 棋盘，开始时这个棋盘每个格子的颜色是白黑相间的，即第一行的第 $1,3,5\cdots$ 个格子是白色，第 $2,4,6\cdots$ 个格子是黑色，第二行第 $2,4,6\cdots$ 个格子是白色，第 $1,3,5\cdots$ 个格子是黑色，如下图所示。


$$
\def\b{\color{ff}\rule{10px}{10px}\kern{1px}}
\def\w{\color{white}\rule{10px}{10px}\kern{1px}}
\def\bg{\color{black}\rule{33.5px}{33.5px}}
\def\eps{\\[-39.5px]}
\def\ep{\\[-5.5px]}
\begin{aligned}
\bg\eps
\w\b\w\ep
\b\w\b\ep
\w\b\w
\end{aligned}
$$

小 Y 会进行 $q$ 次操作，每次操作会将某一行或者某一列的所有格子的颜色反转，即白色格子变成黑色格子，黑色格子变成白色格子。

小 Y 想知道，在每次操作之后，一共有多少个同颜色（全黑或全白）的连通区域。这里联通指的是**四连通**，即两个格子之间有边相邻才算联通。



## 输入格式
第 $1$ 行 $2$ 个正整数 $n,q$，表示棋盘的大小和操作的次数。

第 $2$ 到 $q+1$ 行每行 $2$ 个正整数 $\text{opt}_i,a_i$，若 $\text{opt}_i=1$ 则表示反转的是行，$\text{opt}_i=2$ 则表示反转的是列，$a_i$ 表示反转的是第几行（列）。

## 输出格式
输出 $q$ 行每行一个整数，表示在经过该次操作后，一共有多少个同颜色的联通区域。



```input1
3 3
1 2
2 3
1 2
```

```output1
3
2
6
```

```input2
100000 1
1 1
```

```output2
9999900000
```

```input3
15000 5
1 90
1 1231
1 91
1 1233
1 1232
```

```output3
224970000
224940000
224940000
224910000
224940000
```

## 提示
### 样例 $\textbf 1$ 解释
$$
\def\b{\color{ff}\rule{10px}{10px}\kern{1px}}
\def\w{\color{white}\rule{10px}{10px}\kern{1px}}
\def\bg{\color{black}\rule{33.5px}{33.5px}}
\def\eps{\\[-39.5px]}
\def\ep{\\[-5.5px]}
\begin{aligned}
\bg\eps
\w\b\w\ep
\b\w\b\ep
\w\b\w
\end{aligned}
\to
\begin{aligned}
\bg\eps
\w\b\w\ep
\w\b\w\ep
\w\b\w
\end{aligned}
\to
\begin{aligned}
\bg\eps
\w\b\b\ep
\w\b\b\ep
\w\b\b
\end{aligned}
\to
\begin{aligned}
\bg\eps
\w\b\b\ep
\b\w\w\ep
\w\b\b
\end{aligned}
$$

### 数据范围
对于所有数据，$1≤q, n≤10^5, 1≤\text{opt}_i≤2, 1≤a_i≤n$。

|测试点编号|$n$|$q$|特殊性质|
|:-:|:-:|:-:|:-:|
|$1\sim4$|$\le 4$|$\le 10$|无|
|$5\sim6$|$\le10^5$|$=1$|无|
|$7\sim9$|$\le10^5$|$\le10^5$|$\alpha$|
|$10$|$\le10^5$|$\le10^5$|无|

- 特殊性质 $\alpha$：保证同一个测试点所有的 $\text{opt}_i$ 均相等。

