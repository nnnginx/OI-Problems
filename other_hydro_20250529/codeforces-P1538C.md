## Description

<div><p>You are given an array $a$ of $n$ integers. Find the number of pairs $(i, j)$ ($1 \le i &lt; j \le n$) where the sum of $a_i + a_j$ is greater than or equal to $l$ and less than or equal to $r$ (that is, $l \le a_i + a_j \le r$).</p><p>For example, if $n = 3$, $a = [5, 1, 2]$, $l = 4$ and $r = 7$, then two pairs are suitable: </p><ul> <li> $i=1$ and $j=2$ ($4 \le 5 + 1 \le 7$); </li><li> $i=1$ and $j=3$ ($4 \le 5 + 2 \le 7$). </li></ul></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains three integers $n, l, r$ ($1 \le n \le 2 \cdot 10^5$, $1 \le l \le r \le 10^9$)&nbsp;�� the length of the array and the limits on the sum in the pair.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ overall test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;�� the number of index pairs $(i, j)$ ($i &lt; j$), such that $l \le a_i + a_j \le r$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains three integers $n, l, r$ ($1 \le n \le 2 \cdot 10^5$, $1 \le l \le r \le 10^9$)&nbsp;�� the length of the array and the limits on the sum in the pair.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ overall test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;�� the number of index pairs $(i, j)$ ($i &lt; j$), such that $l \le a_i + a_j \le r$.</p>

## Samples

```input1
4
3 4 7
5 1 2
5 5 8
5 1 2 4 3
4 100 1000
1 1 1 1
5 9 13
2 5 5 1 1
```

```output1
2
7
0
1
```



