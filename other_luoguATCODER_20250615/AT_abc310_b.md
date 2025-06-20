# AT_abc310_b [ABC310B] Strictly Superior

## 题目描述

#### 题意简述
商店有 $N$ 个产品。第 $i$ 个产品的价格为 $P_i$ ，并且有 $C_i$ 个功能。这些功能的数值不超过 $M$ 。

在这里，如果满足以下条件，则称产品 $i$ “绝对优越” 于产品 $j$ ：

- $P_i \ge P_j$。
- 产品 $i$ 的所有功能产品 $j$ 都有。
- $P_i > P_j$ ，或者产品 $j$ 有至少一个功能是产品 $i$ 所没有的。

请你计算是否存在一个产品 “绝对优越” 于另一个产品。

## 输入格式

第一行有两个整数： $N,M$

接下来 $N$ 行，每行第一个整数为 $P_i$ ，第二个整数为 $C_i$ 。后面 $C_i$ 个整数为 $F_{i,j}$ ，表示第 $i$ 个产品的第 $j$ 个功能。

## 输出格式

如果有 “绝对优越” 的产品，输出 $Yes$ 。否则输出 $No$ 。

## 输入输出样例 #1

### 输入 #1

```
5 6
10000 2 1 3
15000 3 1 2 4
30000 3 1 3 5
35000 2 1 5
100000 6 1 2 3 4 5 6
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
4 4
3 1 1
3 1 2
3 1 2
4 2 2 3
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
20 10
72036 3 3 4 9
7716 4 1 2 3 6
54093 5 1 6 7 8 10
25517 7 3 4 5 6 7 9 10
96930 8 2 3 4 6 7 8 9 10
47774 6 2 4 5 6 7 9
36959 5 1 3 4 5 8
46622 7 1 2 3 5 6 8 10
34315 9 1 3 4 5 6 7 8 9 10
54129 7 1 3 4 6 7 8 9
4274 5 2 4 7 9 10
16578 5 2 3 6 7 9
61809 4 1 2 4 5
1659 5 3 5 6 9 10
59183 5 1 2 3 4 9
22186 4 3 5 6 8
98282 4 1 4 7 10
72865 8 1 2 3 4 6 8 9 10
33796 6 1 3 5 7 9 10
74670 4 1 2 6 8
```

### 输出 #3

```
Yes
```

## 说明/提示

- $2 \le N \le 100$
- $1 \le M \le 100$
- $1 \le P_i \le 10^5 (1 \le i \le N)$
- $1 \le C_i \le M (1 \le i \le N)$
- $1 \le F_{i,1} < F_{i,2} < ... < F_{i,C_i} \le M(1 \le i \le N)$