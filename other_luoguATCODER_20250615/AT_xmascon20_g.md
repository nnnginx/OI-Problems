# AT_xmascon20_g Graph Products

## 题目描述

在这个问题中，我们只考虑无向简单图。给定图 $H$ 和 $H'$，定义 $H \mathbin{\square} H'$ 和 $H \times H'$ 如下。假设 $H$ 和 $H'$ 的顶点集合分别为 $V(H)$ 和 $V(H')$。令 $W = V(H) \times V(H')$（即所有「$H$ 的一个顶点与 $H'$ 的一个顶点组合」的集合）。

对于 $H \mathbin{\square} H'$，其顶点集合为 $W$。在这个图中，顶点 $(u, u') \in W$ 与顶点 $(v, v') \in W$ 之间有边相连，当且仅当满足以下条件之一：

- $u = v$，并且在 $H'$ 中，顶点 $u'$ 与顶点 $v'$ 之间有边。
- $u' = v'$，并且在 $H$ 中，顶点 $u$ 与顶点 $v$ 之间有边。

而对于 $H \times H'$，顶点集合同样是 $W$。在这个图中，顶点 $(u, u') \in W$ 与顶点 $(v, v') \in W$ 之间有边相连，当且仅当在 $H$ 中顶点 $u$ 与顶点 $v$ 之间有边，并且在 $H'$ 中顶点 $u'$ 与顶点 $v'$ 之间有边。

你将得到 $K$ 个图 $G_1, \ldots, G_K$。每个图 $G_k$ ($1 \le k \le K$) 的顶点集合为 $\{1, \ldots, N_k\}$，有 $M_k$ 条边，第 $i$ 条边连接的是顶点 $A_{k,i}$ 和 $B_{k,i}$。

对于每对图 $G_k$ 和 $G_{k'}$ ($1 \le k \le K$，$1 \le k' \le K$)，判断 $G_k \mathbin{\square} G_{k'}$ 和 $G_k \times G_{k'}$ 是否同构。也就是说，是否存在一个双射 $f: V(G_k) \times V(G_{k'}) \to V(G_k) \times V(G_{k'})$，使得对于任意 $(u, u')$ 和 $(v, v')$ 有「$G_k \mathbin{\square} G_{k'}$ 中 $(u, u')$ 和 $(v, v')$ 有边」等价于「$G_k \times G_{k'}$ 中 $f((u, u'))$ 和 $f((v, v'))$ 有边」。

## 输入格式

输入格式如下：

> $K$  
> $N_1$ $M_1$  
> $A_{1,1}$ $B_{1,1}$  
> $\vdots$  
> $A_{1,M_1}$ $B_{1,M_1}$  
> $\vdots$  
> $N_K$ $M_K$  
> $A_{K,1}$ $B_{K,1}$  
> $\vdots$  
> $A_{K,M_K}$ $B_{K,M_K}$

## 输出格式

输出共 $K$ 行，每行有 $K$ 个字符。第 $k$ 行 ($1 \le k \le K$) 的第 $k'$ 个字符为 `1`，如果 $G_k \mathbin{\square} G_{k'}$ 和 $G_k \times G_{k'}$ 是同构的；否则为 `0`。

## 输入输出样例 #1

### 输入 #1

```
5
3
2
1 2
2 3
4
3
1 2
2 3
3 4
5
5
1 2
1 3
2 4
3 5
2 3
8
6
1 2
5 8
1 6
4 8
2 7
6 7
6
9
1 3
3 5
1 5
1 2
2 3
3 4
4 5
5 6
1 6
```

### 输出 #1

```
00000
00000
00000
00000
00000
```

## 说明/提示

- $1 \le K \le 10$。
- $1 \le N_k \le 25000$ ($1 \le k \le K$)。
- $0 \le M_k \le 25000$ ($1 \le k \le K$)。
- $1 \le A_{k,i} < B_{k,i} \le N_k$ ($1 \le k \le K$，$1 \le i \le M_k$)。
- 对于每个 $1 \le k \le K$，所有的 $(A_{k,i}, B_{k,i})$ 都是不同的。

 **本翻译由 AI 自动生成**