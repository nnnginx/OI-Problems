## Description

<div><p>You are given an array $a_1, a_2, \ldots, a_n$. Find the number of tuples ($x, y, z$) such that: </p><ul> <li> $1 \leq x \leq y \leq z \leq n$, and </li><li> $f(x, y) \oplus f(y, z) &gt; f(x, z)$. </li></ul><p>We define $f(l, r) = a_l \oplus a_{l + 1} \oplus \ldots \oplus a_{r}$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer on a new line&nbsp;！ the number of described tuples.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer on a new line&nbsp;！ the number of described tuples.</p>





```input1|2,3,6,7
3
3
6 2 4
1
3
5
7 3 7 2 1
```




```output1
4
0
16
```



## Note

<p>In the first case, there are 4 such tuples in the array $[6, 2, 4]$: </p><ul> <li> ($1$, $2$, $2$): $(a_1 \oplus a_2) \oplus (a_2) = 4 \oplus 2 &gt; (a_1 \oplus a_2) = 4$ </li><li> ($1$, $1$, $3$): $(a_1) \oplus (a_1 \oplus a_2 \oplus a_3) = 6 \oplus 0 &gt; (a_1 \oplus a_2 \oplus a_3) = 0$ </li><li> ($1$, $2$, $3$): $(a_1 \oplus a_2) \oplus (a_2 \oplus a_3) = 4 \oplus 6 &gt; (a_1 \oplus a_2 \oplus a_3) = 0$ </li><li> ($1$, $3$, $3$): $(a_1 \oplus a_2 \oplus a_3) \oplus (a_3) = 0 \oplus 4 &gt; (a_1 \oplus a_2 \oplus a_3) = 0$ </li></ul><p>In the second test case, there are no such tuples.</p>
