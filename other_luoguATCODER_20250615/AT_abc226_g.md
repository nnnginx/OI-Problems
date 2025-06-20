# AT_abc226_g [ABC226G] The baggage

## 题目描述

有质量为 $1 \sim 5$ 的重物，质量为 $i(1 \leq i \leq 5)$ 的重物有 $A_i$ 个；同时有可搬运的最大质量不超过 $i(1 \leq i \leq 5)$ 的人 $B_i$ 个。 问是否存在一种分配方式，使所有重物均可被一次性搬运。

## 输入格式

本题具有多组测试数据。

第 $1$ 行为一个整数 $T$，表示本测试点共有 $T$ 组测试数据。

第 $2i (1 ≤ i ≤ T)$ 行为 $5$ 个整数，分别为 $A_{1}$，$A_{2}$，$A_{3}$，$A_{4}$，$A_{5}$。

第 $2i+1 (1 ≤ i ≤ T)$ 行为 $5$ 个整数，分别为 $B_{1}$，$B_{2}$，$B_{3}$，$B_{4}$，$B_{5}$。

## 输出格式

输出共 $T$ 行，若 $i (1 ≤ i ≤ T)$ 组测试数据中所有重物均可被一次性搬运，则在第 $i$ 行输出 `Yes` ，否则输出 `No`。

## 输入输出样例 #1

### 输入 #1

```
3
5 1 0 0 1
0 0 0 2 1
0 3 0 0 0
0 0 2 0 0
10000000000000000 0 0 0 0
0 0 0 0 2000000000000000
```

### 输出 #1

```
Yes
No
Yes
```