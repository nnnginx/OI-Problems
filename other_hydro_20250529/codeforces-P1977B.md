## Description

<div><p>You are given a positive integer $x$. Find any array of integers $a_0, a_1, \ldots, a_{n-1}$ for which the following holds: </p><ul> <li> $1 \le n \le 32$, </li><li> $a_i$ is $1$, $0$, or $-1$ for all $0 \le i \le n - 1$, </li><li> $x = \displaystyle{\sum_{i=0}^{n - 1}{a_i \cdot 2^i}}$, </li><li> There does not exist an index $0 \le i \le n - 2$ such that both $a_{i} \neq 0$ and $a_{i + 1} \neq 0$. </li></ul><p>It can be proven that under the constraints of the problem, a valid array always exists.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single positive integer $x$ ($1 \le x &lt; 2^{30}$).</p></div><div class="output-specification"><p>For each test case, output two lines.</p><p>On the first line, output an integer $n$ ($1 \le n \le 32$)&nbsp;！ the length of the array $a_0, a_1, \ldots, a_{n-1}$.</p><p>On the second line, output the array $a_0, a_1, \ldots, a_{n-1}$.</p><p>If there are multiple valid arrays, you can output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single positive integer $x$ ($1 \le x &lt; 2^{30}$).</p>

## Output

<p>For each test case, output two lines.</p><p>On the first line, output an integer $n$ ($1 \le n \le 32$)&nbsp;！ the length of the array $a_0, a_1, \ldots, a_{n-1}$.</p><p>On the second line, output the array $a_0, a_1, \ldots, a_{n-1}$.</p><p>If there are multiple valid arrays, you can output any of them.</p>





```input1|2,4,6,8
7
1
14
24
15
27
11
19
```




```output1
1
1
5
0 -1 0 0 1
6
0 0 0 -1 0 1
5
-1 0 0 0 1
6
-1 0 -1 0 0 1
5
-1 0 -1 0 1
5
-1 0 1 0 1
```



## Note

<p>In the first test case, one valid array is $[1]$, since $(1) \cdot 2^0 = 1$.</p><p>In the second test case, one possible valid array is $[0,-1,0,0,1]$, since $(0) \cdot 2^0 + (-1) \cdot 2^1 + (0) \cdot 2^2 + (0) \cdot 2^3 + (1) \cdot 2^4 = -2 + 16 = 14$.</p>
