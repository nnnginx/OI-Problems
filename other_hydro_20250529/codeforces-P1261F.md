## Description

<div><p>You are given two sets of integers: $A$ and $B$. You need to output the sum of elements in the set $C = \{x | x = a \oplus b, a \in A, b \in B\}$ modulo $998244353$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. Each number should be counted only once.</p><p>For example, if $A = \{2, 3\}$ and $B = \{2, 3\}$ you should count integer $1$ only once, despite the fact that you can get it as $3 \oplus 2$ and as $2 \oplus 3$. So the answer for this case is equal to $1 + 0 = 1$.</p><p>Let's call a segment $[l; r]$ a set of integers $\{l, l+1, \dots, r\}$.</p><p>The set $A$ is given as a union of $n_A$ segments, the set $B$ is given as a union of $n_B$ segments.</p></div><div class="input-specification"><p>The first line contains a single integer $n_A$ ($1 \le n_A \le 100$).</p><p>The $i$-th of the next $n_A$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le 10^{18}$), describing a segment of values of set $A$.</p><p>The next line contains a single integer $n_B$ ($1 \le n_B \le 100$).</p><p>The $i$-th of the next $n_B$ lines contains two integers $l_j$ and $r_j$ ($1 \le l_j \le r_j \le 10^{18}$), describing a segment of values of set $B$.</p><p>Note that segments in both sets may intersect.</p></div><div class="output-specification"><p>Print one integer&nbsp;�� the sum of all elements in set $C = \{x | x = a \oplus b, a \in A, b \in B\}$ modulo $998244353$.</p></div>

## Input

<p>The first line contains a single integer $n_A$ ($1 \le n_A \le 100$).</p><p>The $i$-th of the next $n_A$ lines contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le 10^{18}$), describing a segment of values of set $A$.</p><p>The next line contains a single integer $n_B$ ($1 \le n_B \le 100$).</p><p>The $i$-th of the next $n_B$ lines contains two integers $l_j$ and $r_j$ ($1 \le l_j \le r_j \le 10^{18}$), describing a segment of values of set $B$.</p><p>Note that segments in both sets may intersect.</p>

## Output

<p>Print one integer&nbsp;�� the sum of all elements in set $C = \{x | x = a \oplus b, a \in A, b \in B\}$ modulo $998244353$.</p>

## Samples

```input1
2
3 5
5 8
3
1 2
1 9
2 9
```

```output1
112
```






```input2
1
1 9
2
2 4
2 10
```

```output2
120
```




## Note

<p>In the second example, we can discover that the set $C = \{0,1,\dots,15\}$, which means that all numbers between $0$ and $15$ can be represented as $a \oplus b$.</p>
