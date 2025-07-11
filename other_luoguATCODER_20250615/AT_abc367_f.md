# AT_abc367_f [ABC367F] Rearrange Query

## 题目描述

给定两个长度为 $N$ 的正整数序列 $A=(A_1,A_2,\ldots,A_N)$ 和 $B=(B_1,B_2,\ldots,B_N)$。

你需要处理 $Q$ 个查询。对于第 $i$ 个查询，给定四个正整数 $l_i$, $r_i$, $L_i$, 和 $R_i$。你需要判断是否可以通过重新排列序列 $(A_{l_i},A_{l_i+1},\ldots,A_{r_i})$ 来使其与 $(B_{L_i},B_{L_i+1},\ldots,B_{R_i})$ 完全相同。如果可以做到，则输出 `Yes`；否则输出 `No`。

## 输入格式

输入以以下格式从标准输入中给出：

- 第一行包含 $N$, $Q$, 接着是序列 $A$ 的元素 $A_1, A_2, \ldots, A_N$ 和序列 $B$ 的元素 $B_1, B_2, \ldots, B_N$。
- 接下来有 $Q$ 行，每行包含四个整数 $l_i$, $r_i$, $L_i$, 和 $R_i$，代表每个查询。

## 输出格式

输出共 $Q$ 行。第 $i$ 行输出第 $i$ 个查询的答案。

## 输入输出样例 #1

### 输入 #1

```
5 4
1 2 3 2 4
2 3 1 4 2
1 3 1 3
1 2 3 5
1 4 2 5
1 5 1 5
```

### 输出 #1

```
Yes
No
No
Yes
```

## 输入输出样例 #2

### 输入 #2

```
4 4
4 4 4 4
4 4 4 4
1 2 2 3
3 3 1 1
1 3 1 4
1 4 2 3
```

### 输出 #2

```
Yes
Yes
No
No
```

## 说明/提示

#### 制约条件

- $1 \leq N, Q \leq 2 \times 10^5$
- $1 \leq A_i, B_i \leq N$
- $1 \leq l_i \leq r_i \leq N$
- $1 \leq L_i \leq R_i \leq N$
- 所有输入均为整数。

#### 示例解释 1

- 对于第 1 个查询，$(1,2,3)$ 可以通过重排变为 $(2,3,1)$。因此输出 `Yes`。
- 对于第 2 个查询，无论怎样重排 $(1,2)$ 都无法变为 $(1,4,2)$。因此输出 `No`。
- 对于第 3 个查询，无论怎样重排 $(1,2,3,2)$ 都无法变为 $(3,1,4,2)$。因此输出 `No`。
- 对于第 4 个查询，$(1,2,3,2,4)$ 可以通过重排变为 $(2,3,1,4,2)$。因此输出 `Yes`。