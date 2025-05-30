## Description

<div><p>Hr0d1y has $q$ queries on a binary string $s$ of length $n$. A binary string is a string containing only characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p><p>A query is described by a pair of integers $l_i$, $r_i$ $(1 \leq l_i \lt r_i \leq n)$. </p><p>For each query, he has to determine whether there exists a good subsequence in $s$ that is equal to the substring $s[l_i\ldots r_i]$. </p><ul> <li> A substring $s[i\ldots j]$ of a string $s$ is the string formed by characters $s_i s_{i+1} \ldots s_j$.</li><li> String $a$ is said to be a subsequence of string $b$ if $a$ can be obtained from $b$ by deleting some characters without changing the order of the remaining characters.</li><li> A subsequence is said to be <span class="tex-font-style-bf">good</span> if it is not contiguous and has length $\ge 2$. For example, if $s$ is "<span class="tex-font-style-tt">1100110</span>", then the subsequences $s_1s_2s_4$ ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">11</span>0<span class="tex-font-style-bf">0</span>110</span>") and $s_1s_5s_7$ ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">1</span>100<span class="tex-font-style-bf">1</span>1<span class="tex-font-style-bf">0</span></span>") are good, while $s_1s_2s_3$ ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">110</span>0110</span>") is not good. </li></ul><p>Can you help Hr0d1y answer each query?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1\leq t \leq 100$)&nbsp;�� the number of test cases. The description of each test case is as follows.</p><p>The first line contains two integers $n$ ($2 \leq n \leq 100$) and $q$ ($1\leq q \leq 100$)&nbsp;�� the length of the string and the number of queries. </p><p>The second line contains the string $s$.</p><p>The $i$-th of the next $q$ lines contains two integers $l_i$ and $r_i$ ($1 \leq l_i \lt r_i \leq n$).</p></div><div class="output-specification"><p>For each test case, output $q$ lines. The $i$-th line of the output of each test case should contain "<span class="tex-font-style-tt">YES</span>" if there exists a good subsequence equal to the substring $s[l_i...r_i]$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1\leq t \leq 100$)&nbsp;�� the number of test cases. The description of each test case is as follows.</p><p>The first line contains two integers $n$ ($2 \leq n \leq 100$) and $q$ ($1\leq q \leq 100$)&nbsp;�� the length of the string and the number of queries. </p><p>The second line contains the string $s$.</p><p>The $i$-th of the next $q$ lines contains two integers $l_i$ and $r_i$ ($1 \leq l_i \lt r_i \leq n$).</p>

## Output

<p>For each test case, output $q$ lines. The $i$-th line of the output of each test case should contain "<span class="tex-font-style-tt">YES</span>" if there exists a good subsequence equal to the substring $s[l_i...r_i]$, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print each letter in any case (upper or lower).</p>

## Samples

```input1
2
6 3
001000
2 4
1 3
3 5
4 2
1111
1 4
2 3
```

```output1
YES
NO
YES
NO
YES
```




## Note

<p>In the first test case, </p><ul> <li> $s[2\ldots 4] = $ "<span class="tex-font-style-tt">010</span>". In this case $s_1s_3s_5$ ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">0</span>0<span class="tex-font-style-bf">1</span>0<span class="tex-font-style-bf">0</span>0</span>") and $s_2s_3s_6$ ("<span class="tex-font-style-tt">0<span class="tex-font-style-bf">0</span><span class="tex-font-style-bf">1</span>00<span class="tex-font-style-bf">0</span></span>") are good suitable subsequences, while $s_2s_3s_4$ ("<span class="tex-font-style-tt">0<span class="tex-font-style-bf">0</span><span class="tex-font-style-bf">1</span><span class="tex-font-style-bf">0</span>00</span>") is not good. </li><li> $s[1\ldots 3] = $ "<span class="tex-font-style-tt">001</span>". No suitable good subsequence exists. </li><li> $s[3\ldots 5] = $ "<span class="tex-font-style-tt">100</span>". Here $s_3s_5s_6$ ("<span class="tex-font-style-tt">00<span class="tex-font-style-bf">1</span>0<span class="tex-font-style-bf">00</span></span>") is a suitable good subsequence. </li></ul>
