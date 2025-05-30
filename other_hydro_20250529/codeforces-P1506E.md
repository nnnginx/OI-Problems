## Description

<div><p>A permutation is a sequence of $n$ integers from $1$ to $n$, in which all numbers occur exactly once. For example, $[1]$, $[3, 5, 2, 1, 4]$, $[1, 3, 2]$ are permutations, and $[2, 3, 2]$, $[4, 3, 1]$, $[0]$ are not.</p><p>Polycarp was presented with a permutation $p$ of numbers from $1$ to $n$. However, when Polycarp came home, he noticed that in his pocket, the permutation $p$ had turned into an array $q$ according to the following rule: </p><ul> <li> $q_i = \max(p_1, p_2, \ldots, p_i)$. </li></ul><p>Now Polycarp wondered what lexicographically minimal and lexicographically maximal permutations could be presented to him.</p><p>An array $a$ of length $n$ is lexicographically smaller than an array $b$ of length $n$ if there is an index $i$ ($1 \le i \le n$) such that the first $i-1$ elements of arrays $a$ and $b$ are the same, and the $i$-th element of the array $a$ is less than the $i$-th element of the array $b$. For example, the array $a=[1, 3, 2, 3]$ is lexicographically smaller than the array $b=[1, 3, 4, 2]$.</p><p>For example, if $n=7$ and $p=[3, 2, 4, 1, 7, 5, 6]$, then $q=[3, 3, 4, 4, 7, 7, 7]$ and the following permutations could have been as $p$ initially: </p><ul> <li> $[3, 1, 4, 2, 7, 5, 6]$ (lexicographically minimal permutation); </li><li> $[3, 1, 4, 2, 7, 6, 5]$; </li><li> $[3, 2, 4, 1, 7, 5, 6]$; </li><li> $[3, 2, 4, 1, 7, 6, 5]$ (lexicographically maximum permutation). </li></ul><p>For a given array $q$, find the lexicographically minimal and lexicographically maximal permutations that could have been originally presented to Polycarp.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $q_1, q_2, \ldots, q_n$ ($1 \le q_i \le n$).</p><p>It is guaranteed that the array $q$ was obtained by applying the rule from the statement to some permutation $p$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output two lines: </p><ul> <li> on the first line output $n$ integers&nbsp;�� lexicographically <span class="tex-font-style-bf">minimal</span> permutation that could have been originally presented to Polycarp; </li><li> on the second line print $n$ integers&nbsp;�� lexicographically <span class="tex-font-style-bf">maximal</span> permutation that could have been originally presented to Polycarp; </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $q_1, q_2, \ldots, q_n$ ($1 \le q_i \le n$).</p><p>It is guaranteed that the array $q$ was obtained by applying the rule from the statement to some permutation $p$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output two lines: </p><ul> <li> on the first line output $n$ integers&nbsp;�� lexicographically <span class="tex-font-style-bf">minimal</span> permutation that could have been originally presented to Polycarp; </li><li> on the second line print $n$ integers&nbsp;�� lexicographically <span class="tex-font-style-bf">maximal</span> permutation that could have been originally presented to Polycarp; </li></ul>

## Samples

```input1
4
7
3 3 4 4 7 7 7
4
1 2 3 4
7
3 4 5 5 5 7 7
1
1
```

```output1
3 1 4 2 7 5 6 
3 2 4 1 7 6 5 
1 2 3 4 
1 2 3 4 
3 4 5 1 2 7 6 
3 4 5 2 1 7 6 
1 
1
```



