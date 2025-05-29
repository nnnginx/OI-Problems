## Description

<div><p>Let $bit(x)$ denote the number of ones in the binary representation of a non-negative integer $x$.</p><p>A subarray of an array is called <span class="tex-font-style-it">$k$-good</span> if it consists only of numbers with no more than $k$ ones in their binary representation, i.e., a subarray $(l, r)$ of array $a$ is good if for any $i$ such that $l \le i \le r$ condition $bit(a_{i}) \le k$ is satisfied.</p><p>You are given an array $a$ of length $n$, consisting of consecutive non-negative integers starting from $0$, i.e., $a_{i} = i$ for $0 \le i \le n - 1$ (in $0$-based indexing). You need to count the number of <span class="tex-font-style-it">$k$-good</span> subarrays in this array.</p><p>As the answer can be very large, output it modulo $10^{9} + 7$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. The following lines describe the test cases.</p><p>The single line of each test case contains two integers $n$, $k$ ($1 \le n \le 10^{18}, 1 \le k \le 60$).</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of <span class="tex-font-style-it">$k$-good</span> subarrays modulo $10^{9} + 7$.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. The following lines describe the test cases.</p><p>The single line of each test case contains two integers $n$, $k$ ($1 \le n \le 10^{18}, 1 \le k \le 60$).</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of <span class="tex-font-style-it">$k$-good</span> subarrays modulo $10^{9} + 7$.</p>





```input1|2,4,6,8,10
10
6 1
16 2
1 1
3 1
31 3
14 1
1337 5
100000 20
795569939321040850 56
576460752303423268 59
```




```output1
7
35
1
6
155
8
7323
49965
741136395
66679884
```



## Note

<p>For the first test case $a = [0, 1, 2, 3, 4, 5]$, $k = 1$.</p><p>To find the answer, let's write all the numbers in binary representation:</p><p>$$a = [\color{green}{000}, \color{green}{001}, \color{green}{010}, \color{red}{011}, \color{green}{100}, \color{red}{101}]$$</p><p>From this, it can be seen that the numbers $3$ and $5$ have $2 \ge (k = 1)$ ones in their binary representation, so the answer should include all subarrays that do not contain either $3$ or $5$, which are the subarrays (in $0$-based indexing): ($0$, $0$), ($0$, $1$), ($0$, $2$), ($1$, $1$), ($1$, $2$), ($2$, $2$), ($4$, $4$).</p>
