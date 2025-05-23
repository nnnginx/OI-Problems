# 最小环

奶龙刚学会怎么找环，暴暴龙就来难为他了。

暴暴龙给了奶龙一张 $n$ 个点，$m$ 条边的简单无向图。一个简单环的价值计做环上最小的边权，请你帮奶龙找出图上所有简单环里，最小的一个价值是多少。

图不保证联通，但保证图中至少有一个简单环。

### 输入格式

第一行，两个整数表示点数，边数 $n, m$；
接下来的 $m$ 行，每行三个整数 $u_i, v_i, w_i$，表示 $u_i$ 到 $v_i$ 有一条价值为 $w_i$ 的无向边。

### 输出格式

一行一个整数，输出你的答案。

## 样例

### 样例输入 #1

```
6 6
1 2 1
2 3 1
3 1 1
4 5 1
5 6 1
6 4 1
```

### 样例输出 #1

```
1
```

### 样例输入 #2

```
6 6
1 2 10
2 3 8
3 1 5
4 5 100
5 6 40
6 4 3
```

### 样例输出 #2

```
3
```

### 样例输入 #3

```
6 15
1 2 4
5 2 8
6 1 7
6 3 10
6 5 1
3 2 8
4 3 4
5 3 6
2 6 6
5 4 5
4 1 3
6 4 5
4 2 1
3 1 7
1 5 5
```

### 样例输出 #3

```
1
```

### 样例输入 #4

```
4 6
2 3 2
1 3 10
1 4 1
3 4 7
2 4 5
1 2 2
```

### 样例输出 #4

```
1
```

### 数据范围与约定

对于 $20\%$ 的数据，保证 $n=m$，且$\forall i$，$i$ 到 $(i\mod n)+1$ 有一条边；
对于 $40\%$ 的数据，$n, m \leq 200$；
对于 $100\%$ 的数据，$1\leq n, m\leq 2\times 10^5, 1\leq w_i \leq 10^9$