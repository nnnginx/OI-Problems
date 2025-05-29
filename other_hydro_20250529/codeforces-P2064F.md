## Description

<div><p>You are given an array $a$ of length $n$ and an integer $k$.</p><p>Call a non-empty array $b$ of length $m$ <span class="tex-font-style-it">epic</span> if there exists an integer $i$ where $1 \le i &lt; m$ and $\min(b_1,\ldots,b_i) + \max(b_{i + 1},\ldots,b_m) = k$.</p><p>Count the number of <span class="tex-font-style-it">epic</span> subarrays$^{\text{∗}}$ of $a$.</p><div class="statement-footnote"><p>$^{\text{∗}}$An array $a$ is a subarray of an array $b$ if $a$ can be obtained from $b$ by the deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end. </p></div></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$; $n &lt; k &lt; 2 \cdot n$)&nbsp;— the length of the array $a$ and $k$.</p><p>The second line of each testcase contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le n$).</p><p>The sum of $n$ across all testcases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, output the number of epic contiguous subarrays of $a$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$; $n &lt; k &lt; 2 \cdot n$)&nbsp;— the length of the array $a$ and $k$.</p><p>The second line of each testcase contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le n$).</p><p>The sum of $n$ across all testcases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, output the number of epic contiguous subarrays of $a$.</p>





```input1|2,3,6,7,10,11
6
5 7
1 2 3 4 5
7 13
6 6 6 6 7 7 7
6 9
4 5 6 6 5 1
5 9
5 5 4 5 5
5 6
3 3 3 3 3
6 8
4 5 4 5 4 5
```




```output1
2
12
3
8
10
4
```



## Note

<p>These are all the epic subarrays in the first testcase: </p><ul> <li> $[2, 3, 4, 5]$, because $\min(2, 3) + \max(4, 5) = 2 + 5 = 7$. </li><li> $[3, 4]$, because $\min(3) + \max(4) = 3 + 4 = 7$. </li></ul><p>In the second test case, every subarray that contains at least one $6$ and at least one $7$ is epic.</p>
