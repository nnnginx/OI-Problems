## Description

<div><p>A permutation is a sequence of integers from $1$ to $n$ of length $n$ containing each number exactly once. For example, $[1]$, $[4, 3, 5, 1, 2]$, $[3, 2, 1]$&nbsp;！ are permutations, and $[1, 1]$, $[4, 3, 1]$, $[2, 3, 4]$&nbsp;！ no.</p><p>Permutation $a$ is lexicographically smaller than permutation $b$ (they have the same length $n$), if in the first index $i$ in which they differ, $a[i] &lt; b[i]$. For example, the permutation $[1, 3, 2, 4]$ is lexicographically smaller than the permutation $[1, 3, 4, 2]$, because the first two elements are equal, and the third element in the first permutation is smaller than in the second.</p><p>The next permutation for a permutation $a$ of length $n$&nbsp;！ is the lexicographically smallest permutation $b$ of length $n$ that lexicographically larger than $a$. For example: </p><ul> <li> for permutation $[2, 1, 4, 3]$ the next permutation is $[2, 3, 1, 4]$; </li><li> for permutation $[1, 2, 3]$ the next permutation is $[1, 3, 2]$; </li><li> for permutation $[2, 1]$ next permutation does not exist. </li></ul><p>You are given the number $n$&nbsp;！ the length of the initial permutation. The initial permutation has the form $a = [1, 2, \ldots, n]$. In other words, $a[i] = i$ ($1 \le i \le n$).</p><p>You need to process $q$ queries of two types: </p><ul> <li> $1$ $l$ $r$: query for the sum of all elements on the segment $[l, r]$. More formally, you need to find $a[l] + a[l + 1] + \ldots + a[r]$. </li><li> $2$ $x$: $x$ times replace the current permutation with the next permutation. For example, if $x=2$ and the current permutation has the form $[1, 3, 4, 2]$, then we should perform such a chain of replacements $[1, 3, 4, 2] \rightarrow [1, 4, 2, 3] \rightarrow [1, 4, 3, 2]$. </li></ul><p>For each query of the $1$-st type output the required sum.</p></div><div class="input-specification"><p>The first line contains two integers $n$ ($2 \le n \le 2 \cdot 10^5$) and $q$ ($1 \le q \le 2 \cdot 10^5$), where $n$&nbsp;！ the length of the initial permutation, and $q$&nbsp;！ the number of queries.</p><p>The next $q$ lines contain a single query of the $1$-st or $2$-nd type. The $1$-st type query consists of three integers $1$, $l$ and $r$ $(1 \le l \le r \le n)$, the $2$-nd type query consists of two integers $2$ and $x$ $(1 \le x \le 10^5)$.</p><p>It is guaranteed that all requests of the $2$-nd type are possible to process.</p></div><div class="output-specification"><p>For each query of the $1$-st type, output on a separate line one integer&nbsp;！ the required sum.</p></div>

## Input

<p>The first line contains two integers $n$ ($2 \le n \le 2 \cdot 10^5$) and $q$ ($1 \le q \le 2 \cdot 10^5$), where $n$&nbsp;！ the length of the initial permutation, and $q$&nbsp;！ the number of queries.</p><p>The next $q$ lines contain a single query of the $1$-st or $2$-nd type. The $1$-st type query consists of three integers $1$, $l$ and $r$ $(1 \le l \le r \le n)$, the $2$-nd type query consists of two integers $2$ and $x$ $(1 \le x \le 10^5)$.</p><p>It is guaranteed that all requests of the $2$-nd type are possible to process.</p>

## Output

<p>For each query of the $1$-st type, output on a separate line one integer&nbsp;！ the required sum.</p>

## Samples

```input1
4 4
1 2 4
2 3
1 1 2
1 3 4
```

```output1
9
4
6
```




## Note

<p>Initially, the permutation has the form $[1, 2, 3, 4]$. Queries processing is as follows: </p><ol> <li> $2 + 3 + 4 = 9$; </li><li> $[1, 2, 3, 4] \rightarrow [1, 2, 4, 3] \rightarrow [1, 3, 2, 4] \rightarrow [1, 3, 4, 2]$; </li><li> $1 + 3 = 4$; </li><li> $4 + 2 = 6$ </li></ol>
