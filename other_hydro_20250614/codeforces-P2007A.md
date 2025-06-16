## Description

<div><p>Dora has a set $s$ containing integers. In the beginning, she will put all integers in $[l, r]$ into the set $s$. That is, an integer $x$ is initially contained in the set if and only if $l \leq x \leq r$. Then she allows you to perform the following operations:</p><ul> <li> Select three <span class="tex-font-style-bf">distinct</span> integers $a$, $b$, and $c$ from the set $s$, such that $\gcd(a, b) = \gcd(b, c) = \gcd(a, c) = 1^\dagger$. </li><li> Then, remove these three integers from the set $s$. </li></ul><p>What is the maximum number of operations you can perform?</p><p>$^\dagger$Recall that $\gcd(x, y)$ means the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> of integers $x$ and $y$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 500$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $l$ and $r$ ($1 \leq l \leq r \leq 1000$)&nbsp;！ the range of integers in the initial set.</p></div><div class="output-specification"><p>For each test case, output a single integer ！ the maximum number of operations you can perform.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 500$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $l$ and $r$ ($1 \leq l \leq r \leq 1000$)&nbsp;！ the range of integers in the initial set.</p>

## Output

<p>For each test case, output a single integer ！ the maximum number of operations you can perform.</p>





```input1|2,4,6,8
8
1 3
3 7
10 21
2 8
51 60
2 15
10 26
1 1000
```




```output1
1
1
3
1
2
3
4
250
```



## Note

<p>In the first test case, you can choose $a = 1$, $b = 2$, $c = 3$ in the only operation, since $\gcd(1, 2) = \gcd(2, 3) = \gcd(1, 3) = 1$, and then there are no more integers in the set, so no more operations can be performed.</p><p>In the second test case, you can choose $a = 3$, $b = 5$, $c = 7$ in the only operation.</p><p>In the third test case, you can choose $a = 11$, $b = 19$, $c = 20$ in the first operation, $a = 13$, $b = 14$, $c = 15$ in the second operation, and $a = 10$, $b = 17$, $c = 21$ in the third operation. After the three operations, the set $s$ contains the following integers: $12$, $16$, $18$. It can be proven that it's impossible to perform more than $3$ operations.</p>
