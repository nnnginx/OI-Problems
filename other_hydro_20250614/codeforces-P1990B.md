## Description

<div><p>For an array $b$ of size $m$, we define:</p><ul><li> the <span class="tex-font-style-bf">maximum prefix position</span> of $b$ is the <span class="tex-font-style-bf">smallest</span> index $i$ that satisfies $b_1+\ldots+b_i=\max_{j=1}^{m}(b_1+\ldots+b_j)$;</li><li> the <span class="tex-font-style-bf">maximum suffix position</span> of $b$ is the <span class="tex-font-style-bf">largest</span> index $i$ that satisfies $b_i+\ldots+b_m=\max_{j=1}^{m}(b_j+\ldots+b_m)$.</li></ul><p>You are given three integers $n$, $x$, and $y$ ($x &gt; y$). Construct an array $a$ of size $n$ satisfying:</p><ul><li> $a_i$ is either $1$ or $-1$ for all $1 \le i \le n$;</li><li> the <span class="tex-font-style-bf">maximum prefix position</span> of $a$ is $x$;</li><li> the <span class="tex-font-style-bf">maximum suffix position</span> of $a$ is $y$.</li></ul><p>If there are multiple arrays that meet the conditions, print any. It can be proven that such an array always exists under the given conditions.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¡ª the number of test cases.</p><p>For each test case: </p><ul> <li> The only line contains three integers $n$, $x$, and $y$ ($2 \leq n \leq 10^5, 1 \le y \lt x \le n)$. </li></ul><p>It is guaranteed that the sum of $n$ over all test cases will not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ space-separated integers $a_1, a_2, \ldots, a_n$ in a new line.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¡ª the number of test cases.</p><p>For each test case: </p><ul> <li> The only line contains three integers $n$, $x$, and $y$ ($2 \leq n \leq 10^5, 1 \le y \lt x \le n)$. </li></ul><p>It is guaranteed that the sum of $n$ over all test cases will not exceed $10^5$.</p>

## Output

<p>For each test case, output $n$ space-separated integers $a_1, a_2, \ldots, a_n$ in a new line.</p>





```input1|2,4
3
2 2 1
4 4 3
6 5 1
```




```output1
1 1
1 -1 1 1
1 1 -1 1 1 -1
```



## Note

<p>In the second test case, </p><ul><li> $i=x=4$ is the <span class="tex-font-style-bf">smallest</span> index that satisfies $a_1+\ldots +a_i=\max_{j=1}^{n}(a_1+\ldots+a_j)=2$;</li><li> $i=y=3$ is the <span class="tex-font-style-bf">greatest</span> index that satisfies $a_i+\ldots +a_n=\max_{j=1}^{n}(a_j+\ldots+a_n)=2$.</li></ul><p>Thus, the array $a=[1,-1,1,1]$ is considered correct.</p>
