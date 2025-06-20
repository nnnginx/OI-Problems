# AT_past202104_l 都市計画

## 题目描述

在平面直角坐标系上有 $n$ 个点（编号 $1$ 至 $n$）和 $m$ 个圆（编号 $1$ 至 $m$）。第 $i$ 个点的坐标为 $(p_i,q_i)$；第 $i$ 个圆的圆心点坐标为 $(x_i,y_i)$，半径为 $r_i$。

现在你要在这个坐标系中画一些线段，每条线段的端点都是上述 $n$ 个点之一或位于上述 $m$ 个圆之一的边缘。在画完这些线段后，你需要保证上述 $n$ 个点中的任意两个都能通过圆的边缘和你画的线段联通。

请求出你画出的线段的长度的和的最小值。

## 输入格式

第一行输入两个整数，$n$ 和 $m$。

接下来 $n$ 行，每行输入两个整数 $p_i,q_i$。

最后 $m$ 行，每行输入三个整数 $x_i,y_i,r_i$。

## 输出格式

输出一行一个实数，你的答案。请将误差控制在 $10^{-5}$ 以内。

## 输入输出样例 #1

### 输入 #1

```
2 1
0 0
6 0
3 0 2
```

### 输出 #1

```
2.00000000000
```

## 输入输出样例 #2

### 输入 #2

```
2 2
4 2
0 1
0 0 2
0 1 4
```

### 输出 #2

```
2.12310562562
```

## 输入输出样例 #3

### 输入 #3

```
3 4
9 2
5 20
0 21
0 0 2
0 0 10
16 0 10
10 15 3
```

### 输出 #3

```
13.10603728957
```

## 说明/提示

#### 样例 #1 说明

![样例 #1 图](https://img.atcoder.jp/past202104/70ffd4874808032c5c57f53fdabbd4a8.png)

如图，画出以下两条线段即可。

| 端点 1 | 端点 2 |
| :----------: | :----------: |
| $(0,0)$ | $(1,0)$ |
| $(5,0)$ | $(6,0)$ |

#### 样例 #2 说明

![样例 #2 图](https://img.atcoder.jp/past202104/18299e958b01610e07dc58b413b73cfb.png)

如图，画出以下三条线段即可。

| 端点 A | 端点 B |
| :-----------: | :-----------: |
| $(0,1)$ | $(0,2)$ |
| $(0,-2)$ | $(0,-3)$ |
| $(\frac{16\sqrt{17}}{17},1+\frac{4\sqrt{17}}{17})$ | $(4,2)$ |

#### 样例 #3 说明

![样例 #3 图](https://img.atcoder.jp/past202104/5cb78063bd44131bd78ef88726db263c.png)

图片如上。

#### 数据规模与约定

对于 $100\%$ 的数据，保证：

- $2 \le n \le 50$，$1 \le m \le 8$；
- $0 \le p_i,q_i,x_i,y_i \le 1000$；
- $1 \le r_i \le 1000$；
- 没有两个及以上的点在同一位置，没有两个及以上的圆的圆心在同一位置。