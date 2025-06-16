## Description

<div><p>You are given an undirected connected weighted graph. Define the cost of a path of length $k$ to be as follows:</p><ul> <li> Let the weights of all the edges on the path be $w_1,...,w_k$. </li><li> The cost of the path is $(\min_{i = 1}^{k}{w_i}) + (\max_{i=1}^{k}{w_i})$, or in other words, the maximum edge weight + the minimum edge weight. </li></ul><p>Across all paths from vertex $1$ to $n$, report the cost of the path with minimum cost. Note that the path is not necessarily simple.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;¡ª the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5, n - 1 \le m \le \min(2 \cdot 10^5, \frac{n(n - 1)}{2})$).</p><p>The next $m$ lines each contain integers $u, v$ and $w$ ($1 \le u, v \le n, 1 \le w \le 10^9$) representing an edge from vertex $u$ to $v$ with weight $w$. It is guaranteed that the graph does not contain self-loops or multiple edges and the resulting graph is connected.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and that the sum of $m$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer, the minimum cost path from vertex $1$ to $n$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;¡ª the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5, n - 1 \le m \le \min(2 \cdot 10^5, \frac{n(n - 1)}{2})$).</p><p>The next $m$ lines each contain integers $u, v$ and $w$ ($1 \le u, v \le n, 1 \le w \le 10^9$) representing an edge from vertex $u$ to $v$ with weight $w$. It is guaranteed that the graph does not contain self-loops or multiple edges and the resulting graph is connected.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and that the sum of $m$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer, the minimum cost path from vertex $1$ to $n$.</p>





```input1|2,3,4,8,9,10,11,12,13,14,15,16,17
4
3 2
1 2 1
2 3 1
3 2
1 3 13
1 2 5
8 9
1 2 6
2 3 5
3 8 6
1 4 7
4 5 4
5 8 7
1 6 5
6 7 5
7 8 5
3 3
1 3 9
1 2 8
2 3 3
```




```output1
2
18
10
11
```



## Note

<p>For the second test case, the optimal path is $1 \rightarrow 2 \rightarrow 1 \rightarrow 3$, the edge weights are $5, 5, 13$ so the cost is $\min(5, 5, 13) + \max(5, 5, 13) = 5 + 13 = 18$. It can be proven that there is no path with lower cost.</p>
