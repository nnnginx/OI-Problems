## 题目背景
译自 [XXXI Olimpiada Informatyczna - I etap](https://sio2.mimuw.edu.pl/c/oi31-1/dashboard/) [Budowa lotniska](https://sio2.mimuw.edu.pl/c/oi31-1/p/bud/)。

## 题目描述
给你一个 $n\times n$ 的地图，地图上有 `.` 有 `X`。

求出最大的 $k$，使得：

在地图上能找到 $m(m\leq 2)$ 个 $1\times k$ 或 $k\times 1$ 的长条，使得长条不交且长条内全是 `.`。

## 输入格式
第一行两个正整数 $n,m$。

接下来 $n$ 行，描述地图。

## 输出格式
一行一个非负整数，最大的 $k$。

```input1
5 2
.X...
.XXXX
XX...
.....
.X.X.

```

```output1
3

```

```input2
2 1
..
..

```

```output2
2

```

```input3
2 2
X.
..

```

```output3
1

```

```input4
10 2
XXXXXXXXXX
XXXXXXXXXX
XXXXXXXXXX
XXXXXXXXXX
XXXXXXXXXX
..........
XXXXXXXXXX
XXXXXXXXXX
XXXXXXXXXX
XXXXXXXXXX

```

```output4
5

```

```input5
10 2
XX.XXXXX.X
XX.XXXXX.X
XX.XXXXX.X
XX.XXXXX.X
XX.XXXXX.X
XX.XXXXX.X
XX.XXXXX.X
XX.XXXXX.X
XX.XXXXX.X
XX.XXXXX.X

```

```output5
10

```

```input6
见附件
```

```output6
531

```

## 提示
样例解释：

```plain
.X...
.XXXX
XX..2
111.2
.X.X2
```

对于所有数据，$1\leq n\leq1500$，$1\leq m\leq2$，地图上只有 `.` 和 `X`。

| 子任务编号 | 附加限制 | 分值 |
| :----------: | :----------: | :----------: |
| 1 | $m=1$ | 20 |
| 2 | $n\leq 30$ | 22 |
| 3 | $n\leq 300$ | 23 |
| 4 |  | 35 |


