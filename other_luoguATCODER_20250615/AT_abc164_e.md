# AT_abc164_e [ABC164E] Two Currencies

## 题目描述

有 $n$ 个城市，它们由 $m$ 条双向道路连接，保证它们能够彼此到达。第 $i$ 条道路连接 $u_i,v_i$，需要花费 $x_i$ 个银币，耗费 $t_i$ 秒的时间。每个城市处都有兑换银币处，第 $i$ 个城市中你可以用 $1$ 个金币兑换 $c_i$ 个银币，可以兑换无限次，不过兑换 $1$ 次需要花费 $d_i$ 秒的时间。你一开始在 $1$ 号城市，有 $s$ 个银币和无限多的金币，求到其它城市需要耗费的最小时间。

$1 \leq n \leq 50$，$n - 1 \le m \le 100$，$1 \leq x_i \leq 50$，$1 \leq t_i,d_i \leq 10^9$，$1 \leq s,c_i \leq 10^9$

## 输入格式

- 第一行 $n,m,s$
- 接下来 $m$ 行 $u_i,v_i,x_i,t_i$
- 接下来 $n$ 行 $c_i,d_i$

## 输出格式

一个整数表示答案。

## 输入输出样例 #1

### 输入 #1

```
3 2 1
1 2 1 2
1 3 2 4
1 11
1 2
2 5
```

### 输出 #1

```
2
14
```

## 输入输出样例 #2

### 输入 #2

```
4 4 1
1 2 1 5
1 3 4 4
2 4 2 2
3 4 1 1
3 1
3 1
5 2
6 4
```

### 输出 #2

```
5
5
7
```

## 输入输出样例 #3

### 输入 #3

```
6 5 1
1 2 1 1
1 3 2 1
2 4 5 1
3 5 11 1
1 6 50 1
1 10000
1 3000
1 700
1 100
1 1
100 1
```

### 输出 #3

```
1
9003
14606
16510
16576
```

## 输入输出样例 #4

### 输入 #4

```
4 6 1000000000
1 2 50 1
1 3 50 5
1 4 50 7
2 3 50 2
2 4 50 4
3 4 50 3
10 2
4 4
5 5
7 7
```

### 输出 #4

```
1
3
5
```

## 输入输出样例 #5

### 输入 #5

```
2 1 0
1 2 1 1
1 1000000000
1 1
```

### 输出 #5

```
1000000001
```