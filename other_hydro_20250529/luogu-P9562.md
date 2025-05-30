## 题目描述
Given an integer sequence $a_1, a_2, \cdots, a_n$ of length $n$, we construct an undirected graph $G$ from the sequence. More precisely, for all $1 \le i < j \le n$, if $i - j = a_i - a_j$, there will be an undirected edge in $G$ connecting vertices $i$ and $j$. The weight of the edge is $(a_i + a_j)$.

Find a matching of $G$ so that the sum of weight of all edges in the matching is maximized, and output this maximized sum.

Recall that a matching of an undirected graph means that we choose some edges from the graph such that any two edges have no common vertices. Specifically, not choosing any edge is also a matching.

## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($2 \le n \le 10^5$) indicating the length of the sequence.

The second line contains $n$ integers $a_1, a_2, \cdots, a_n$ ($-10^9 \le a_i \le 10^9$) indicating the sequence.

It's guaranteed that the sum of $n$ of all test cases will not exceed $5 \times 10^5$.

## 输出格式
For each test case output one line containing one integer indicating the maximum sum of weight of all edges in a matching.

## 题目大意
**【题目描述】**

给定长度为 $n$ 的整数序列 $a_1, a_2, \cdots, a_n$，我们将从该序列中构造出一张无向图 $G$。具体来说，对于所有 $1 \le i < j \le n$，若 $i - j = a_i - a_j$，则 $G$ 中将存在一条连接节点 $i$ 与 $j$ 的无向边，其边权为 $(a_i + a_j)$。

求 $G$ 的一个匹配，使得该匹配中所有边的边权之和最大，并输出最大边权之和。

请回忆：无向图的匹配，指的是从该无向图中选出一些边，使得任意两条边都没有公共的节点。特别地，不选任何边也是一个匹配。

**【输入格式】**

有多组测试数据。第一行输入一个整数 $T$ 表示测试数据组数。对于每组测试数据：

第一行输入一个整数 $n$（$2 \le n \le 10^5$）表示序列的长度。

第二行输入 $n$ 个整数 $a_1, a_2, \cdots, a_n$（$-10^9 \le a_i \le 10^9$）表示序列。

保证所有数据中 $n$ 之和不超过 $5 \times 10^5$。

**【输出格式】**

每组数据输出一行一个整数，表示匹配的最大边权之和。

**【样例解释】**

对于第一组样例数据，最优方案是选择连接节点 $3$ 和 $5$，节点 $4$ 和 $7$，以及节点 $8$ 和 $9$ 的三条边，边权之和为 $(5 + 7) + (6 + 9) + (1 + 2) = 30$。

对于第二组样例数据，由于每条边的边权都是负数，因此最优匹配不应该选择任何边，答案为 $0$。

对于第三组样例数据，由于图中不存在任何边，因此答案为 $0$。

```input1
3
9
3 -5 5 6 7 -1 9 1 2
3
-5 -4 -3
3
1 10 100

```

```output1
30
0
0

```

## 提示
For the first sample test case, the optimal choice is to choose the three edges connecting vertex $3$ and $5$, vertex $4$ and $7$, and finally vertex $8$ and $9$. The sum of weight is $(5 + 7) + (6 + 9) + (1 + 2) = 30$.

For the second sample test case, as all edges have negative weights, the optimal matching should not choose any edge. The answer is $0$.

For the third sample test case, as there is no edge in the graph, the answer is $0$.

