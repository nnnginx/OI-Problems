## Description

<div><p>Suppose you have two arrays $c$ and $d$, each of length $k$. The pair $(c, d)$ is called <span class="tex-font-style-bf">good</span> if $c$ can be changed to $d$ by performing the following operation any number of times.</p><ul> <li> Select two distinct indices $i$ and $j$ ($1 \leq i, j \leq k$, $i \neq j$) and a nonnegative integer $x$ ($0 \leq x &lt; 2^{30}$). Then, apply the following transformations: <ul> <li> $c_i := c_i \mathbin{\&amp;} x$, where $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>. </li><li> $c_j := c_j \mathbin{|} x$, where $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>. </li></ul> </li></ul><p>You are given two arrays $a$ and $b$, both of length $n$, containing nonnegative integers not exceeding $m$. </p><p>You can perform two types of moves on these arrays any number of times:</p><ol> <li> Select an index $i$ ($1 \leq i \leq n$) and set $a_i := a_i + 1$. </li><li> Select an index $i$ ($1 \leq i \leq n$) and set $b_i := b_i + 1$. </li></ol><p>Note that the elements of $a$ and $b$ may exceed $m$ at some point while performing the moves.</p><p>Find the minimum number of moves required to make the pair $(a, b)$ good.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 2 \cdot 10^6$)&nbsp;！ the length of arrays $a$ and $b$, and the maximum possible value in these arrays, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq m$)&nbsp;！ denoting the array $a$.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \leq b_i \leq m$)&nbsp;！ denoting the array $b$.</p><p>Additionally, it is guaranteed that the sum of all values of $n$ and the sum of all values of $m$ across all test cases do not exceed $2 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of moves required to make the pair $(a, b)$ good.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n, m \leq 2 \cdot 10^6$)&nbsp;！ the length of arrays $a$ and $b$, and the maximum possible value in these arrays, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq m$)&nbsp;！ denoting the array $a$.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \leq b_i \leq m$)&nbsp;！ denoting the array $b$.</p><p>Additionally, it is guaranteed that the sum of all values of $n$ and the sum of all values of $m$ across all test cases do not exceed $2 \cdot 10^6$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of moves required to make the pair $(a, b)$ good.</p>





```input1|2,3,4,8,9,10,14,15,16
5
4 3
0 1 2 3
0 1 2 3
3 32
8 9 32
8 6 32
5 64
5 7 16 32 64
4 8 16 32 64
4 11
9 1 4 3
8 11 6 2
5 10
7 9 5 4 2
3 10 6 5 9
```




```output1
0
2
2
0
1
```



## Note

<p>In the first case, we already have $a = b$.</p><p>In the second case, we can perform move $2$ on index $i = 2$ twice. The array $b$ becomes $[8, 8, 32]$. We can see that $(a, b)$ is now good.</p><p>In the third case, we can perform move $2$ on index $i = 1$, then perform move $1$ on index $i = 2$. It can be proven that you cannot make the pair $(a, b)$ good in fewer than $2$ moves.</p>
