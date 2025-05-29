## Description

<div><p>Given an array $a$ of length $n$, determine the lexicographically largest$^{\text{∗}}$ subsequence$^{\text{†}}$ $s$ of $a$ such that $s$ can be the side lengths of a polygon.</p><p>Recall that $s$ can be the side lengths of a polygon if and only if $|s| \geq 3$ and</p><p>$$ 2 \cdot \max(s_1, s_2, \ldots, s_{|s|}) &lt; s_1 + s_2 + \ldots + s_{|s|}. $$</p><p>If no such subsequence $s$ exists, print $-1$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A sequence $x$ is lexicographically smaller than a sequence $y$ if and only if one of the following holds:</p><ul><li> $x$ is a prefix of $y$, but $x \ne y$;</li><li> in the first position where $x$ and $y$ differ, the sequence $x$ has a smaller element than the corresponding element in $y$.</li></ul><p>$^{\text{†}}$A sequence $x$ is a subsequence of a sequence $y$ if $x$ can be obtained from $y$ by deleting several (possibly zero or all) elements.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($3 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the array $a$.</p><p>It is guaranteed that the total sum of all values of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the answer in the following format:</p><p>If the answer exists, output the following.</p><p>In the first line, output the integer $k$ ($1 \leq k \leq n$) — the length of the subsequence $s$.</p><p>In the second line, output $k$ integers $s_1, s_2, \ldots, s_k$ ($1 \leq s_i \leq 10^9$, $s$ is a subsequence of $a$) — the subsequence $s$. Note that the desired output is the value, not the index.</p><p>Otherwise, output a single line with the integer $-1$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($3 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the array $a$.</p><p>It is guaranteed that the total sum of all values of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the answer in the following format:</p><p>If the answer exists, output the following.</p><p>In the first line, output the integer $k$ ($1 \leq k \leq n$) — the length of the subsequence $s$.</p><p>In the second line, output $k$ integers $s_1, s_2, \ldots, s_k$ ($1 \leq s_i \leq 10^9$, $s$ is a subsequence of $a$) — the subsequence $s$. Note that the desired output is the value, not the index.</p><p>Otherwise, output a single line with the integer $-1$.</p>





```input1|2,3,6,7,10,11
5
3
3 1 2
4
1 4 2 3
6
1 6 4 5 3 2
6
43 12 99 53 22 4
7
9 764 54 73 22 23 1
```




```output1
-1
3
4 2 3 
4
6 5 3 2 
5
43 99 53 22 4 
4
54 73 23 1
```



## Note

<p>In the first test case, there are no subsequences that can be the side lengths of a polygon.</p><p>In the second test case, there are $2$ subsequences that can be the side lengths of a polygon: $1, 4, 2, 3$ and $4, 2, 3$. The latter is the lexicographically larger subsequence.</p>
