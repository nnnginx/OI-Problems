## Description

<div><p>You are given a set $S$, which contains the first $n$ positive integers: $1, 2, \ldots, n$.</p><p>You can perform the following operation on $S$ any number of times (possibly zero): </p><ul> <li> Choose a positive integer $k$ where $1 \le k \le n$, such that there exists a multiple of $k$ in $S$. Then, delete the <span class="tex-font-style-bf">smallest</span> multiple of $k$ from $S$. This operation requires a cost of $k$. </li></ul><p>You are given a set $T$, which is a subset of $S$. Find the minimum possible total cost of operations such that $S$ would be transformed into $T$. We can show that such a transformation is always possible.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;�� the number of test cases. The description of the test cases follows.</p><p>The first line contains a single positive integer $n$ ($1 \le n \le 10^6$).</p><p>The second line of each test case contains a binary string of length $n$, describing the set $T$. The $i$-th character of the string is '<span class="tex-font-style-tt">1</span>' if and only if $i$ is an element of $T$, and '<span class="tex-font-style-tt">0</span>' otherwise.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$. </p></div><div class="output-specification"><p>For each test case, output one non-negative integer&nbsp;�� the minimum possible total cost of operations such that $S$ would be transformed into $T$.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;�� the number of test cases. The description of the test cases follows.</p><p>The first line contains a single positive integer $n$ ($1 \le n \le 10^6$).</p><p>The second line of each test case contains a binary string of length $n$, describing the set $T$. The $i$-th character of the string is '<span class="tex-font-style-tt">1</span>' if and only if $i$ is an element of $T$, and '<span class="tex-font-style-tt">0</span>' otherwise.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$. </p>

## Output

<p>For each test case, output one non-negative integer&nbsp;�� the minimum possible total cost of operations such that $S$ would be transformed into $T$.</p>





```input1|2,3,6,7,10,11
6
6
111111
7
1101001
4
0000
4
0010
8
10010101
15
110011100101100
```




```output1
0
11
4
4
17
60
```



## Note

<p>In the first test case, we shall not perform any operations as $S$ is already equal to $T$, which is the set $\{1, 2, 3, 4, 5, 6\}$.</p><p>In the second test case, initially, $S = \{1, 2, 3, 4, 5, 6, 7\}$, and $T = \{1, 2, 4, 7\}$. We shall perform the following operations: </p><ol> <li> Choose $k=3$, then delete $3$ from $S$. </li><li> Choose $k=3$, then delete $6$ from $S$. </li><li> Choose $k=5$, then delete $5$ from $S$. </li></ol><p>The total cost is $3+3+5 = 11$. It can be shown that this is the smallest cost possible.</p><p>In the third test case, initially, $S = \{1, 2, 3, 4\}$ and $T = \{\}$ (empty set). We shall perform $4$ operations of $k=1$ to delete $1$, $2$, $3$, and $4$.</p><p>In the fourth test case, initially, $S = \{1, 2, 3, 4\}$ and $T = \{3\}$. We shall perform two operations with $k=1$ to delete $1$ and $2$, then perform one operation with $k=2$ to delete $4$.</p>
