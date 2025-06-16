## Description

<div><p>Sadly, Dora poured the paint when painting the class mural. Dora considers the mural as the matrix $b$ of size $n \times n$. Initially, $b_{i,j} = 0$ for all $1 \le i, j \le n$.</p><p>Dora has only two brushes which have two different colors. In one operation, she can paint the matrix with one of two brushes:</p><ul> <li> The first brush has color $1$ on it and can paint one column of the matrix. That is, Dora chooses $1 \leq j \leq n$ and makes $b_{i,j} := 1$ for all $1 \leq i \leq n$; </li><li> The second brush has color $2$ on it and can paint one row of the matrix. That is, Dora chooses $1 \leq i \leq n$ and makes $b_{i,j} := 2$ for all $1 \leq j \leq n$. </li></ul><p>Dora paints the matrix so that the resulting matrix $b$ <span class="tex-font-style-bf">contains only</span> $1$ and $2$.</p><p>For a matrix $b$, let $f(b)$ denote the minimum number of operations needed to turn the initial matrix (containing only $0$) into $b$. The <span class="tex-font-style-it">beauty</span> of a matrix $b$ is the number of ways to paint the initial matrix in exactly $f(b)$ operations to turn it into $b$. If there's no way to turn the initial matrix into $b$, the beauty of $b$ is $0$.</p><p>However, Dora made a uniformly random mistake; there's <span class="tex-font-style-bf">exactly one</span> element different in the matrix $a$ given to you from the real matrix $b$. That is, there is exactly one pair $(i, j)$ such that $a_{i, j} = 3 - b_{i, j}$.</p><p>Please help Dora compute the expected beauty of the real matrix $b$ modulo $998\,244\,353$ (all possible $n^2$ mistakes have equal probability).</p><p>Since the size of the matrix is too large, Dora will only tell you the positions of $m$ elements of color $1$, and the remaining $n^2-m$ elements have color $2$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 2 \cdot 10^5$, $0 \leq m \leq \min(10^6, n^2)$)&nbsp;！ the size of the matrix and the number of elements of color $1$.</p><p>Then $m$ lines follow, each containing two positive integers $x_i$ and $y_i$ ($1 \leq x_i, y_i \leq n$)&nbsp;！ denoting that $a_{x_i, y_i} = 1$.</p><p>It is guaranteed that if $i \neq j$, then $(x_i, y_i) \neq (x_j, y_j)$.</p><p>It is also guaranteed that the sum of $n$ over all test cases does not exceed $4\cdot10^5$, and the sum of $m$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output a single integer ！ the expected beauty of the real matrix $b$, modulo $998\,244\,353$.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 2 \cdot 10^5$, $0 \leq m \leq \min(10^6, n^2)$)&nbsp;！ the size of the matrix and the number of elements of color $1$.</p><p>Then $m$ lines follow, each containing two positive integers $x_i$ and $y_i$ ($1 \leq x_i, y_i \leq n$)&nbsp;！ denoting that $a_{x_i, y_i} = 1$.</p><p>It is guaranteed that if $i \neq j$, then $(x_i, y_i) \neq (x_j, y_j)$.</p><p>It is also guaranteed that the sum of $n$ over all test cases does not exceed $4\cdot10^5$, and the sum of $m$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output a single integer ！ the expected beauty of the real matrix $b$, modulo $998\,244\,353$.</p>





```input1|2,3,4,7,8,9,11,12,13,14,15,16,17,18,19,20,21,28,29,30,31
7
2 2
1 1
1 2
2 1
1 1
3 2
1 1
3 3
6 0
5 10
1 1
1 2
1 3
2 1
2 3
5 1
5 2
5 3
5 4
5 5
3 5
1 1
1 3
2 2
3 1
3 3
4 3
1 1
2 3
2 4
```




```output1
1
499122178
665496236
120
79859554
776412275
1
```



## Note

<p>In the first test case, the matrix $a = \left[\begin{matrix}1&amp;1\\2&amp;2\end{matrix}\right]$. Let's consider changing the element $(1,1)$ to calculate the answer.</p><p>It can be proved that the minimum steps to paint the initial matrix into $\left[\begin{matrix}2&amp;1\\2&amp;2\end{matrix}\right]$ is $3$. We can first paint the first row into color $2$, then paint the second column into color $1$, and finally paint the second row into color $2$. The process is listed below:</p><p>$$\left[\begin{matrix}0&amp;0\\0&amp;0\end{matrix}\right]\Rightarrow\left[\begin{matrix}2&amp;2\\0&amp;0\end{matrix}\right]\Rightarrow\left[\begin{matrix}2&amp;1\\0&amp;1\end{matrix}\right]\Rightarrow\left[\begin{matrix}2&amp;1\\2&amp;2\end{matrix}\right]$$</p><p>It can be proved that this is the only way to paint the matrix in $3$ steps. So the beauty of the matrix $\left[\begin{matrix}2&amp;1\\2&amp;2\end{matrix}\right]$ is $1$. Similarly, if any other element of the matrix is changed, the beauty is always $1$, so the expected beauty of the real matrix $b$ is $1$.</p><p>In the second test case, the matrix $a = \left[\begin{matrix}1&amp;2\\2&amp;2\end{matrix}\right]$. Let's consider changing the element $(2, 2)$ to calculate the answer.</p><p>It can be proven that it's impossible to paint the initial matrix into $\left[\begin{matrix}1&amp;2\\2&amp;1\end{matrix}\right]$, so its beauty is $0$. If any other element of the matrix is changed, the beauty is always $2$, so the expected beauty is $\frac{0 + 2 + 2 + 2}{4} = \frac{6}{4} \equiv 499\,122\,178 \pmod {998\,244\,353}$.</p>
