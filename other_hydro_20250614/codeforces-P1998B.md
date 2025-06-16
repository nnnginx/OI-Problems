## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">It is known that <a href="https://usaco.org/index.php?page=viewproblem2&amp;cpid=1421">Farmer John likes Permutations</a>, but I like them too!</span></div><div class="epigraph-source">— Sun Tzu, <span class="tex-font-style-it">The Art of Constructing Permutations</span></div></div><p>You are given a permutation$^{\text{∗}}$ $p$ of length $n$.</p><p>Find a permutation $q$ of length $n$ that minimizes the number of pairs ($i, j$) ($1 \leq i \leq j \leq n$) such that $p_i + p_{i+1} + \ldots + p_j = q_i + q_{i+1} + \ldots + q_j$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains $n$ ($1 \leq n \leq 2 \cdot 10^5$).</p><p>The following line contains $n$ space-separated integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$)&nbsp;— denoting the permutation $p$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output one line containing any permutation of length $n$ (the permutation $q$) such that $q$ minimizes the number of pairs.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains $n$ ($1 \leq n \leq 2 \cdot 10^5$).</p><p>The following line contains $n$ space-separated integers $p_1, p_2, \ldots, p_n$ ($1 \leq p_i \leq n$)&nbsp;— denoting the permutation $p$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output one line containing any permutation of length $n$ (the permutation $q$) such that $q$ minimizes the number of pairs.</p>





```input1|2,3,6,7
3
2
1 2
5
1 2 3 4 5
7
4 7 5 1 2 6 3
```




```output1
2 1
3 5 4 2 1
6 2 1 4 7 3 5
```



## Note

<p>For the first test, there exists only one pair ($i, j$) ($1 \leq i \leq j \leq n$) such that $p_i + p_{i+1} + \ldots + p_j = q_i + q_{i+1} + \ldots + q_j$, which is ($1, 2$). It can be proven that no such $q$ exists for which there are no pairs.</p>
