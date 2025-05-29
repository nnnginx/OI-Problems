## Description

<div><p>You are given a cyclic array $a_1, a_2, \ldots, a_n$.</p><p>You can perform the following operation on $a$ at most $n - 1$ times:</p><ul> <li> Let $m$ be the current size of $a$, you can choose any two adjacent elements where the previous one is no greater than the latter one (In particular, $a_m$ and $a_1$ are adjacent and $a_m$ is the previous one), and delete exactly one of them. In other words, choose an integer $i$ ($1 \leq i \leq m$) where $a_i \leq a_{(i \bmod m) + 1}$ holds, and delete exactly one of $a_i$ or $a_{(i \bmod m) + 1}$ from $a$. </li></ul><p>Your goal is to find the minimum number of operations needed to make all elements in $a$ equal.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$) ！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) ！ the elements of array $a$.</p></div><div class="output-specification"><p>For each test case, output a single line containing an integer: the minimum number of operations needed to make all elements in $a$ equal.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$) ！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) ！ the elements of array $a$.</p>

## Output

<p>For each test case, output a single line containing an integer: the minimum number of operations needed to make all elements in $a$ equal.</p>





```input1|2,3,6,7,10,11,14,15
7
1
1
3
1 2 3
3
1 2 2
5
5 4 3 2 1
6
1 1 2 2 3 3
8
8 7 6 3 8 7 6 3
6
1 1 4 5 1 4
```




```output1
0
2
1
4
4
6
3
```



## Note

<p>In the first test case, there is only one element in $a$, so we can't do any operation.</p><p>In the second test case, we can perform the following operations to make all elements in $a$ equal:</p><ul> <li> choose $i = 2$, delete $a_3$, then $a$ would become $[1, 2]$. </li><li> choose $i = 1$, delete $a_1$, then $a$ would become $[2]$. </li></ul><p>It can be proven that we can't make all elements in $a$ equal using fewer than $2$ operations, so the answer is $2$.</p>
