## Description

<div><p>   </p><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference between the versions is that in this version, $l\le r$. You can hack only if you solved all versions of this problem.</span> </p><p>You are given a positive integer $n$ and the first $n$ terms of an infinite binary sequence $a$, which is defined as follows:</p><ul> <li> For $m&gt;n$, $a_m = a_1 \oplus a_2 \oplus \ldots \oplus a_{\lfloor \frac{m}{2} \rfloor}$$^{\text{∗}}$. </li></ul><p>Your task is to compute the sum of elements in a given range $[l, r]$: $a_l + a_{l + 1} + \ldots + a_r$.</p><div class="statement-footnote"><p>$^{\text{∗}}$$\oplus$ denotes the <a>bitwise XOR operation</a>. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $l$, and $r$ ($1 \le n \le 2 \cdot 10^5$, $1 \le l \leq r \le 10^{18}$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($\color{red}{a_i \in \{0, 1\}}$)&nbsp;— the first $n$ terms of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the sum of elements in the given range.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $l$, and $r$ ($1 \le n \le 2 \cdot 10^5$, $1 \le l \leq r \le 10^{18}$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($\color{red}{a_i \in \{0, 1\}}$)&nbsp;— the first $n$ terms of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case, output a single integer&nbsp;— the sum of elements in the given range.</p>





```input1|2,3,6,7,10,11,14,15,18,19
9
1 1 1
1
2 3 10
1 0
3 5 25
1 1 1
1 234 567
0
5 1111 10000000000
1 0 1 0 1
1 1000000000000000000 1000000000000000000
1
10 41 87
0 1 1 1 1 1 1 1 0 0
12 65 69
1 0 0 0 0 1 0 1 0 1 1 0
13 46 54
0 1 0 1 1 1 1 1 1 0 1 1 1
```




```output1
1
5
14
0
6666665925
0
32
3
2
```



## Note

<p>In the first test case, the sequence $a$ is equal to $$[\underline{\color{red}{1}}, 1, 1, 0, 0, 1, 1, 1, 1, 1, \ldots]$$ where $l = 1$, and $r = 1$. The sum of elements in the range $[1, 1]$ is equal to $$a_1 = 1.$$</p><p>In the second test case, the sequence $a$ is equal to $$[\color{red}{1}, \color{red}{0}, \underline{1, 1, 1, 0, 0, 1, 1, 0}, \ldots]$$ where $l = 3$, and $r = 10$. The sum of elements in the range $[3, 10]$ is equal to $$a_3 + a_4 + \ldots + a_{10} = 1 + 1 + 1 + 0 + 0 + 1 + 1 + 0 = 5.$$</p>
