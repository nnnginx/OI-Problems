# AT_ddcc2019_final_d DISCO!

## 题目描述

高桥君写下了字符串 $S$ 。请回答接下来的 $Q$ 个问题。

- 问题 $q(1 \le q \le  Q)$：给出整数 $L_q$、$R_q$。满足 $S_i = D$，$S_j = I$，$S_k=S$，$S_l = C$，$S_m = O$ 的组 $(i,j,k,l,m)(L_q \le i < j < k < l < m \le R_q)$ 有多少个？求出这个数量对 $2^{32}$ **取余的结果**。

## 输入格式

输入以以下形式从标准输入中给出。

> $ S $ $ Q $ $ L_1 $ $ R_1 $ $ L_2 $ $ R_2 $ $ L_3 $ $ R_3 $ $ : $ $ L_Q $ $ R_Q $

## 输出格式

输出 $Q$ 行。第 $q$ 行输入表示对问题 $q$ 的答案。

### 输入输出样例

#### 输入 #1

```
DDDDDDISCOOOOOO
7
6 10
5 11
4 12
3 13
2 14
1 15
1 8
```

#### 输出 #1

```
1
4
9
16
25
36
0
```


#### 输入 #2

```
DDDIIISSSCCCOOO
12
1 12
1 13
1 14
1 15
2 12
2 13
2 14
2 15
3 13
3 14
3 15
4 15
```

#### 输出 #2

```
0
81
162
243
0
54
108
162
27
54
81
0
```

## 输入输出样例 #1

### 输入 #1

```
DDDDDDISCOOOOOO
7
6 10
5 11
4 12
3 13
2 14
1 15
1 8
```

### 输出 #1

```
1
4
9
16
25
36
0
```

## 输入输出样例 #2

### 输入 #2

```
DDDIIISSSCCCOOO
12
1 12
1 13
1 14
1 15
2 12
2 13
2 14
2 15
3 13
3 14
3 15
4 15
```

### 输出 #2

```
0
81
162
243
0
54
108
162
27
54
81
0
```

## 说明/提示

### 约束

- $S$ 是由 ```D```、```I```、```S```、```C```、```O``` 构成的长度为 $1 000 000$ 以下的字符串。
- $1 \le Q \le 100 000$
- $1 \le L_q \le R_q \le \left | S \right | $
- $L_q,R_q$ 为整数。