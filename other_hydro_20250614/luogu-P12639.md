## 题目描述
You are given a tree with $n$ vertices, numbered from $1$ to $n$. The root of the tree is the vertex with number $1$. For each $v$ from $2$ to $n$, let's define $p_v$ as the number of the vertex adjacent to $v$ that lies on the simple path between vertex $v$ and the root. Each edge $(p_v, v)$ is labeled with the symbol $\tt{<}$ or $\tt{>}$.

Find the number of ways to place the numbers from $1$ to $n$ in the vertices of the tree, such that each number is used exactly once and all the relationships indicated on the edges are satisfied. That is, for all edges with the symbol $\tt{<}$, $a[p_v] < a[v]$ should hold, and for all edges with the symbol $\tt{>}$, $a[p_v] > a[v]$ should hold.

Since the answer can be very large, output it modulo $10^9 + 7$.

## 输入格式
The first line contains a single integer $n$ ($1 \leq n \leq 3\,000$) - the number of vertices in the tree.

Each of the next $n-1$ lines contains a single integer $p_i$ ($1 \leq p_i < i$) and a character $c_i$ ($c_i \in \{\tt{<}, \tt{>}\}$), indicating that the edge between vertices with indices $p_i$ and $i$ is labeled with the symbol $c_i$. Note that the indexing starts from $2$.

## 输出格式
Output a single integer - the number of ways to arrange all numbers from $1$ to $n$ in the vertices of the tree such that all the relationships indicated on the edges are satisfied. Note that you should output the remainder of the division by $10^9 + 7$, not the actual answer.

```input1
4
1 <
2 <
3 >
```

```output1
3
```

```input2
4
1 <
1 <
1 <
```

```output2
6
```

```input3
5
1 <
1 <
3 >
3 >
```

```output3
18
```

## 提示
- ($8$ points) $n \leq 10$;
- ($6$ points) $n \leq 18$;
- ($10$ points) $c_i = \tt{<}$;
- ($4$ points) $p_i = 1$;
- ($13$ points) $p_i = i - 1, 1 \leq n \leq 200$;
- ($19$ points) $p_i = i - 1$;
- ($24$ points) $n \leq 200$;
- ($16$ points) no additional constraints.

