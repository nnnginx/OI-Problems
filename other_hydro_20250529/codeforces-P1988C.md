## Description

<div><p>You are given a positive integer $n$. Find the <span class="tex-font-style-bf">longest</span> sequence of positive integers $a=[a_1,a_2,\ldots,a_k]$ that satisfies the following conditions, and print the sequence:</p><ul> <li> $a_i\le n$ for all $1\le i\le k$. </li><li> $a$ is strictly increasing. That is, $a_i&gt;a_{i-1}$ for all $2\le i\le k$. </li><li> $a_i\,|\,a_{i-1}=n$ for all $2\le i\le k$, where $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>. </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The only line of each test case contains one integer $n$ ($1\le n\le 10^{18}$).</p><p>It's guaranteed that the sum of lengths of the longest valid sequences does not exceed $5\cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print two lines. In the first line, print the length of your constructed sequence, $k$. In the second line, print $k$ positive integers, denoting the sequence. If there are multiple longest sequences, you can print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The only line of each test case contains one integer $n$ ($1\le n\le 10^{18}$).</p><p>It's guaranteed that the sum of lengths of the longest valid sequences does not exceed $5\cdot 10^5$.</p>

## Output

<p>For each testcase, print two lines. In the first line, print the length of your constructed sequence, $k$. In the second line, print $k$ positive integers, denoting the sequence. If there are multiple longest sequences, you can print any of them.</p>





```input1|2,4
4
1
3
14
23
```




```output1
1
1
3
1 2 3
4
4 10 12 14
5
7 18 21 22 23
```


