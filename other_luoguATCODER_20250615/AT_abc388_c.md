# AT_abc388_c [ABC388C] Various Kagamimochi

## 题目描述

有 $N$ 个大小不一的饼。第 $i$ 个饼的大小为 $a_i$（$1 \le i \le N$）。

对于任意两个大小分别为 $a$ 和 $b$ 的饼 $A$ 和 $B$，如果 $a$ 小于或等于 $b$ 的一半，即 $a\le \frac{b}{2}$，则可以将饼 $A$ 放在饼 $B$ 上制作一个“镜饼”。

从 $N$ 个饼中任选两个，使得其中一个饼放在另一个饼上制作一个“镜饼”。

需要求出可以制作多少种不同的“镜饼”。

此外，即使构成镜饼的饼的大小相同，只要至少有一个是不同的饼，就可以算作是另一种类型的镜饼。

**Translate by [chinazhanghaoxun](https://luogu.com.cn/user/684848)。**

## 输入格式

输入将以以下格式通过标准输入给出：

> $N \ A_1\ A_2\ \dots\ A_N$

## 输出格式

输出可以制作的镜饼数。
### 数据限制
- $2\le N\le 5\times 10^5$
- $1\le A_i \le 10^9(1\le i\le N)$
- $A_i\le A_{i+1}(1\le i\le N)$
- 输入值均为整数

## 输入输出样例 #1

### 输入 #1

```
6
2 3 4 4 7 10
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
3
387 388 389
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
32
1 2 4 5 8 10 12 16 19 25 33 40 50 64 87 101 149 175 202 211 278 314 355 405 412 420 442 481 512 582 600 641
```

### 输出 #3

```
388
```