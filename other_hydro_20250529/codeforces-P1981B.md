## Description

<div><p>There is a sequence $a_0, a_1, a_2, \ldots$ of infinite length. Initially $a_i = i$ for every non-negative integer $i$.</p><p>After every second, each element of the sequence will <span class="tex-font-style-bf">simultaneously</span> change. $a_i$ will change to $a_{i - 1} \mid a_i \mid a_{i + 1}$ for every positive integer $i$. $a_0$ will change to $a_0 \mid a_1$. Here, $|$ denotes <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR</a>.</p><p>Turtle is asked to find the value of $a_n$ after $m$ seconds. In particular, if $m = 0$, then he needs to find the initial value of $a_n$. He is tired of calculating so many values, so please help him!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n, m$ ($0 \le n, m \le 10^9$).</p></div><div class="output-specification"><p>For each test case, output a single integer ¡ª the value of $a_n$ after $m$ seconds.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n, m$ ($0 \le n, m \le 10^9$).</p>

## Output

<p>For each test case, output a single integer ¡ª the value of $a_n$ after $m$ seconds.</p>





```input1|2,4,6,8,10
9
0 0
0 1
0 2
1 0
5 2
10 1
20 3
1145 14
19198 10
```




```output1
0
1
3
1
7
11
23
1279
19455
```



## Note

<p>After $1$ second, $[a_0, a_1, a_2, a_3, a_4, a_5]$ will become $[1, 3, 3, 7, 7, 7]$.</p><p>After $2$ seconds, $[a_0, a_1, a_2, a_3, a_4, a_5]$ will become $[3, 3, 7, 7, 7, 7]$.</p>
