## Description

<div><p>You are given an array $b$ of $n - 1$ integers.</p><p>An array $a$ of $n$ integers is called <span class="tex-font-style-it">good</span> if $b_i = a_i \, \&amp; \, a_{i + 1}$ for $1 \le i \le n-1$, where $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operator</a>.</p><p>Construct a good array, or report that no good arrays exist.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n - 1$ integers $b_1, b_2, \ldots, b_{n - 1}$ ($0 \le b_i &lt; 2^{30}$)&nbsp;！ the elements of the array $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer $-1$ if no good arrays exist. </p><p>Otherwise, output $n$ space-separated integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{30}$)&nbsp;！ the elements of a good array $a$.</p><p>If there are multiple solutions, you may output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n - 1$ integers $b_1, b_2, \ldots, b_{n - 1}$ ($0 \le b_i &lt; 2^{30}$)&nbsp;！ the elements of the array $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output a single integer $-1$ if no good arrays exist. </p><p>Otherwise, output $n$ space-separated integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{30}$)&nbsp;！ the elements of a good array $a$.</p><p>If there are multiple solutions, you may output any of them.</p>





```input1|2,3,6,7
4
2
1
3
2 0
4
1 2 3
5
3 5 4 2
```




```output1
5 3
3 2 1
-1
3 7 5 6 3
```



## Note

<p>In the first test case, $b = [1]$. A possible good array is $a=[5, 3]$, because $a_1 \, \&amp; \, a_2 = 5 \, \&amp; \, 3 = 1 = b_1$.</p><p>In the second test case, $b = [2, 0]$. A possible good array is $a=[3, 2, 1]$, because $a_1 \, \&amp; \, a_2 = 3 \, \&amp; \, 2 = 2 = b_1$ and $a_2 \, \&amp; \, a_3 = 2 \, \&amp; \, 1 = 0 = b_2$.</p><p>In the third test case, $b = [1, 2, 3]$. It can be shown that no good arrays exist, so the output is $-1$.</p><p>In the fourth test case, $b = [3, 5, 4, 2]$. A possible good array is $a=[3, 7, 5, 6, 3]$.</p>
