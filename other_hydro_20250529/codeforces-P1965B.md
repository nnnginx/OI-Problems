## Description

<div><p>You are given two integers $n$ and $k$. Find a sequence $a$ of non-negative integers of size at most $25$ such that the following conditions hold.</p><ul> <li> There is no subsequence of $a$ with a sum of $k$. </li><li> For all $1 \le v \le n$ where $v \ne k$, there is a subsequence of $a$ with a sum of $v$. </li></ul><p>A sequence $b$ is a subsequence of $a$ if $b$ can be obtained from $a$ by the deletion of several (possibly, zero or all) elements, without changing the order of the remaining elements. For example, $[5, 2, 3]$ is a subsequence of $[1, 5, 7, 8, 2, 4, 3]$.</p><p>It can be shown that under the given constraints, a solution always exists.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>Each test case consists of a single line containing two integers $n$ and $k$ ($2 \le n \le 10^6$, $1 \le k \le n$)&nbsp;！ the parameters described above. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^7$.</p></div><div class="output-specification"><p>The first line of output for each test case should contain a single integer $m$ ($1 \le m \le 25$)&nbsp;！ the size of your chosen sequence.</p><p>The second line of output for each test case should contain $m$ integers $a_i$ ($0 \le a_i \le 10^9$)&nbsp;！ the elements of your chosen sequence.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>Each test case consists of a single line containing two integers $n$ and $k$ ($2 \le n \le 10^6$, $1 \le k \le n$)&nbsp;！ the parameters described above. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^7$.</p>

## Output

<p>The first line of output for each test case should contain a single integer $m$ ($1 \le m \le 25$)&nbsp;！ the size of your chosen sequence.</p><p>The second line of output for each test case should contain $m$ integers $a_i$ ($0 \le a_i \le 10^9$)&nbsp;！ the elements of your chosen sequence.</p><p>If there are multiple solutions, print any.</p>





```input1|2,4,6
5
2 2
6 1
8 8
9 3
10 7
```




```output1
1
1
5
2 3 4 5 6
7
1 1 1 1 1 1 1
4
7 1 4 1
4
1 2 8 3
```



## Note

<p>In the first example, we just need a subsequence that adds up to $1$, but not one that adds up to $2$. So the array $a=[1]$ suffices.</p><p>In the second example, all elements are greater than $k=1$, so no subsequence adds up to $1$. Every other integer between $1$ and $n$ is present in the array, so there is a subsequence of size $1$ adding up to each of those numbers.</p>
