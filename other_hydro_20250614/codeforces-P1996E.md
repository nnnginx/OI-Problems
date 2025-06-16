## Description

<div><p><span class="tex-font-style-it">In a desperate attempt to obtain your <span class="tex-font-style-striked">waifu</span> favorite character, you have hacked into the source code of the game. After days of struggling, you finally find the binary string that encodes the gacha system of the game. In order to decode it, you must first solve the following problem.</span> </p><p>You are given a binary string $s$ of length $n$. For each pair of integers $(l, r)$ $(1 \leq l \leq r \leq n)$, count the number of pairs $(x, y)$ $(l \leq x \leq y \leq r)$ such that the amount of $\mathtt{0}$ equals the amount of $\mathtt{1}$ in the substring $s_xs_{x+1}...s_y$. </p><p>Output the sum of counts over all possible $(l, r)$ modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 1000$)&nbsp;¡ª the number of test cases.</p><p>Each test case contains a binary string $s$ ($1 \leq |s| \leq 2 \cdot 10^5$). It is guaranteed $s$ only contains characters $\mathtt{0}$ and $\mathtt{1}$.</p><p>It is guaranteed the sum of $|s|$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output an integer, the answer modulo $10^9+7$.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 1000$)&nbsp;¡ª the number of test cases.</p><p>Each test case contains a binary string $s$ ($1 \leq |s| \leq 2 \cdot 10^5$). It is guaranteed $s$ only contains characters $\mathtt{0}$ and $\mathtt{1}$.</p><p>It is guaranteed the sum of $|s|$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output an integer, the answer modulo $10^9+7$.</p>





```input1|2,4
4
0000
01010101
1100111001
11000000111
```




```output1
0
130
147
70
```


