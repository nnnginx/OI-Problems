## Description

<div><p>Let $\operatorname{lowbit}(x)$ denote the value of the lowest binary bit of $x$, e.g. $\operatorname{lowbit}(12)=4$, $\operatorname{lowbit}(8)=8$.</p><p>For an array $a$ of length $n$, if an array $s$ of length $n$ satisfies $s_k=\left(\sum\limits_{i=k-\operatorname{lowbit}(k)+1}^{k}a_i\right)\bmod 998\,244\,353$ for all $k$, then $s$ is called the <span class="tex-font-style-it">Fenwick Tree</span> of $a$. Let's denote it as $s=f(a)$.</p><p>For a positive integer $k$ and an array $a$, $f^k(a)$ is defined as follows:</p><p>$$ f^k(a)= \begin{cases} f(a)&amp;\textrm{if }k=1\\ f(f^{k-1}(a))&amp;\textrm{otherwise.}\\ \end{cases} $$</p><p>You are given an array $b$ of length $n$ and a positive integer $k$. Find an array $a$ that satisfies $0\le a_i &lt; 998\,244\,353$ and $f^k(a)=b$. It can be proved that an answer always exists. If there are multiple possible answers, you may print any of them.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two positive integers $n$ ($1 \leq n \leq 2\cdot 10^5$) and $k$ ($1\le k\le 10^9$), representing the length of the array and the number of times the function $f$ is performed.</p><p>The second line of each test case contains an array $b_1, b_2, \ldots, b_n$ ($0\le b_i &lt; 998\,244\,353$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line, containing a valid array $a$ of length $n$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two positive integers $n$ ($1 \leq n \leq 2\cdot 10^5$) and $k$ ($1\le k\le 10^9$), representing the length of the array and the number of times the function $f$ is performed.</p><p>The second line of each test case contains an array $b_1, b_2, \ldots, b_n$ ($0\le b_i &lt; 998\,244\,353$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, print a single line, containing a valid array $a$ of length $n$.</p>





```input1|2,3
2
8 1
1 2 1 4 1 2 1 8
6 2
1 4 3 17 5 16
```




```output1
1 1 1 1 1 1 1 1
1 2 3 4 5 6
```



## Note

<p>In the first test case, it can be seen that $f^1([1,1,1,1,1,1,1,1])=[1,2,1,4,1,2,1,8]$.</p><p>In the second test case, it can be seen that $f^2([1,2,3,4,5,6])=f^1([1,3,3,10,5,11])=[1,4,3,17,5,16]$.</p>
