## Description

<div><p>Omkar has received a message from Anton saying "Your story for problem A is confusing. Just make a formal statement." Because of this, Omkar gives you an array $a = [a_1, a_2, \ldots, a_n]$ of $n$ distinct integers. An array $b = [b_1, b_2, \ldots, b_k]$ is called <span class="tex-font-style-bf">nice</span> if for any two distinct elements $b_i, b_j$ of $b$, $|b_i-b_j|$ appears in $b$ at least once. In addition, all elements in $b$ must be distinct. Can you add several (maybe, $0$) integers to $a$ to create a <span class="tex-font-style-bf">nice</span> array $b$ <span class="tex-font-style-bf">of size at most $300$</span>? If $a$ is already <span class="tex-font-style-bf">nice</span>, you don't have to add any elements.</p><p>For example, array $[3, 6, 9]$ is <span class="tex-font-style-bf">nice</span>, as $|6-3|=|9-6| = 3$, which appears in the array, and $|9-3| = 6$, which appears in the array, while array $[4, 2, 0, 6, 9]$ is not <span class="tex-font-style-bf">nice</span>, as $|9-4| = 5$ is not present in the array.</p><p>For integers $x$ and $y$, $|x-y| = x-y$ if $x &gt; y$ and $|x-y| = y-x$ otherwise.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains $t$ ($1 \leq t \leq 50$), the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 100$) �� the length of the array $a$.</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \cdots, a_n$ ($-100 \leq a_i \leq 100$) �� the elements of the array $a$.</p></div><div class="output-specification"><p>For each test case, output one line containing <span class="tex-font-style-tt">YES</span> if Omkar can create a <span class="tex-font-style-bf">nice</span> array $b$ by adding elements to $a$ and <span class="tex-font-style-tt">NO</span> otherwise. The case of each letter does not matter, so <span class="tex-font-style-tt">yEs</span> and <span class="tex-font-style-tt">nO</span> will also be accepted.</p><p>If the first line is <span class="tex-font-style-tt">YES</span>, output a second line containing a single integer $k$ ($n \leq k \leq 300$). </p><p>Then output one line containing $k$ <span class="tex-font-style-bf">distinct</span> integers $b_1, b_2, \cdots, b_k$ ($-10^9 \leq b_i \leq 10^9$), the elements of the <span class="tex-font-style-bf">nice</span> array $b$. $b_1, b_2, \cdots, b_k$ can be in any order. For each $a_i$ in $a$, $a_i$ must appear at least once in $b$.</p><p>It can be proved that if Omkar can create such an array $b$, then he can also do so in a way that satisfies the above constraints.</p><p>If multiple solutions exist, you can print any. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains $t$ ($1 \leq t \leq 50$), the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 100$) �� the length of the array $a$.</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \cdots, a_n$ ($-100 \leq a_i \leq 100$) �� the elements of the array $a$.</p>

## Output

<p>For each test case, output one line containing <span class="tex-font-style-tt">YES</span> if Omkar can create a <span class="tex-font-style-bf">nice</span> array $b$ by adding elements to $a$ and <span class="tex-font-style-tt">NO</span> otherwise. The case of each letter does not matter, so <span class="tex-font-style-tt">yEs</span> and <span class="tex-font-style-tt">nO</span> will also be accepted.</p><p>If the first line is <span class="tex-font-style-tt">YES</span>, output a second line containing a single integer $k$ ($n \leq k \leq 300$). </p><p>Then output one line containing $k$ <span class="tex-font-style-bf">distinct</span> integers $b_1, b_2, \cdots, b_k$ ($-10^9 \leq b_i \leq 10^9$), the elements of the <span class="tex-font-style-bf">nice</span> array $b$. $b_1, b_2, \cdots, b_k$ can be in any order. For each $a_i$ in $a$, $a_i$ must appear at least once in $b$.</p><p>It can be proved that if Omkar can create such an array $b$, then he can also do so in a way that satisfies the above constraints.</p><p>If multiple solutions exist, you can print any. </p>

## Samples

```input1
4
3
3 0 9
2
3 4
5
-7 3 13 -2 8
4
4 8 12 6
```

```output1
yes
4
6 0 3 9
yEs
5
5 3 1 2 4
NO
Yes
6
8 12 6 2 4 10
```




## Note

<p>For the first case, you can add integers to $a$ to receive the array $b = [6, 0, 3, 9]$. Note that $|6-3| = |9-6| = |3-0| = 3$ and $3$ is in $b$, $|6-0| = |9-3| = 6$ and $6$ is in $b$, and $|9-0| = 9$ is in $b$, so $b$ is <span class="tex-font-style-bf">nice</span>.</p><p>For the second case, you can add integers to $a$ to receive the array $b = [5, 3, 1, 2, 4]$. We have that $|2-1| = |3-2| = |4-3| = |5-4| = 1$ is in $b$, $|3-1| = |4-2| = |5-3| = 2$ is in $b$, $|4-1| = |5-2| = 3$ is in $b$, and $|5-1| = 4$ is in $b$, so $b$ is <span class="tex-font-style-bf">nice</span>.</p><p>For the fourth case, you can add integers to $a$ to receive the array $b = [8, 12, 6, 2, 4, 10]$. We have that $|4-2| = |6-4| = |8-6| = |10-8| = |12-10| = 2$ is in $b$, $|6-2| = |8-4| = |10-6| = |12-8| = 4$ is in $b$, $|8-2| = |10-4| = |12-6| = 6$ is in $b$, $|10-2| = |12-4| = 8$ is in $b$, and $|12-2| = 10$ is in $b$, so $b$ is <span class="tex-font-style-bf">nice</span>.</p><p>It can be proven that for all other test cases it is impossible to create a <span class="tex-font-style-bf">nice</span> array $b$.</p>
