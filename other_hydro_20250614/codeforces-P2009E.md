## Description

<div><p>Klee has an array $a$ of length $n$ containing integers $[k, k+1, ..., k+n-1]$ in that order. Klee wants to choose an index $i$ ($1 \leq i \leq n$) such that $x = |a_1 + a_2 + \dots + a_i - a_{i+1} - \dots - a_n|$ is minimized. Note that for an arbitrary integer $z$, $|z|$ represents the absolute value of $z$. </p><p>Output the minimum possible value of $x$.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$) �� the number of test cases.</p><p>Each test case contains two integers $n$ and $k$ ($2 \leq n, k \leq 10^9$) �� the length of the array and the starting element of the array.</p></div><div class="output-specification"><p>For each test case, output the minimum value of $x$ on a new line.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$) �� the number of test cases.</p><p>Each test case contains two integers $n$ and $k$ ($2 \leq n, k \leq 10^9$) �� the length of the array and the starting element of the array.</p>

## Output

<p>For each test case, output the minimum value of $x$ on a new line.</p>





```input1|2,4
4
2 2
7 2
5 3
1000000000 1000000000
```




```output1
1
5
1
347369930
```



## Note

<p>In the first sample, $a = [2, 3]$. When $i = 1$ is chosen, $x = |2-3| = 1$. It can be shown this is the minimum possible value of $x$.</p><p>In the third sample, $a = [3, 4, 5, 6, 7]$. When $i = 3$ is chosen, $x = |3 + 4 + 5 - 6 - 7| = 1$. It can be shown this is the minimum possible value of $x$.</p>
