## Description

<div><p>In the 2050 Conference, some people from the competitive programming community meet together and are going to take a photo. The $n$ people form a line. They are numbered from $1$ to $n$ from left to right. Each of them either holds a cardboard with the letter '<span class="tex-font-style-tt">C</span>' or a cardboard with the letter '<span class="tex-font-style-tt">P</span>'.</p><p>Let $C=\{c_1,c_2,\dots,c_m\}$ $(c_1&lt;c_2&lt;\ldots &lt;c_m)$ be the set of people who hold cardboards of '<span class="tex-font-style-tt">C</span>'. Let $P=\{p_1,p_2,\dots,p_k\}$ $(p_1&lt;p_2&lt;\ldots &lt;p_k)$ be the set of people who hold cardboards of '<span class="tex-font-style-tt">P</span>'. The photo is good if and only if it satisfies the following constraints: </p><ol> <li> $C\cup P=\{1,2,\dots,n\}$ </li><li> $C\cap P =\emptyset $. </li><li> $c_i-c_{i-1}\leq c_{i+1}-c_i(1&lt; i &lt;m)$. </li><li> $p_i-p_{i-1}\geq p_{i+1}-p_i(1&lt; i &lt;k)$. </li></ol><p>Given an array $a_1,\ldots, a_n$, please find the number of good photos satisfying the following condition: $$\sum\limits_{x\in C} a_x &lt; \sum\limits_{y\in P} a_y.$$</p><p>The answer can be large, so output it modulo $998\,244\,353$. Two photos are different if and only if there exists at least one person who holds a cardboard of '<span class="tex-font-style-tt">C</span>' in one photo but holds a cardboard of '<span class="tex-font-style-tt">P</span>' in the other.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 200\,000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1\leq n\leq 200\,000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $200\,000$.</p></div><div class="output-specification"><p>For each test case, output the answer modulo $998\,244\,353$ in a separate line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 200\,000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1\leq n\leq 200\,000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $200\,000$.</p>

## Output

<p>For each test case, output the answer modulo $998\,244\,353$ in a separate line.</p>

## Samples

```input1
3
5
2 1 2 1 1
4
9 2 2 2
1
998244353
```

```output1
10
7
1
```




## Note

<p>For the first test case, there are $10$ possible good photos satisfying the condition: <span class="tex-font-style-tt">PPPPP</span>, <span class="tex-font-style-tt">CPPPP</span>, <span class="tex-font-style-tt">PCPPP</span>, <span class="tex-font-style-tt">CCPPP</span>, <span class="tex-font-style-tt">PCCPP</span>, <span class="tex-font-style-tt">PCPCP</span>, <span class="tex-font-style-tt">PPPPC</span>, <span class="tex-font-style-tt">CPPPC</span>, <span class="tex-font-style-tt">PCPPC</span>, <span class="tex-font-style-tt">PPPCC</span>.</p><p>For the second test case, there are $7$ possible good photos satisfying the condition: <span class="tex-font-style-tt">PPPP</span>, <span class="tex-font-style-tt">PCPP</span>, <span class="tex-font-style-tt">PCCP</span>, <span class="tex-font-style-tt">PPPC</span>, <span class="tex-font-style-tt">PCPC</span>, <span class="tex-font-style-tt">PPCC</span>, <span class="tex-font-style-tt">PCCC</span>.</p>
