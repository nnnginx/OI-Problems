## Description

<div><p>You are the proud... never mind, just solve this problem.</p><p>There are $n$ intervals $[l_1, r_1], [l_2, r_2], \ldots [l_n, r_n]$. For each $x$ from $0$ to $2^m - 1$, find the number, modulo $998\,244\,353$, of sequences $a_1, a_2, \ldots a_n$ such that:</p><ul><li> $l_i \leq a_i \leq r_i$ for all $i$ from $1$ to $n$; </li><li> $a_1 \oplus a_2 \oplus \ldots \oplus a_n = x$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operator</a>. </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq m \leq 18$).</p><p>The $i$-th of the next $n$ lines contains two integers $l_i$ and $r_i$ ($0 \leq l_i \leq r_i &lt; 2^m$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$, and the sum of $2^m$ over all test cases does not exceed $2^{18}$.</p></div><div class="output-specification"><p>For each $x$ from $0$ to $2^m - 1$, let:</p><ul><li> $f_x$ be the number of valid sequences, modulo $998\,244\,353$; </li><li> $g_x = f_x \cdot 2^x \mod 998\,244\,353$. </li></ul><p>Here, $f_x$ and $g_x$ are both integers in the interval $[0, 998\,244\,352]$.</p><p>Let $h = g_0 \oplus g_1 \oplus \ldots \oplus g_{2^m - 1}$.</p><p>Output a single integer&nbsp;¡ª the value of $h$ itself. <span class="tex-font-style-bf">Do not</span> perform a modulo operation. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq m \leq 18$).</p><p>The $i$-th of the next $n$ lines contains two integers $l_i$ and $r_i$ ($0 \leq l_i \leq r_i &lt; 2^m$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$, and the sum of $2^m$ over all test cases does not exceed $2^{18}$.</p>

## Output

<p>For each $x$ from $0$ to $2^m - 1$, let:</p><ul><li> $f_x$ be the number of valid sequences, modulo $998\,244\,353$; </li><li> $g_x = f_x \cdot 2^x \mod 998\,244\,353$. </li></ul><p>Here, $f_x$ and $g_x$ are both integers in the interval $[0, 998\,244\,352]$.</p><p>Let $h = g_0 \oplus g_1 \oplus \ldots \oplus g_{2^m - 1}$.</p><p>Output a single integer&nbsp;¡ª the value of $h$ itself. <span class="tex-font-style-bf">Do not</span> perform a modulo operation. </p>





```input1|2,3,4,11,12,13,14,15,16,17,18,19,20,21
4
2 2
0 2
1 3
5 3
3 7
1 3
0 2
1 5
3 6
10 14
314 1592
653 5897
932 3846
264 3383
279 5028
841 9716
939 9375
105 8209
749 4459
230 7816
1 5
0 29
```




```output1
22
9812
75032210
1073741823
```



## Note

<p>For the first test case, the values of $f_x$ are as follows:</p><ul><li> $f_0 = 2$, because there are $2$ valid sequences: $[1, 1]$ and $[2, 2]$; </li><li> $f_1 = 2$, because there are $2$ valid sequences: $[0, 1]$ and $[2, 3]$; </li><li> $f_2 = 2$, because there are $2$ valid sequences: $[0, 2]$ and $[1, 3]$; </li><li> $f_3 = 3$, because there are $3$ valid sequences: $[0, 3]$, $[1, 2]$, and $[2, 1]$.</li></ul><p>The values of $g_x$ are as follows:</p><ul><li> $g_0 = f_0 \cdot 2^0 = 2 \cdot 2^0 = 2$; </li><li> $g_1 = f_1 \cdot 2^1 = 2 \cdot 2^1 = 4$; </li><li> $g_2 = f_2 \cdot 2^2 = 2 \cdot 2^2 = 8$; </li><li> $g_3 = f_3 \cdot 2^3 = 3 \cdot 2^3 = 24$.</li></ul><p>Thus, the value to output is $2 \oplus 4 \oplus 8 \oplus 24 = 22$.</p><p>For the second test case, the values of $f_x$ are as follows:</p><ul><li> $f_{0} = 120$; </li><li> $f_{1} = 120$; </li><li> $f_{2} = 119$; </li><li> $f_{3} = 118$; </li><li> $f_{4} = 105$; </li><li> $f_{5} = 105$; </li><li> $f_{6} = 106$; </li><li> $f_{7} = 107$.</li></ul>
