# AT_abc401_e [ABC401E] Reachable Set

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc401/tasks/abc401_e

给定一个包含 $N$ 个顶点和 $M$ 条边的无向图。顶点编号为 $1,2,\ldots,N$，第 $i$ 条边 $(1 \leq i \leq M)$ 连接顶点 $u_i$ 和顶点 $v_i$。

对于每个 $k=1,2,\ldots,N$，请解决以下问题：

> 考虑以下操作：
> 
> - 选择一个顶点，删除该顶点及其所有连接的边。
>  
> 通过重复上述操作，判断是否能够满足以下条件：
> 
> - 从顶点 $1$ 出发，通过边能够到达的顶点集合恰好为 $\{1,2,\ldots,k\}$（共 $k$ 个顶点）。
>  
> 如果可能，求出满足条件所需的最少操作次数；否则输出 `-1`。

## 输入格式

输入通过标准输入给出，格式如下：

> $N$ $M$  
> $u_1$ $v_1$  
> $u_2$ $v_2$  
> $\vdots$  
> $u_M$ $v_M$

## 输出格式

输出 $N$ 行。第 $i$ 行 $(1 \leq i \leq N)$ 输出 $k=i$ 时的答案：若无法满足条件则输出 `-1`，否则输出所需的最少操作次数。

## 输入输出样例 #1

### 输入 #1

```
6 7
1 2
1 5
2 3
2 4
2 5
3 6
5 6
```

### 输出 #1

```
2
3
3
2
1
0
```

## 输入输出样例 #2

### 输入 #2

```
5 4
1 5
2 3
3 4
4 5
```

### 输出 #2

```
1
-1
-1
-1
0
```

## 输入输出样例 #3

### 输入 #3

```
2 0
```

### 输出 #3

```
0
-1
```

## 输入输出样例 #4

### 输入 #4

```
11 25
6 9
5 9
2 3
1 9
10 11
4 5
9 10
8 9
7 8
3 5
1 7
6 10
4 7
7 9
1 10
4 11
3 8
2 7
3 4
1 8
2 8
3 7
2 10
1 6
6 11
```

### 输出 #4

```
5
-1
-1
-1
-1
-1
4
3
2
1
0
```

## 说明/提示

### 约束条件

- $1 \leq N \leq 2 \times 10^5$
- $0 \leq M \leq 3 \times 10^5$
- $1 \leq u_i < v_i \leq N$ $(1 \leq i \leq M)$
- $(u_i, v_i) \neq (u_j, v_j)$ $(1 \leq i < j \leq M)$
- 输入的所有数值均为整数

### 样例解释 1

例如，当 $k=2$ 时，可以通过删除顶点 $3$、顶点 $4$ 和顶点 $5$（共 3 次操作），使得从顶点 $1$ 可达的顶点仅为 $\{1,2\}$。由于无法通过少于 3 次操作满足条件，因此第 2 行输出 `3`。  
当 $k=6$ 时，不需要删除任何顶点即可满足条件，因此第 6 行输出 `0`。

### 样例解释 3

图中可能不存在任何边。

翻译由 DeepSeek V3 完成