## Description

<div><p>To help those contestants who struggle a lot in contests, the headquarters of Codeforces are planning to introduce Division 5. In this new division, the tags of all problems will be announced prior to the round to help the contestants.</p><p>The contest consists of $n$ problems, where the tag of the $i$-th problem is denoted by an integer $a_i$.</p><p>You want to AK (solve all problems). To do that, you must solve the problems in some order. To make the contest funnier, you created extra limitations on yourself. You do not want to solve two problems consecutively with the same tag since it is boring. Also, you are afraid of big jumps in difficulties while solving them, so you want to minimize the number of times that you solve two problems consecutively that are not adjacent in the contest order.</p><p>Formally, your solve order can be described by a permutation $p$ of length $n$. The <span class="tex-font-style-bf">cost</span> of a permutation is defined as the number of indices $i$ ($1\le i&lt;n$) where $|p_{i+1}-p_i|&gt;1$. You have the requirement that $a_{p_i}\ne a_{p_{i+1}}$ for all $1\le i&lt; n$.</p><p>You want to know the minimum possible cost of permutation that satisfies the requirement. If no permutations meet this requirement, you should report about it.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\leq t\leq 10^4$) ！ the number of test cases.</p><p>The first line of the description of each test case contains a single integer $n$ ($1 \le n \le 10^5$) ！ the number of problems in the contest.</p><p>The next line contains $n$ integers $a_1,a_2,\ldots a_n$ ($1 \le a_i \le n$) ！ the tags of the problems.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if there are no permutations that satisfy the required condition, print $-1$. Otherwise, print the minimum possible cost of a permutation that satisfies the required condition.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\leq t\leq 10^4$) ！ the number of test cases.</p><p>The first line of the description of each test case contains a single integer $n$ ($1 \le n \le 10^5$) ！ the number of problems in the contest.</p><p>The next line contains $n$ integers $a_1,a_2,\ldots a_n$ ($1 \le a_i \le n$) ！ the tags of the problems.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, if there are no permutations that satisfy the required condition, print $-1$. Otherwise, print the minimum possible cost of a permutation that satisfies the required condition.</p>

## Samples

```input1
4
6
2 1 2 3 1 1
5
1 1 1 2 2
8
7 7 2 7 7 1 8 7
10
1 2 3 4 1 1 2 3 4 1
```

```output1
1
3
-1
2
```




## Note

<p>In the first test case, let $p=[5, 4, 3, 2, 1, 6]$. The cost is $1$ because we jump from $p_5=1$ to $p_6=6$, and $|6-1|&gt;1$. This permutation is valid because we don't solve problems with the same tag twice in a row. We cannot find a permutation with a cost smaller than $1$.</p><p>In the second test case, let $p=[1,5,2,4,3]$. The cost is $3$ because $|p_2-p_1|&gt;1$, $|p_3-p_2|&gt;1$, and $|p_4-p_3|&gt;1$. The permutation is valid because we don't solve problems with the same tag twice in a row. We cannot find a permutation with a cost smaller than $3$.</p><p>In the third test case, for any order of solving the problems, we will solve two problems with the same tag consecutively, so the answer is $-1$.</p>
