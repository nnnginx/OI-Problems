## Description

<div><p>Recently, Misha at the IT Campus "NEIMARK" camp learned a new topic&nbsp;！ the Euclidean algorithm.</p><p>He was somewhat surprised when he realized that $a \cdot b = lcm(a, b) \cdot gcd(a, b)$, where $gcd(a, b)$&nbsp;！ is <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">the greatest common divisor (GCD)</a> of the numbers $a$ and $b$ and $lcm(a, b)$&nbsp;！ is <a href="https://en.wikipedia.org/wiki/Least_common_multiple">the least common multiple (LCM)</a>. Misha thought that since the product of LCM and GCD exists, it might be interesting to consider their quotient: $F(a,b)=\frac{lcm(a, b)}{gcd(a, b)}$.</p><p>For example, he took $a = 2$ and $b = 4$, computed $F(2, 4) = \frac{4}{2} = 2$ and obtained a prime number (a number is prime if it has exactly two divisors)! Now he considers $F(a, b)$ to be an interesting ratio if $a &lt; b$ and $F(a, b)$ is a prime number.</p><p>Since Misha has just started studying number theory, he needs your help to calculate ！ how many different pairs of numbers $a$ and $b$ are there such that $F(a, b)$ is an interesting ratio and $1 \leq a &lt; b \leq n$?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^3$). The description of the test cases follows.</p><p>A single line of each test case contains a single integer $n$ ($2 \leq n \leq 10^7$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^7$.</p></div><div class="output-specification"><p>For each test case, output the number of interesting ratios $F(a, b)$ for pairs satisfying $1 \leq a &lt; b \leq n$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^3$). The description of the test cases follows.</p><p>A single line of each test case contains a single integer $n$ ($2 \leq n \leq 10^7$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^7$.</p>

## Output

<p>For each test case, output the number of interesting ratios $F(a, b)$ for pairs satisfying $1 \leq a &lt; b \leq n$.</p>





```input1|2,4
4
5
10
34
10007
```




```output1
4
11
49
24317
```


