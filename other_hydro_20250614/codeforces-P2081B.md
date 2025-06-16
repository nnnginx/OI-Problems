## Description

<div><p>Ecrade has an integer array $a_1, a_2, \ldots, a_n$. It's guaranteed that for each $1 \le i &lt; n$, $a_i \neq a_{i+1}$.</p><p>Ecrade can perform several operations on the array to make it strictly increasing.</p><p>In each operation, he can choose two integers $l$ and $r$ ($1 \le l \le r \le n$) and replace $a_l, a_{l+1}, \ldots, a_r$ with any $r-l+1$ integers $a'_l, a'_{l+1}, \ldots, a'_r$ satisfying the following constraint:</p><ul> <li> For each $l \le i &lt; r$, the comparison between $a'_i$ and $a'_{i+1}$ is the same as that between $a_i$ and $a_{i+1}$, i.e., if $a_i &lt; a_{i + 1}$, then $a'_i &lt; a'_{i + 1}$; otherwise, if $a_i &gt; a_{i + 1}$, then $a'_i &gt; a'_{i + 1}$; otherwise, if $a_i = a_{i + 1}$, then $a'_i = a'_{i + 1}$. </li></ul><p>Ecrade wants to know the minimum number of operations to make the array strictly increasing. However, it seems a little difficult, so please help him!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$).</p><p>It is guaranteed that for each $1 \le i&lt; n$, $a_i \neq a_{i+1}$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer representing the minimum number of operations to make the array strictly increasing.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$).</p><p>It is guaranteed that for each $1 \le i&lt; n$, $a_i \neq a_{i+1}$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer representing the minimum number of operations to make the array strictly increasing.</p>





```input1|2,3,6,7
4
3
3 2 1
3
3 1 2
4
-2 -5 5 2
7
1 9 1 9 8 1 0
```




```output1
2
1
1
3
```



## Note

<p>In the first test case, a possible way to obtain the minimum number of operations:</p><ul> <li> In the first operation, choose $l = 2, r = 2$ and $a'_2 = 4$, then $a=[3, 4, 1]$; </li><li> In the second operation, choose $l = 1, r = 2$ and $a'_1 = -1, a'_2 = 0$, then $a=[-1, 0, 1]$. </li></ul><p>In the second test case, a possible way to obtain the minimum number of operations:</p><ul> <li> In the first operation, choose $l = 2, r = 3$ and $a'_2 = 4, a'_3 = 5$, then $a = [3, 4, 5]$. </li></ul><p>In the third test case, a possible way to obtain the minimum number of operations:</p><ul> <li> In the first operation, choose $l = 2, r = 3$ and $a'_2 = -1, a'_3 = 1$, then $a = [-2, -1, 1, 2]$. </li></ul>
