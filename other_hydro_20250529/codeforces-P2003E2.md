## Description

<div><p><span class="tex-font-style-bf">This is a hard version of this problem. The differences between the versions are the constraint on $m$ and $r_i &lt; l_{i + 1}$ holds for each $i$ from $1$ to $m - 1$ in the easy version. You can make hacks only if both versions of the problem are solved.</span></p><p>Turtle gives you $m$ intervals $[l_1, r_1], [l_2, r_2], \ldots, [l_m, r_m]$. He thinks that a permutation $p$ is interesting if there exists an integer $k_i$ for every interval ($l_i \le k_i &lt; r_i$), and if he lets $a_i = \max\limits_{j = l_i}^{k_i} p_j, b_i = \min\limits_{j = k_i + 1}^{r_i} p_j$ for every integer $i$ from $1$ to $m$, the following condition holds:</p><p>$$\max\limits_{i = 1}^m a_i &lt; \min\limits_{i = 1}^m b_i$$</p><p>Turtle wants you to calculate the maximum number of inversions of all interesting permutations of length $n$, or tell him if there is no interesting permutation.</p><p>An inversion of a permutation $p$ is a pair of integers $(i, j)$ ($1 \le i &lt; j \le n$) such that $p_i &gt; p_j$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n, m$ ($2 \le n \le 5 \cdot 10^3, 0 \le m \le 5 \cdot 10^3$) ！ the length of the permutation and the number of intervals.</p><p>The $i$-th of the following $m$ lines contains two integers $l_i, r_i$ ($1 \le l_i &lt; r_i \le n$) ！ the $i$-th interval. Note that there may exist identical intervals (i.e., there may exist two different indices $i, j$ such that $l_i = l_j$ and $r_i = r_j$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^3$ and the sum of $m$ over all test cases does not exceed $5 \cdot 10^3$.</p></div><div class="output-specification"><p>For each test case, if there is no interesting permutation, output a single integer $-1$.</p><p>Otherwise, output a single integer ！ the maximum number of inversions.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n, m$ ($2 \le n \le 5 \cdot 10^3, 0 \le m \le 5 \cdot 10^3$) ！ the length of the permutation and the number of intervals.</p><p>The $i$-th of the following $m$ lines contains two integers $l_i, r_i$ ($1 \le l_i &lt; r_i \le n$) ！ the $i$-th interval. Note that there may exist identical intervals (i.e., there may exist two different indices $i, j$ such that $l_i = l_j$ and $r_i = r_j$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^3$ and the sum of $m$ over all test cases does not exceed $5 \cdot 10^3$.</p>

## Output

<p>For each test case, if there is no interesting permutation, output a single integer $-1$.</p><p>Otherwise, output a single integer ！ the maximum number of inversions.</p>





```input1|2,5,6,11,12,13,18,19,20,21,22
8
2 0
2 1
1 2
5 1
2 4
8 3
1 4
2 5
7 8
7 2
1 4
4 7
7 3
1 2
1 7
3 7
7 4
1 3
4 7
1 3
4 7
7 3
1 2
3 4
5 6
```




```output1
1
0
8
18
-1
-1
15
15
```



## Note

<p>In the third test case, the interesting permutation with the maximum number of inversions is $[5, 2, 4, 3, 1]$.</p><p>In the fourth test case, the interesting permutation with the maximum number of inversions is $[4, 3, 8, 7, 6, 2, 1, 5]$. In this case, we can let $[k_1, k_2, k_3] = [2, 2, 7]$.</p><p>In the fifth and the sixth test case, it can be proven that there is no interesting permutation.</p><p>In the seventh test case, the interesting permutation with the maximum number of inversions is $[4, 7, 6, 3, 2, 1, 5]$. In this case, we can let $[k_1, k_2, k_3, k_4] = [1, 6, 1, 6]$.</p><p>In the eighth test case, the interesting permutation with the maximum number of inversions is $[4, 7, 3, 6, 2, 5, 1]$.</p>
