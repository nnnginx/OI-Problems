## Description

<div><p><span class="tex-font-style-it">This is the harder version of the problem. In this version, $1 \le n, m \le 2\cdot10^5$. You can hack this problem if you locked it. But you can hack the previous problem only if you locked both problems.</span></p><p>You are given a sequence of integers $a=[a_1,a_2,\dots,a_n]$ of length $n$. Its <span class="tex-font-style-it">subsequence</span> is obtained by removing zero or more elements from the sequence $a$ (they do not necessarily go consecutively). For example, for the sequence $a=[11,20,11,33,11,20,11]$:</p><ul> <li> $[11,20,11,33,11,20,11]$, $[11,20,11,33,11,20]$, $[11,11,11,11]$, $[20]$, $[33,20]$ are subsequences (these are just some of the long list); </li><li> $[40]$, $[33,33]$, $[33,20,20]$, $[20,20,11,11]$ are not subsequences. </li></ul><p>Suppose that an additional non-negative integer $k$ ($1 \le k \le n$) is given, then the subsequence is called <span class="tex-font-style-it">optimal</span> if:</p><ul> <li> it has a length of $k$ and the sum of its elements is the maximum possible among all subsequences of length $k$; </li><li> and among all subsequences of length $k$ that satisfy the previous item, it is <span class="tex-font-style-it">lexicographically</span> minimal. </li></ul><p>Recall that the sequence $b=[b_1, b_2, \dots, b_k]$ is lexicographically smaller than the sequence $c=[c_1, c_2, \dots, c_k]$ if the first element (from the left) in which they differ less in the sequence $b$ than in $c$. Formally: there exists $t$ ($1 \le t \le k$) such that $b_1=c_1$, $b_2=c_2$, ..., $b_{t-1}=c_{t-1}$ and at the same time $b_t&lt;c_t$. For example:</p><ul> <li> $[10, 20, 20]$ lexicographically less than $[10, 21, 1]$, </li><li> $[7, 99, 99]$ is lexicographically less than $[10, 21, 1]$, </li><li> $[10, 21, 0]$ is lexicographically less than $[10, 21, 1]$. </li></ul><p>You are given a sequence of $a=[a_1,a_2,\dots,a_n]$ and $m$ requests, each consisting of two numbers $k_j$ and $pos_j$ ($1 \le k \le n$, $1 \le pos_j \le k_j$). For each query, print the value that is in the index $pos_j$ of the optimal subsequence of the given sequence $a$ for $k=k_j$.</p><p>For example, if $n=4$, $a=[10,20,30,20]$, $k_j=2$, then the optimal subsequence is $[20,30]$ ！ it is the minimum lexicographically among all subsequences of length $2$ with the maximum total sum of items. Thus, the answer to the request $k_j=2$, $pos_j=1$ is the number $20$, and the answer to the request $k_j=2$, $pos_j=2$ is the number $30$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 2\cdot10^5$) ！ the length of the sequence $a$.</p><p>The second line contains elements of the sequence $a$: integer numbers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>The third line contains an integer $m$ ($1 \le m \le 2\cdot10^5$) ！ the number of requests.</p><p>The following $m$ lines contain pairs of integers $k_j$ and $pos_j$ ($1 \le k \le n$, $1 \le pos_j \le k_j$) ！ the requests.</p></div><div class="output-specification"><p>Print $m$ integers $r_1, r_2, \dots, r_m$ ($1 \le r_j \le 10^9$) one per line: answers to the requests in the order they appear in the input. The value of $r_j$ should be equal to the value contained in the position $pos_j$ of the optimal subsequence for $k=k_j$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 2\cdot10^5$) ！ the length of the sequence $a$.</p><p>The second line contains elements of the sequence $a$: integer numbers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>The third line contains an integer $m$ ($1 \le m \le 2\cdot10^5$) ！ the number of requests.</p><p>The following $m$ lines contain pairs of integers $k_j$ and $pos_j$ ($1 \le k \le n$, $1 \le pos_j \le k_j$) ！ the requests.</p>

## Output

<p>Print $m$ integers $r_1, r_2, \dots, r_m$ ($1 \le r_j \le 10^9$) one per line: answers to the requests in the order they appear in the input. The value of $r_j$ should be equal to the value contained in the position $pos_j$ of the optimal subsequence for $k=k_j$.</p>

## Samples

```input1
3
10 20 10
6
1 1
2 1
2 2
3 1
3 2
3 3
```

```output1
20
10
20
10
20
10
```






```input2
7
1 2 1 3 1 2 1
9
2 1
2 2
3 1
3 2
3 3
1 1
7 1
7 7
7 4
```

```output2
2
3
2
3
2
3
1
1
3
```




## Note

<p>In the first example, for $a=[10,20,10]$ the optimal subsequences are: </p><ul> <li> for $k=1$: $[20]$, </li><li> for $k=2$: $[10,20]$, </li><li> for $k=3$: $[10,20,10]$. </li></ul>
