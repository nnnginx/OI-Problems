## Description

<div><p>Let's call the <span class="tex-font-style-it">Manhattan value</span> of a permutation$^{\dagger}$ $p$ the value of the expression $|p_1 - 1| + |p_2 - 2| + \ldots + |p_n - n|$.</p><p>For example, for the permutation $[1, 2, 3]$, the Manhattan value is $|1 - 1| + |2 - 2| + |3 - 3| = 0$, and for the permutation $[3, 1, 2]$, the Manhattan value is $|3 - 1| + |1 - 2| + |2 - 3| = 2 + 1 + 1 = 4$.</p><p>You are given integers $n$ and $k$. Find a permutation $p$ of length $n$ such that its Manhattan value is equal to $k$, or determine that no such permutation exists.</p><p>$^{\dagger}$A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^{4}$) �� the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^{5}, 0 \le k \le 10^{12}$) �� the length of the permutation and the required Manhattan value.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^{5}$.</p></div><div class="output-specification"><p>For each test case, if there is no suitable permutation, output "<span class="tex-font-style-tt">No</span>". Otherwise, in the first line, output "<span class="tex-font-style-tt">Yes</span>", and in the second line, output $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$) �� a suitable permutation.</p><p>If there are multiple solutions, output any of them.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^{4}$) �� the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^{5}, 0 \le k \le 10^{12}$) �� the length of the permutation and the required Manhattan value.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^{5}$.</p>

## Output

<p>For each test case, if there is no suitable permutation, output "<span class="tex-font-style-tt">No</span>". Otherwise, in the first line, output "<span class="tex-font-style-tt">Yes</span>", and in the second line, output $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$) �� a suitable permutation.</p><p>If there are multiple solutions, output any of them.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,4,6,8
8
3 4
4 5
7 0
1 1000000000000
8 14
112 777
5 12
5 2
```




```output1
Yes
3 1 2
No
Yes
1 2 3 4 5 6 7
No
Yes
8 2 3 4 5 6 1 7
No
Yes
5 4 3 1 2
Yes
2 1 3 4 5
```



## Note

<p>In the first test case, the permutation $[3, 1, 2]$ is suitable, its Manhattan value is $|3 - 1| + |1 - 2| + |2 - 3| = 2 + 1 + 1 = 4$.</p><p>In the second test case, it can be proven that there is no permutation of length $4$ with a Manhattan value of $5$.</p><p>In the third test case, the permutation $[1,2,3,4,5,6,7]$ is suitable, its Manhattan value is $|1-1|+|2-2|+|3-3|+|4-4|+|5-5|+|6-6|+|7-7|=0$.</p>
