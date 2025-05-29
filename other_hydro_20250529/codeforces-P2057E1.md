## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between the versions is that in this version, there is an additional constraint on $m$. You can hack only if you solved all versions of this problem.</span> </p><p>Recently, the instructors of "T-generation" needed to create a training contest. They were missing one problem, and there was not a single problem on graphs in the contest, so they came up with the following problem.</p><p>You are given a connected weighted undirected graph with $n$ vertices and $m$ edges, which does not contain self-loops or multiple edges.</p><p>There are $q$ queries of the form $(a, b, k)$: among all paths from vertex $a$ to vertex $b$, find the smallest $k$-th maximum weight of edges on the path$^{\dagger}$.</p><p>The instructors thought that the problem sounded very interesting, but there is one catch. They do not know how to solve it. Help them and solve the problem, as there are only a few hours left until the contest starts.</p><p>$^{\dagger}$ Let $w_1 \ge w_2 \ge \ldots \ge w_{h}$ be the weights of all edges in a path, in non-increasing order. The $k$-th maximum weight of the edges on this path is $w_{k}$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each set of test case contains three integers $n, m$ and $q$ ($2 \le n \le 400$, $n - 1 \le m \le \operatorname{min}(\mathbf{400}, \frac{n \cdot (n - 1)}{2})$, $1 \le q \le 3 \cdot 10^5$)&nbsp;！ the number of vertices, the number of edges, and the number of questions, respectively.</p><p>Each of the following $m$ lines of each set of test case contains three integers $v, u$ and $w$ ($1 \le v, u \le n$, $1 \le w \le 10^9$)&nbsp;！ the ends of the next edge of the graph and its weight, respectively. It is guaranteed that the graph does not contain self-loops and multiple edges.</p><p>Each of the following $q$ lines of each set of test case contains three integers $a, b$ and $k$ ($1 \le a, b \le n$, $k \ge 1$)&nbsp;！ the next question. It is guaranteed that any path from vertex $a$ to vertex $b$ contains at least $k$ edges.</p><p>It is guaranteed that the sum of the values of $n$ across all sets of test cases does not exceed $400$.</p><p>It is guaranteed that the sum of the values of $m$ across all sets of test cases does not exceed $400$.</p><p>It is guaranteed that the sum of the values of $q$ across all sets of test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the answers to all questions.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each set of test case contains three integers $n, m$ and $q$ ($2 \le n \le 400$, $n - 1 \le m \le \operatorname{min}(\mathbf{400}, \frac{n \cdot (n - 1)}{2})$, $1 \le q \le 3 \cdot 10^5$)&nbsp;！ the number of vertices, the number of edges, and the number of questions, respectively.</p><p>Each of the following $m$ lines of each set of test case contains three integers $v, u$ and $w$ ($1 \le v, u \le n$, $1 \le w \le 10^9$)&nbsp;！ the ends of the next edge of the graph and its weight, respectively. It is guaranteed that the graph does not contain self-loops and multiple edges.</p><p>Each of the following $q$ lines of each set of test case contains three integers $a, b$ and $k$ ($1 \le a, b \le n$, $k \ge 1$)&nbsp;！ the next question. It is guaranteed that any path from vertex $a$ to vertex $b$ contains at least $k$ edges.</p><p>It is guaranteed that the sum of the values of $n$ across all sets of test cases does not exceed $400$.</p><p>It is guaranteed that the sum of the values of $m$ across all sets of test cases does not exceed $400$.</p><p>It is guaranteed that the sum of the values of $q$ across all sets of test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output the answers to all questions.</p>





```input1|2,3,4,5,6,7,8,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47
3
4 4 2
1 2 2
2 4 2
1 3 4
3 4 1
1 4 2
2 3 1
6 7 3
1 2 10
2 3 3
3 4 9
4 5 2
5 6 1
2 4 10
4 6 10
1 6 3
1 6 2
2 4 1
11 17 10
1 4 5
1 3 19
1 2 10
3 2 13
4 5 1
4 6 11
3 5 9
3 6 18
2 7 17
5 8 15
5 10 8
6 9 4
7 10 20
7 8 16
8 11 3
9 11 6
10 11 14
3 11 1
3 11 3
1 11 1
1 11 4
1 11 3
8 2 2
10 4 1
3 9 2
3 9 1
6 7 3
```




```output1
1 2
2 9 9
11 3 11 1 3 10 8 4 11 4
```



## Note

<p>In the first set of test cases, one of the optimal paths in the first query is the path $1 \rightarrow 3 \rightarrow 4$; the $2$-nd maximum weight of the edges on this path is $1$. In the second query, one of the optimal paths is $2 \rightarrow 4 \rightarrow 3$; $1$-st maximum weight of the edges is $2$.</p><p>In the second set of input data, one of the optimal paths in the first query is the path $1 \rightarrow 2 \rightarrow 4 \rightarrow 5 \rightarrow 6$; the $3$-rd maximum weight of the edges on this path is $2$.</p>
