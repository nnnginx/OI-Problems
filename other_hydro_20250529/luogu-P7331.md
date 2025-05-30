## 题目背景
[Link](https://youtu.be/tylNqtyj0gs?t=2388)

*I have gone over the scenarios in my head,*

*and there are 6.96969 billion outcomes, and only one of them -*

*- do I win.*

## 题目描述
Dream abstracts the fabric of spacetime as a directed rooted tree (arborescence) with $N$ nodes (numbered $1$ through $N$). Node $1$ is the root and for each $i$ ($1 \le i \le N-1$), the parent of node $i+1$ is $f_i$. All edges of this tree are directed away from the root.

Then, Dream employs a magical superpower and adds $M$ directed edges to this tree in such a way that the resulting directed graph remains acyclic (a DAG).

Let's call a node of this DAG an *event* and further call a simple path on this DAG an *era*. Dream considers a pair of events $(i,j)$ to be *plausible* if there is an era whose first event is $i$ and last event is $j$. Note that $i \lt j$ does not have to hold for a plausible pair.

Dream now wants you to answer $Q$ queries. In each query, he gives you two positive integers $l$ and $r$, where $l \leq r$, and he wishes to know the number of plausible pairs of events $(i,j)$ such that $l \leq i \lt j \leq r$.

## 输入格式
The first line of the input contains two space-separated integers $N$ and $M$.

The second line contains $N-1$ space-separated integers $f_1, f_2, \ldots, f_{N-1}$.

$M$ lines follow. Each of these lines contains two space-separated integers $u$ and $v$ describing an additional edge from node $u$ to node $v$.

The following line contains a single integer $Q$.

$Q$ lines follow. Each of these lines contains two space-separated integers $l$ and $r$ describing a query.

## 输出格式
For each query, print a single line containing one integer ― the number of plausible pairs $(i,j)$ such that $l \leq i \lt j \leq r$.

```input1
8 2
1 2 5 1 4 3 3
2 4
4 7
3
4 6
5 7
1 8
```

```output1
2
2
18
```

## 提示
 - $2 \leq N \leq 7 \cdot 10^5$
 - $1 \leq Q \leq 7 \cdot 10^5$
 - $0 \leq M \leq 20$
 - $1 \le f_i \le N$ for each valid $i$
 - $1 \le u, v \le N$
 - the graph described on the input is acyclic
 - $1 \le l \le r \le N$

### Subtasks

**Subtask #1 (17 points):** $N,Q\le3\cdot 10^5$

**Subtask #2 (83 points):** original constraints


