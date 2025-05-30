## Description

<div><p>You are given a multiset of powers of two. More precisely, for each $i$ from $0$ to $n$ exclusive you have $cnt_i$ elements equal to $2^i$.</p><p>In one operation, you can choose any one element $2^l &gt; 1$ and divide it into two elements $2^{l - 1}$.</p><p>You should perform $q$ queries. Each query has one of two types: </p><ul> <li> "$1$ $pos$ $val$"&nbsp;�� assign $cnt_{pos} := val$; </li><li> "$2$ $x$ $k$"&nbsp;�� calculate the minimum number of operations you need to make at least $k$ elements with value lower or equal to $2^x$. </li></ul><p>Note that all queries of the second type don't change the multiset; that is, you just calculate the minimum number of operations, you don't perform them.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n \le 30$; $1 \le q \le 2 \cdot 10^5$)&nbsp;�� the size of array $cnt$ and the number of queries.</p><p>The second line contains $n$ integers $cnt_0, cnt_1, \dots, cnt_{n - 1}$ ($0 \le cnt_i \le 10^6$).</p><p>Next $q$ lines contain queries: one per line. Each query has one of two types: </p><ul> <li> "$1$ $pos$ $val$" ($0 \le pos &lt; n$; $0 \le val \le 10^6$); </li><li> "$2$ $x$ $k$" ($0 \le x &lt; n$; $1 \le k \le 10^{15}$). </li></ul><p>It's guaranteed that there is at least one query of the second type.</p></div><div class="output-specification"><p>For each query of the second type, print the minimum number of operations you need to make at least $k$ elements with a value lower or equal to $2^x$ or $-1$ if there is no way to do it.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n \le 30$; $1 \le q \le 2 \cdot 10^5$)&nbsp;�� the size of array $cnt$ and the number of queries.</p><p>The second line contains $n$ integers $cnt_0, cnt_1, \dots, cnt_{n - 1}$ ($0 \le cnt_i \le 10^6$).</p><p>Next $q$ lines contain queries: one per line. Each query has one of two types: </p><ul> <li> "$1$ $pos$ $val$" ($0 \le pos &lt; n$; $0 \le val \le 10^6$); </li><li> "$2$ $x$ $k$" ($0 \le x &lt; n$; $1 \le k \le 10^{15}$). </li></ul><p>It's guaranteed that there is at least one query of the second type.</p>

## Output

<p>For each query of the second type, print the minimum number of operations you need to make at least $k$ elements with a value lower or equal to $2^x$ or $-1$ if there is no way to do it.</p>

## Samples

```input1
6 11
0 1 0 0 1 0
2 1 5
2 4 18
1 1 0
2 2 5
2 0 17
1 0 3
2 1 2
1 1 4
1 4 0
1 5 1
2 2 8
```

```output1
4
16
4
-1
0
1
```



