## Description

<div><p>In 2077, after the world was enslaved by robots, the robots decided to implement an educational reform, and now the operation of taking the modulus is only taught in the faculty of "Ancient World History". Here is one of the entrance tasks for this faculty:</p><p>We define the <span class="tex-font-style-tt">beauty</span> of an array of positive integers $b$ as the maximum $f(b_i, b_j)$ over all pairs $1 \leq i, j \leq n$, where $f(x, y) = (x \bmod y) + (y \bmod x)$.</p><p>Given an array of positive integers $a$ of length $n$, output $n$ numbers, where the $i$-th number ($1 \leq i \leq n$) is the <span class="tex-font-style-tt">beauty</span> of the array $a_1, a_2, \ldots, a_i$.</p><p>$x \bmod y$ is the remainder of the division of $x$ by $y$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^6$)&nbsp;！ the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers&nbsp;！ the beauties of all prefixes of the array $a$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^6$)&nbsp;！ the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output $n$ integers&nbsp;！ the beauties of all prefixes of the array $a$.</p>





```input1|2,3
2
5
3 1 4 1 5
7
5 11 11 4 2 1 10
```




```output1
0 1 4 4 5 
0 6 6 7 7 7 11
```



## Note

<p>The beauty of the array $3$ is $0$.</p><p>The beauty of the array $3, 1$ is $f(3, 1) = 1$.</p><p>The beauty of the array $3, 1, 4$ is $f(3, 4) = 4$.</p><p>The beauty of the array $3, 1, 4, 1$ is $f(4, 3) = 4$.</p><p>The beauty of the array $3, 1, 4, 1, 5$ is $f(4, 5) = 5$.</p>
