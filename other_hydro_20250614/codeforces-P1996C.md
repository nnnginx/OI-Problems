## Description

<div><p>You are given two strings $a$ and $b$ of length $n$. Then, you are (forced against your will) to answer $q$ queries.</p><p>For each query, you are given a range bounded by $l$ and $r$. In one operation, you can choose an integer $i$ ($l \leq i \leq r$) and set $a_i = x$ where $x$ is any character you desire. Output the minimum number of operations you must perform such that $\texttt{sorted(a[l..r])} = \texttt{sorted(b[l..r])}$. <span class="tex-font-style-bf">The operations you perform on one query does not affect other queries.</span></p><p>For an arbitrary string $c$, $\texttt{sorted(c[l..r])}$ denotes the substring consisting of characters $c_l, c_{l+1}, ... , c_r$ sorted in lexicographical order.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 1000$) 每 the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n, q \leq 2 \cdot 10^5$) 每 the length of both strings and the number of queries.</p><p>The following line contains $a$ of length $n$. It is guaranteed $a$ only contains lowercase latin letters.</p><p>The following line contains $b$ of length $n$. It is guaranteed $b$ only contains lowercase latin letters.</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n$) 每 the range of the query.</p><p>It is guaranteed the sum of $n$ and $q$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each query, output an integer, the minimum number of operations you need to perform in a new line.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 1000$) 每 the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n, q \leq 2 \cdot 10^5$) 每 the length of both strings and the number of queries.</p><p>The following line contains $a$ of length $n$. It is guaranteed $a$ only contains lowercase latin letters.</p><p>The following line contains $b$ of length $n$. It is guaranteed $b$ only contains lowercase latin letters.</p><p>The following $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n$) 每 the range of the query.</p><p>It is guaranteed the sum of $n$ and $q$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each query, output an integer, the minimum number of operations you need to perform in a new line.</p>





```input1|2,3,4,5,6,7,13,14,15,16,17,18
3
5 3
abcde
edcba
1 5
1 4
3 3
4 2
zzde
azbe
1 3
1 4
6 3
uwuwuw
wuwuwu
2 4
1 3
1 6
```




```output1
0
1
0
2
2
1
1
0
```



## Note

<p>For the first query, $\texttt{sorted(a[1..5])} =$ <span class="tex-font-style-tt">abcde</span> and $\texttt{sorted(b[1..5])} =$ <span class="tex-font-style-tt">abcde</span>, so no operations are necessary.</p><p>For the second query, you need to set $a_1 = $ <span class="tex-font-style-tt">e</span>. Then, $\texttt{sorted(a[1..4])} = \texttt{sorted(b[1..4])} = $ <span class="tex-font-style-tt">bcde</span>.</p>
