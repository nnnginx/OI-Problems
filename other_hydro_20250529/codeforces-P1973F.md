## Description

<div><p>For $k$ positive integers $x_1, x_2, \ldots, x_k$, the value $\gcd(x_1, x_2, \ldots, x_k)$ is the greatest common divisor of the integers $x_1, x_2, \ldots, x_k$&nbsp;�� the largest integer $z$ such that all the integers $x_1, x_2, \ldots, x_k$ are divisible by $z$.</p><p>You are given three arrays $a_1, a_2, \ldots, a_n$, $b_1, b_2, \ldots, b_n$ and $c_1, c_2, \ldots, c_n$ of length $n$, containing positive integers. </p><p>You also have a machine that allows you to swap $a_i$ and $b_i$ for any $i$ ($1 \le i \le n$). Each swap costs you $c_i$ coins.</p><p>Find the maximum possible value of $$\gcd(a_1, a_2, \ldots, a_n) + \gcd(b_1, b_2, \ldots, b_n)$$ that you can get by paying in total at most $d$ coins for swapping some elements. The amount of coins you have changes a lot, so find the answer to this question for each of the $q$ possible values $d_1, d_2, \ldots, d_q$.</p></div><div class="input-specification"><p>There are two integers on the first line&nbsp;�� the numbers $n$ and $q$ ($1 \leq n \leq 5 \cdot 10^5$, $1 \leq q \leq 5 \cdot 10^5$).</p><p>On the second line, there are $n$ integers&nbsp;�� the numbers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^8$).</p><p>On the third line, there are $n$ integers&nbsp;�� the numbers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 10^8$).</p><p>On the fourth line, there are $n$ integers&nbsp;�� the numbers $c_1, c_2, \ldots, c_n$ ($1 \leq c_i \leq 10^9$).</p><p>On the fifth line, there are $q$ integers&nbsp;�� the numbers $d_1, d_2, \ldots, d_q$ ($0 \leq d_i \leq 10^{15}$).</p></div><div class="output-specification"><p>Print $q$ integers&nbsp;�� the maximum value you can get for each of the $q$ possible values $d$.</p></div>

## Input

<p>There are two integers on the first line&nbsp;�� the numbers $n$ and $q$ ($1 \leq n \leq 5 \cdot 10^5$, $1 \leq q \leq 5 \cdot 10^5$).</p><p>On the second line, there are $n$ integers&nbsp;�� the numbers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^8$).</p><p>On the third line, there are $n$ integers&nbsp;�� the numbers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 10^8$).</p><p>On the fourth line, there are $n$ integers&nbsp;�� the numbers $c_1, c_2, \ldots, c_n$ ($1 \leq c_i \leq 10^9$).</p><p>On the fifth line, there are $q$ integers&nbsp;�� the numbers $d_1, d_2, \ldots, d_q$ ($0 \leq d_i \leq 10^{15}$).</p>

## Output

<p>Print $q$ integers&nbsp;�� the maximum value you can get for each of the $q$ possible values $d$.</p>





```input1|
3 4
1 2 3
4 5 6
1 1 1
0 1 2 3
```




```input2|
5 5
3 4 6 8 4
8 3 4 9 3
10 20 30 40 50
5 55 13 1000 113
```




```input3|
1 1
3
4
5
0
```




```output1
2 3 3 3
```




```output2
2 7 3 7 7
```




```output3
7
```



## Note

<p>In the first query of the first example, we are not allowed to do any swaps at all, so the answer is $\gcd(1, 2, 3) + \gcd(4, 5, 6) = 2$. In the second query, one of the ways to achieve the optimal value is to swap $a_2$ and $b_2$, then the answer is $\gcd(1, 5, 3) + \gcd(4, 2, 6) = 3$.</p><p>In the second query of the second example, it's optimal to perform swaps on positions $1$ and $3$, then the answer is $\gcd(3, 3, 6, 9, 3) + \gcd(8, 4, 4, 8, 4) = 7$ and we have to pay $40$ coins in total.</p>
