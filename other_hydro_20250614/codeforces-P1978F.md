## Description

<div><p>Given an array $a$ of length $n$. Let's construct a square matrix $b$ of size $n \times n$, in which the $i$-th row contains the array $a$ cyclically shifted to the right by $(i - 1)$. For example, for the array $a = [3, 4, 5]$, the obtained matrix is</p><p>$$b = \begin{bmatrix} 3 &amp; 4 &amp; 5 \\ 5 &amp; 3 &amp; 4 \\ 4 &amp; 5 &amp; 3 \end{bmatrix}$$</p><p>Let's construct the following graph:</p><ul> <li> The graph contains $n^2$ vertices, each of which corresponds to one of the elements of the matrix. Let's denote the vertex corresponding to the element $b_{i, j}$ as $(i, j)$.</li><li> We will draw an edge between vertices $(i_1, j_1)$ and $(i_2, j_2)$ if $|i_1 - i_2| + |j_1 - j_2| \le k$ and $\gcd(b_{i_1, j_1}, b_{i_2, j_2}) &gt; 1$, where $\gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> of integers $x$ and $y$. </li></ul><p>Your task is to calculate the number of connected components$^{\dagger}$ in the obtained graph.</p><p>$^{\dagger}$A connected component of a graph is a set of vertices in which any vertex is reachable from any other via edges, and adding any other vertex to the set violates this rule.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le n \le 10^6$, $2 \le k \le 2 \cdot 10^6$) ！ the length of the array and the parameter $k$. </p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$) ！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output a single integer ！ the number of connected components in the obtained graph.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le n \le 10^6$, $2 \le k \le 2 \cdot 10^6$) ！ the length of the array and the parameter $k$. </p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$) ！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output a single integer ！ the number of connected components in the obtained graph.</p>





```input1|2,3,6,7,10,11
6
3 3
3 4 5
3 3
3 4 9
3 2
3 4 9
2 2
2 8
5 3
8 27 5 4 3
4 10
2 2 2 2
```




```output1
3
2
3
1
4
1
```



## Note

<p>In the first test case, the matrix $b$ is given in the statement. The first connected component contains the vertices $(1, 1)$, $(2, 2)$, and $(3, 3)$. The second connected component contains the vertices $(1, 2)$, $(2, 3)$, and $(3, 1)$. The third connected component contains the vertices $(1, 3)$, $(2, 1)$, and $(3, 2)$. Thus, the graph has $3$ connected components.</p><p>In the second test case, the following matrix is obtained:</p><p>$$b = \begin{bmatrix} 3 &amp; 4 &amp; 9 \\ 9 &amp; 3 &amp; 4 \\ 4 &amp; 9 &amp; 3 \end{bmatrix}$$</p><p>The first connected component contains all vertices corresponding to elements with values $3$ and $9$. The second connected component contains all vertices corresponding to elements with the value $4$.</p><p>In the fourth test case, all vertices are in one connected component.</p>
