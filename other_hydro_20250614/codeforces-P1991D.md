## Description

<div><p>You are given an undirected graph with $n$ vertices, numbered from $1$ to $n$. There is an edge between vertices $u$ and $v$ if and only if $u \oplus v$ is a <a href="https://en.wikipedia.org/wiki/Prime_number">prime number</a>, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operator</a>.</p><p>Color all vertices of the graph using the minimum number of colors, such that no two vertices directly connected by an edge have the same color.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of test cases follows.</p><p>The only line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of vertices in the graph.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output two lines.</p><p>The first line should contain a single integer $k$ ($1 \le k \le n$)&nbsp;！ the minimum number of colors required.</p><p>The second line should contain $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le k$)&nbsp;！ the color of each vertex.</p><p>If there are multiple solutions, output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of test cases follows.</p><p>The only line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of vertices in the graph.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output two lines.</p><p>The first line should contain a single integer $k$ ($1 \le k \le n$)&nbsp;！ the minimum number of colors required.</p><p>The second line should contain $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le k$)&nbsp;！ the color of each vertex.</p><p>If there are multiple solutions, output any of them.</p>





```input1|2,4,6
6
1
2
3
4
5
6
```




```output1
1
1
2
1 2
2
1 2 2
3
1 2 2 3
3
1 2 2 3 3
4
1 2 2 3 3 4
```



## Note

<p>In the first test case, the minimum number of colors is $1$, because there is only one vertex.</p><p>In the second test case, the minimum number of colors is $2$, because there is an edge connecting $1$ and $2$ ($1 \oplus 2 = 3$, which is a prime number).</p><p>In the third test case, the minimum number of colors is still $2$, because $2$ and $3$ can be colored the same since there is no edge between $2$ and $3$ ($2 \oplus 3 = 1$, which is not a prime number).</p><p>In the fourth test case, it can be shown that the minimum number of colors is $3$.</p><p>In the fifth test case, it can be shown that the minimum number of colors is $3$.</p><p>In the sixth test case, it can be shown that the minimum number of colors is $4$.</p>
