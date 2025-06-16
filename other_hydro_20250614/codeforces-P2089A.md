## Description

<div><p>Given an integer $n$. Construct a permutation $p_1, p_2, \ldots, p_n$ of length $n$ that satisfies the following property:</p><p>For $1 \le i \le n$, define $c_i = \lceil \frac{p_1+p_2+\ldots +p_i}{i} \rceil$, then among $c_1,c_2,\ldots,c_n$ there must be at least $\lfloor \frac{n}{3} \rfloor - 1$ prime numbers.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>In a single line of each test case, there is a single integer $n$ ($2 \le n \le 10^5)$&nbsp;！ the size of the permutation.</p></div><div class="output-specification"><p>For each test case, output the permutation $p_1,p_2,\ldots,p_n$ of length $n$ that satisfies the condition. It is guaranteed that such a permutation always exists.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>In a single line of each test case, there is a single integer $n$ ($2 \le n \le 10^5)$&nbsp;！ the size of the permutation.</p>

## Output

<p>For each test case, output the permutation $p_1,p_2,\ldots,p_n$ of length $n$ that satisfies the condition. It is guaranteed that such a permutation always exists.</p>





```input1|2,4
3
2
3
5
```




```output1
2 1
2 1 3
2 1 3 4 5
```



## Note

<p>In the first test case, $c_1 = \lceil \frac{2}{1} \rceil = 2$, $c_2 = \lceil \frac{2+1}{2} \rceil = 2$. Both are prime numbers.</p><p>In the third test case, $c_1 = \lceil \frac{2}{1} \rceil = 2$, $c_2 = \lceil \frac{3}{2} \rceil = 2$, $c_3 = \lceil \frac{6}{3} \rceil = 2$, $c_4 = \lceil \frac{10}{4} \rceil = 3$, $c_5 = \lceil \frac{15}{5} \rceil = 3$. All these numbers are prime.</p>
