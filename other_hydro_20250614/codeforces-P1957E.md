## Description

<div><p>You are given an integer $n$. The function $C(i,k)$ represents the number of distinct ways you can select $k$ distinct numbers from the set {$1, 2, \ldots, i$} and arrange them in a circle$^\dagger$.</p><p>Find the value of $$ \sum\limits_{i=1}^n \sum\limits_{j=1}^i \left( C(i,j) \bmod j \right). $$ Here, the operation $x \bmod y$ denotes the remainder from dividing $x$ by $y$.</p><p>Since this value can be very large, find it modulo $10^9+7$.</p><p>$^\dagger$ In a circular arrangement, sequences are considered identical if one can be rotated to match the other. For instance, $[1, 2, 3]$ and $[2, 3, 1]$ are equivalent in a circle.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 10^6$).</p></div><div class="output-specification"><p>For each test case, output a single integer on a new line&nbsp;！ the value of the expression to be calculated modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \le n \le 10^6$).</p>

## Output

<p>For each test case, output a single integer on a new line&nbsp;！ the value of the expression to be calculated modulo $10^9+7$.</p>





```input1|2,4
4
1
3
6
314159
```




```output1
0
4
24
78926217
```



## Note

<p>In the first test case, $C(1,1) \bmod 1 = 0$.</p><p>In the second test case: </p><ul> <li> $C(1,1)=1$ (the arrangements are: $[1]$); </li><li> $C(2,1)=2$ (the arrangements are: $[1]$, $[2]$); </li><li> $C(2,2)=1$ (the arrangements are: $[1, 2]$); </li><li> $C(3,1)=3$ (the arrangements are: $[1]$, $[2]$, $[3]$); </li><li> $C(3,2)=3$ (the arrangements are: $[1, 2]$, $[2, 3]$, $[3, 1]$); </li><li> $C(3,3)=2$ (the arrangements are: $[1, 2, 3]$, $[1, 3, 2]$). </li></ul> In total, $\left(C(1,1) \bmod 1\right) + \left(C(2,1) \bmod 1\right) + \left(C(2,2) \bmod 2\right) + \left(C(3,1) \bmod 1\right) + \left(C(3,2) \bmod 2\right) + \left(C(3,3) \bmod 3\right) = 4$.
