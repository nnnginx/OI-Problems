# AT_abc406_f [ABC406F] Compare Tree Weights

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc406/tasks/abc406_f

给定一个有 $N$ 个顶点的树 $T$，顶点和边分别编号为顶点 $1$, 顶点 $2$, $\ldots$, 顶点 $N$ 和边 $1$, 边 $2$, $\ldots$, 边 $(N-1)$。

特别地，边 $i$ $(1 \leq i \leq N-1)$ 连接顶点 $U_i$ 和顶点 $V_i$。

此外，每个顶点都有一个权重，最初，所有顶点的权重都为 $1$。

给定 $Q$ 个查询，请按顺序处理它们。每个查询是以下两种类型之一：

- `1 x w`：将顶点 $x$ 的权重增加 $w$。
- `2 y`：如果删除边 $y$，$T$ 将分裂成两个子树（连通分量）。将每个子树中包含的顶点的权重总和作为该子树的权重时，输出两个子树权重的差。

关于第二种类型的查询，可以证明，从 $T$ 中选择任意一条边并删除它时，$T$ 总是会分裂成两个子树。

另外，请注意，第二种类型的查询实际上并没有删除边。

## 输入格式

输入按以下格式从标准输入给出。

> $N$  
> $U_1$ $V_1$  
> $U_2$ $V_2$  
> $\vdots$  
> $U_{N-1}$ $V_{N-1}$  
> $Q$  
> $\mathrm{query}_1$  
> $\mathrm{query}_2$  
> $\vdots$  
> $\mathrm{query}_Q$

每个查询 $\mathrm{query}_i$ $(1 \leq i \leq Q)$ 按以下任一格式给出。

> $1$ $x$ $w$
>
> $2$ $y$

## 输出格式

设第二种类型查询的个数为 $K$，输出 $K$ 行。第 $i$ 行 $(1 \leq i \leq K)$ 输出第 $i$ 个第二种类型查询的答案。

## 输入输出样例 #1

### 输入 #1

```
6
1 2
1 3
2 4
4 5
4 6
5
2 1
1 1 3
2 1
1 4 10
2 5
```

### 输出 #1

```
2
1
17
```

## 说明/提示

**「数据范围」**

- $2 \leq N \leq 3 \times 10^5$
- $1 \leq U_i, V_i \leq N$
- $1 \leq Q \leq 3 \times 10^5$
- $1 \leq x \leq N$
- $1 \leq w \leq 1000$
- $1 \leq y \leq N-1$
- 输入均为整数
- 给定的图是一棵树。
- 至少存在一个第二种类型的查询。

**「样例 1 解释」**

树 $T$ 的结构和顶点编号对应如下图左所示。最初，所有顶点的权重都为 $1$。

对于第 $1$ 个查询，考虑删除边 $1$。此时，树会分裂成包含顶点 $1$ 的子树和包含顶点 $2$ 的子树。包含顶点 $1$ 的子树的权重为 $2$，包含顶点 $2$ 的子树的权重为 $4$，因此输出它们的差 $2$。（下图右）

![](https://img.atcoder.jp/abc406/6f17e951940c2460b3ae5fe8e6bddc52.png)

对于第 $2$ 个查询，将顶点 $1$ 的权重增加 $3$。

对于第 $3$ 个查询，考虑删除边 $1$。包含顶点 $1$ 的子树的权重为 $5$，包含顶点 $2$ 的子树的权重为 $4$，因此输出它们的差 $1$。（下图左）

对于第 $4$ 个查询，将顶点 $4$ 的权重增加 $10$。

对于第 $5$ 个查询，考虑删除边 $5$。此时，树会分裂成包含顶点 $4$ 的子树和仅包含顶点 $6$ 的子树。包含顶点 $4$ 的子树的权重为 $18$，仅包含顶点 $6$ 的子树的权重为 $1$，因此输出它们的差 $17$。（下图右）

![](https://img.atcoder.jp/abc406/c5eacf2967bcc2b09866a0d8b83104c4.png)

因此，按顺序换行输出第二种类型查询的答案 $2, 1, 17$。