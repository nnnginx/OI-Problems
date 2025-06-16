## Description

<div><p>Little R is a magician who likes non-decreasing arrays. She has an array of length $n$, initially as $a_1, \ldots, a_n$, in which each element is an integer between $[1, m]$. She wants it to be non-decreasing, i.e., $a_1 \leq a_2 \leq \ldots \leq a_n$.</p><p>To do this, she can perform several magic tricks. Little R has a fixed array $b_1\ldots b_m$ of length $m$. Formally, let's define a trick as a procedure that does the following things in order:</p><ul> <li> Choose a set $S \subseteq \{1, 2, \ldots, n\}$. </li><li> For each $u \in S$, assign $a_u$ with $b_{a_u}$. </li></ul><p>Little R wonders how many tricks are needed at least to make the initial array non-decreasing. If it is not possible with any amount of tricks, print $-1$ instead.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1\leq n \leq 10^6$, $1 \leq m \leq 10^6$)&nbsp;！ the length of the initial array and the range of the elements in the array.</p><p>The second line of each test case contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq m$)&nbsp;！ the initial array.</p><p>The third line of each test case contains $m$ integers $b_1, \ldots, b_m$ ($1 \leq b_i \leq m$)&nbsp;！ the fixed magic array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$ and the sum of $m$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output a single integer: the minimum number of tricks needed, or $-1$ if it is impossible to make $a_1, \ldots, a_n$ non-decreasing.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1\leq n \leq 10^6$, $1 \leq m \leq 10^6$)&nbsp;！ the length of the initial array and the range of the elements in the array.</p><p>The second line of each test case contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq m$)&nbsp;！ the initial array.</p><p>The third line of each test case contains $m$ integers $b_1, \ldots, b_m$ ($1 \leq b_i \leq m$)&nbsp;！ the fixed magic array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$ and the sum of $m$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output a single integer: the minimum number of tricks needed, or $-1$ if it is impossible to make $a_1, \ldots, a_n$ non-decreasing.</p>





```input1|2,3,4,8,9,10
3
5 8
1 6 3 7 1
2 3 5 8 7 1 5 6
3 3
1 3 2
2 1 3
10 10
2 8 5 4 8 4 1 5 10 10
6 7 2 6 3 4 1 1 3 5
```




```output1
3
-1
3
```



## Note

<p>In the first case, the initial array $a_1, \ldots, a_n$ is $[1, 6, 3, 7, 1]$. You can choose $S$ as follows: </p><ul> <li> first trick: $S = [2, 4, 5]$, $a = [1, 1, 3, 5, 2]$; </li><li> second trick: $S = [5]$, $a = [1, 1, 3, 5, 3]$; </li><li> third trick: $S = [5]$, $a = [1, 1, 3, 5, 5]$. </li></ul> So it is possible to make $a_1, \ldots, a_n$ non-decreasing using $3$ tricks. It can be shown that this is the minimum possible amount of tricks.<p>In the second case, it is impossible to make $a_1, \ldots, a_n$ non-decreasing.</p>
