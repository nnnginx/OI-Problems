# AT_abc240_e [ABC240E] Ranges on Tree

## 题目描述

### 题面简述

给出一个有 $N$ 个节点的树和其中的 $N-1$ 条树边（描述无向），其中我们规定节点编号为 $1,2,\cdots,N-1,N$，其中节点 $1$ 为树根。

你需要给予每一个节点 $i$ 一个闭区间 $[L_i,R_i]$，你需要保证一下性质。

- 虽然当 $L_i=R_i$ 的时候不满足闭区间书写规范，但是在本题中允许出现。

- $\forall_i,1\le L_i\le R_i$。

- 如果 $i$ 是 $j$ 的父亲节点，保证 $[L_j,R_j]\subseteq [L_i,R_i]$。

- 如果 $i,j$ 为兄弟节点（拥有相同的父亲节点），那么保证 $[L_i,R_i]\cap[L_j,R_j]=\varnothing$。

你需要保证你构造出的方案的 $\max\limits_{i=1}^{N} R_i$ 最小。

## 输入格式

如以下形式输入。

> $ N $ $ u_1 $ $ v_1 $ $ u_2 $ $ v_2 $ $ \vdots $ $ u_{N-1} $ $ v_{N-1} $

## 输出格式

如一下形式输出，对于每一组 $L_i$ 与 $R_i$ 之间需要空格，不同组之间用换行分开。

> $ L_1 $ $ R_1 $ $ L_2 $ $ R_2 $ $ \vdots $ $ L_N $ $ R_N $

@[_qingshu_](https://www.luogu.com.cn/user/602803) 译。

## 输入输出样例 #1

### 输入 #1

```
3
2 1
3 1
```

### 输出 #1

```
1 2
2 2
1 1
```

## 输入输出样例 #2

### 输入 #2

```
5
3 4
5 4
1 2
1 4
```

### 输出 #2

```
1 3
3 3
2 2
1 2
1 1
```

## 输入输出样例 #3

### 输入 #3

```
5
4 5
3 2
5 2
3 1
```

### 输出 #3

```
1 1
1 1
1 1
1 1
1 1
```