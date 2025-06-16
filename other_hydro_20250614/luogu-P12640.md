## 题目描述
Given a tree with $n$ vertices and $n-1$ edges. It is necessary to add exactly $m$ new edges to this tree. Adding multiple edges or loops is prohibited. If the degree of a certain vertex was $t_i$ before adding edges, then after adding edges, its degree should not exceed $t_i + k$. It should be noted that the degree of a vertex is the number of edges connecting it to other vertices.

In addition, $m+n-1$ integers $a_1, a_2, \dots, a_{m+n-1}$ are given. After adding edges, it is necessary to assign each edge one of the elements of the array $a$ so that each element of the array corresponds to exactly one edge. The value $a_i$ assigned to the edge will denote its weight.

It is necessary to add new edges and assign numbers to the edges in such a way that the sum of the shortest distances between each pair of vertices is **maximized**. That is, it is necessary to maximize the function $\sum d_{ij}$, where $d_{ij}$ is the minimum distance between vertices, for all $i$ and $j$ ($1 \leq i < j \leq n$). The minimum distance between vertices is considered to be the sum of the weights of all edges on the simple path between them.

Please note that in this problem, you need to submit not the code, but the actual answers. You also have access to all the tests.

## 输入格式
There are $5$ tests.

The first line of each test contains three integers $n$, $m$, and $k$ ($1 \leq n \leq 5\,000$, $1 \leq m \leq 250\,000$, $1 \leq k \leq 500$) - the number of vertices in the tree, the number of edges to be added, and the maximum number of edges that can be added to one vertex.

The second line contains $m+n-1$ integers $a_1, a_2, \dots, a_{m+n-1}$ ($1 \leq a_i \leq 10^6$).

The next $n-1$ lines contain two integers each, $v_i$ and $u_i$ ($1 \leq v_i, u_i \leq n$) - the numbers of vertices connected by an edge. It is guaranteed that the initially given graph is a tree.

It is guaranteed that it is always possible to add edges in such a way that all the requirements described in the task are met.

## 输出格式
For each test, output the following:

If you have an answer for this test, output $1$, otherwise output $0$.

If you have an answer, then in each of the next $m+n-1$ lines, output three integers $v_i, u_i, a_i$ - the numbers of vertices connected by an edge in the final graph, and its weight.

## 提示
Let $d_0$ be a certain variable in the test, and $d$ be the sum of distances in your graph. If $d>d_0$, you will receive $20$ points for the test. Otherwise, you will receive as many points for the test as: $$(100^{(d-d_0)/d_0})^5 \cdot 20$$

If $s$ is the sum of points for all tests, then for the attempt you will receive $s$, rounded to the nearest integer.

