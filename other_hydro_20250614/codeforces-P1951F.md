## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://youtu.be/j_MlBCb9-m8"><span class="tex-font-style-it">My Chemical Romance - Disenchanted</span></a></div><div class="epigraph-source">ඞ</div></div><p>You are given a permutation $p$ of size $n$, as well as a non-negative integer $k$. You need to construct a permutation $q$ of size $n$ such that $\operatorname{inv}(q) + \operatorname{inv}(q \cdot p) = k {}^\dagger {}^\ddagger$, or determine if it is impossible to do so.</p><p>${}^\dagger$ For two permutations $p$ and $q$ of the same size $n$, the permutation $w = q \cdot p$ is such that $w_i = q_{p_i}$ for all $1 \le i \le n$.</p><p>${}^\ddagger$ For a permutation $p$ of size $n$, the function $\operatorname{inv}(p)$ returns the number of inversions of $p$, i.e. the number of pairs of indices $1 \le i &lt; j \le n$ such that $p_i &gt; p_j$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5, 0 \le k \le n(n - 1)$)&nbsp;— the size of $p$ and the target number of inversions.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, $p_i$'s are pairwise distinct)&nbsp;— the given permutation $p$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print on one line <span class="tex-font-style-tt">"YES"</span> if there exists a permutation $q$ that satisfies the given condition, or <span class="tex-font-style-tt">"NO"</span> if there is no such permutation.</p><p>If the answer is <span class="tex-font-style-tt">"YES"</span>, on the second line, print $n$ integers $q_1, q_2, \ldots, q_n$ that represent such a satisfactory permutation $q$. If there are multiple such $q$'s, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5, 0 \le k \le n(n - 1)$)&nbsp;— the size of $p$ and the target number of inversions.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, $p_i$'s are pairwise distinct)&nbsp;— the given permutation $p$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print on one line <span class="tex-font-style-tt">"YES"</span> if there exists a permutation $q$ that satisfies the given condition, or <span class="tex-font-style-tt">"NO"</span> if there is no such permutation.</p><p>If the answer is <span class="tex-font-style-tt">"YES"</span>, on the second line, print $n$ integers $q_1, q_2, \ldots, q_n$ that represent such a satisfactory permutation $q$. If there are multiple such $q$'s, print any of them.</p>





```input1|2,3,6,7,10,11
5
3 4
2 3 1
5 5
2 3 5 1 4
6 11
5 1 2 3 4 6
9 51
3 1 4 2 5 6 7 8 9
1 0
1
```




```output1
YES
3 2 1
NO
NO
YES
1 5 9 8 7 6 4 3 2
YES
1
```



## Note

<p>In the first test case, we have $q \cdot p = [2, 1, 3]$, $\operatorname{inv}(q) = 3$, and $\operatorname{inv}(q \cdot p) = 1$.</p><p>In the fourth test case, we have $q \cdot p = [9, 1, 8, 5, 7, 6, 4, 3, 2]$, $\operatorname{inv}(q) = 24$, and $\operatorname{inv}(q \cdot p) = 27$.</p>
