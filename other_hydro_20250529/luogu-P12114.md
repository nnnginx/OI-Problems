## 题目描述
Jacob is studying graph theory. Today he learned that a $\textit{topological ordering}$ of a directed graph is a linear ordering of its vertices such that for every directed edge $(u, v)$ from vertex $u$ to vertex $v$, $u$ comes before~$v$ in the ordering.

It is well-known that topological orderings exist only for graphs without cycles. But how do we generalize this concept for arbitrary graphs?

Jacob came up with the concept of a $\textit{half-topological ordering}$: a linear ordering of the graph's vertices such that $\textbf{for at least half}$ of all directed edges $(u, v)$ in the graph, $u$ comes before $v$ in the ordering.

In other words, if the graph has $m$ edges, and for a particular ordering, $k$ of them satisfy the condition above, then the ordering is called $\textit{half-topological}$ if $k \ge \lceil \frac{m}{2} \rceil$.

Help Jacob find any half-topological ordering of the given graph, or report that none exist.

## 输入格式
Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.

The first line of each test case contains two integers $n$ and $m$, denoting the number of vertices and the number of edges in the graph ($2 \le n \le 10^5$; $1 \le m \le 2 \cdot 10^5$).

The $i$-th of the following $m$ lines contains two integers $u_i$ and $v_i$, describing an edge from vertex $u_i$ to vertex $v_i$ ($1 \le u_i, v_i \le n$; $u_i \ne v_i$). The graph does not contain multiple edges: each directed edge $(u, v)$ appears at most once. However, having both edges $(u, v)$ and $(v, u)$ is allowed.

It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$, and the sum of $m$ over all test cases does not exceed $2 \cdot 10^5$.

## 输出格式
For each test case, print a single integer $-1$ if the required half-topological ordering does not exist.

Otherwise, print $n$ distinct integers $p_1, p_2, \ldots, p_n$, describing the ordering of the given graph ($1 \le p_i \le n$). For at least $\lceil \frac{m}{2} \rceil$ of the edges $(u_i, v_i)$, integer $u_i$ must come before integer $v_i$ in this list. If there are multiple answers, print any of them.

```input1
2
3 3
1 2
2 3
3 1
5 6
4 2
2 1
4 3
1 4
3 2
3 5
```

```output1
1 2 3
3 1 5 4 2
```

