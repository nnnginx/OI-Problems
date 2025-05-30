## 题目描述

这是一道（集合幂级数问题转化为形式幂级数问题，利用求导 $O(n^2)$ 完成形式幂级数操作的）模板题。

给定一个集合 $S = \{{x_1}, {x_2}, \dots, {x_n}\}$ 和一个 $S$ 上的集合族 $\mathcal F = \{{S_0}, {S_1}, \dots, {S_{m-1}}\}$。

一个划分 $\mathcal P$ 是 $\mathcal F$ 的一个子族，满足 $\mathcal P$ 中所有集合的并为 $S$ ，任意两个集合不相交。

求大小不大于 $k$ 的划分的数量 $\text{mod}\;998244353 %% \bmod 会在前面产生一个空白。。$。

两个划分 ${\mathcal P_1}, {\mathcal P_2}$ 不同，当且仅当存在 $i$ 使 $S_i \in {\mathcal P_1} \land S_i \notin {\mathcal P_2}$ 或 $S_i \notin {\mathcal P_1} \land S_i \in {\mathcal P_2}$。$S_i$ 和 $S_j$ 不同当且仅当 $i \neq j$。

## 输入格式

第 $1$ 行：$n\ m\ k$

第 $2$ 行：$s_0\ s_1\ \ldots s_{m-1}$，$s_i$ 二进制第 $j$ 位为 $0$ 表示 ${x_j} \notin {S_i}$ ，为 $1$ 表示 ${x_j} \in {S_i}$

## 输出格式

$1$ 个非负整数，表示大小不大于 $k$ 的划分的数量 $\text{mod}\;998244353 %% \bmod 会在前面产生一个空白。。$。

```input1
4 8 2
7 10 8 11 5 15 4 5
```

```output1
5
```

## 数据范围与提示

* $1 \leq k \leq n \leq 21$
* $1 \leq m \leq 262144$
* $1 \leq s_i \leq 2^n-1 %% 想了想果然还是别非负整数了吧……$

#### 子任务

1. （16 分）$n \leq 7$，$m \leq 16$
2. （20 分）$n \leq 11$，$m \leq 256$
2. （14 分）$n \leq 14$，$m \leq 2048$
3. （25 分）$n \leq 18$，$m \leq 32768$
4. （25 分）没有附加限制

