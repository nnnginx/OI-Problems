## Description

<div><p>You are given a complete graph with $n$ vertices, where the $i$-th vertex has a weight $p_i$. The weight of the edge connecting vertex $x$ and vertex $y$ is equal to $\operatorname{max}(p_x, p_y) \bmod \operatorname{min}(p_x, p_y)$.</p><p>Find the smallest total weight of a set of $n - 1$ edges that connect all $n$ vertices in this graph.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test contains an integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The next line of each test contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le 5 \cdot 10^5$).</p><p>The sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p><p>The sum of $\max(p_1,p_2,\ldots,p_n)$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;¡ª the weight of the minimum spanning tree.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test contains an integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The next line of each test contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le 5 \cdot 10^5$).</p><p>The sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p><p>The sum of $\max(p_1,p_2,\ldots,p_n)$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;¡ª the weight of the minimum spanning tree.</p>





```input1|2,3,6,7
4
5
4 3 3 4 4
10
2 10 3 2 9 9 4 6 4 6
12
33 56 48 41 89 73 99 150 55 100 111 130
7
11 45 14 19 19 8 10
```




```output1
1
0
44
10
```



## Note

<p>In the first test case, one of the possible ways to connect the edges is to draw the edges $(1, 2)$, $(1, 4)$, $(1, 5)$, $(2, 3)$. The weight of the first edge is $\operatorname{max}(p_1, p_2) \bmod \operatorname{min}(p_1, p_2)=4 \bmod 3 = 1$, and the weights of all other edges are $0$.</p>
