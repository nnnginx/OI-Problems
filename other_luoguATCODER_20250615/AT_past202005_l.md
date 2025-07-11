# AT_past202005_l スーパーマーケット

## 题目描述

一个自动售货机有编号为 $1$ 到 $n$ 的 $n$ 个通道。第 $i$ 个通道内有 $k_i$ 个商品，价值从前往后依次为 $t_{i,1},t_{i,2},...,t_{i,k_i}$。保证所有 $t_{i,j}$ 互不相同。

有 $m$ 位顾客先后使用了这台自动售货机。第 $i$ 个使用的顾客会检查每个通道内最靠前的 $a_i$ 个商品的价值（若少于 $a_i$ 则全部检查），然后选择最大的并买下。请将所有客户买走的产品的价值分别求出。

## 输入格式

第一行：一个整数 $n$。

接下来 $n$ 行：第 $i$ 行第 $1$ 个数为 $k_i$，然后是 $k_i$ 个数 $t_{i,1},t_{i,2},...,t_{i,k_i}$。

接下来一行：一个整数 $m$。

接下来一行：$m$ 个整数 $a_1,a_2,...,a_m$。

## 输出格式

$m$ 行，第 $i$ 行输出一个正整数，即第 $i$ 名顾客买走的商品的价值。

### 数据约束条件

- 输入均为整数；
- $1 \le n,k_i \le 10^5$；
- $1 \le m \le$ 所有 $k_i$ 之和 $\le 3 \times 10^5$；
- $1 \le t_{i,j} \le 10^9$；
- $1 \le a_i \le 2$。

## 输入输出样例 #1

### 输入 #1

```
2
3 1 200 1000
5 20 30 40 50 2
5
1 1 1 2 2
```

### 输出 #1

```
20
30
40
200
1000
```

## 输入输出样例 #2

### 输入 #2

```
10
6 8 24 47 29 73 13
1 4
5 72 15 68 49 16
5 65 20 93 64 91
6 100 88 63 50 90 44
2 6 1
10 14 2 76 28 21 78 43 11 97 70
5 31 9 62 84 40
8 10 46 96 23 98 19 38 51
2 37 77
20
1 1 1 1 2 2 2 1 1 2 2 2 2 2 1 2 1 2 2 1
```

### 输出 #2

```
100
88
72
65
93
77
68
63
50
90
64
91
49
46
44
96
37
31
62
20
```