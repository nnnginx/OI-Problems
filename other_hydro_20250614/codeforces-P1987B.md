## Description

<div><p>You are given an array of integers $a$ of length $n$. </p><p>You can apply the following operation any number of times (maybe, zero): </p><ul> <li> First, choose an integer $k$ such that $1 \le k \le n$ and pay $k + 1$ coins. </li><li> Then, choose <span class="tex-font-style-bf">exactly</span> $k$ indices such that $1 \le i_1 &lt; i_2 &lt; \ldots &lt; i_k \le n$. </li><li> Then, for each $x$ from $1$ to $k$, increase $a_{i_x}$ by $1$. </li></ul><p>Find the minimum number of coins needed to make $a$ non-decreasing. That is, $a_1 \le a_2 \le \ldots \le a_n$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of coins needed to make $a$ non-decreasing.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of coins needed to make $a$ non-decreasing.</p>





```input1|2,3,6,7,10,11
5
3
1 7 9
5
2 1 4 7 6
4
1 3 2 4
1
179
9
344 12 37 60 311 613 365 328 675
```




```output1
0
3
2
0
1821
```



## Note

<p>In the first test case, $a$ is already sorted, so you don't have to spend any coins.</p><p>In the second test case, the optimal sequence of operations is: </p><ul> <li> Choose $k = 2$ and the indices $2$ and $5$: $[ 2, \color{red}{1}, 4, 7, \color{red}{6} ] \rightarrow [2, 2, 4, 7, 7]$. This costs $3$ coins. </li></ul> It can be proven that it is not possible to make $a$ non-decreasing by spending less than $3$ coins.
