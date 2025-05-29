## 题目描述
Caroline asked you for help in solving a cactus problem one year ago. During the last year, she researched extensively about cactuses. Today, she is the one presenting the problem.

You are given a $\textbf{cactus without bridges}$ and also the length of each odd simple cycle is greater than or equal to the number of odd simple cycles in cactus. Your task is to answer whether it's possible to label the cactus edges with positive integers such that the following conditions are satisfied:

- Let's define the maximum label with $t$. All the integers $1$, $2$, $\ldots$, $t$ are used in labeling (note that you do not need to minimize or maximize the value of $t$);
- For each vertex $v$ of the given cactus, the labels of edges incident to the vertex $v$ should be different and should form an interval of consecutive integers.

An edge in the graph is called $\textit{bridge}$ if the deletion of that edge increases the number of connected components of the graph. A $\textit{cactus}$ is a connected undirected graph in which every edge lies on at most one simple cycle. Intuitively, a cactus is a generalization of a tree where some cycles are allowed. Multiedges (multiple edges between a pair of vertices) and loops (edges that connect a vertex to itself) are not allowed in a cactus.

## 输入格式
The first line contains two integers $n$ and $m$ ($3 \le n \le 10^5$, $n \le m \le \lfloor \frac{3(n - 1)}{2} \rfloor$) --- the number of vertices and edges in the cactus. Each of the next $m$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$; $u \ne v$) --- the edges of the cactus. The given cactus satisfies all constraints from the problem statement.

## 输出格式
If finding the labeling satisfying the problem's conditions is impossible, output the single line with the word $\tt{NO}$.
Otherwise, in the first line output the single word $\tt{YES}$. In the second line output an integer $t$ ($1 \leq t \leq m$) --- the number of different labels. In the third line output should contain $m$ integers $c_i$ ($1 \leq i \leq m$, $1 \leq c_i \leq t$) --- the labels of the edges.

```input1
5 5
1 2
2 3
3 4
4 5
5 1
```

```output1
NO
```

```input2
8 10
1 2
2 3
1 3
1 4
1 5
4 5
5 6
6 7
7 8
8 5
```

```output2
YES
4
1 2 3 2 4 3 1 2 3 2
```

