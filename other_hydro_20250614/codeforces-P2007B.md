## Description

<div><p>After receiving yet another integer array $a_1, a_2, \ldots, a_n$ at her birthday party, Index decides to perform some operations on it.</p><p>Formally, there are $m$ operations that she is going to perform in order. Each of them belongs to one of the two types:</p><ul> <li> $\texttt{+ l r}$. Given two integers $l$ and $r$, for all $1 \leq i \leq n$ such that $l \leq a_i \leq r$, set $a_i := a_i + 1$. </li><li> $\texttt{- l r}$. Given two integers $l$ and $r$, for all $1 \leq i \leq n$ such that $l \leq a_i \leq r$, set $a_i := a_i - 1$. </li></ul><p>For example, if the initial array $a = [7, 1, 3, 4, 3]$, after performing the operation $\texttt{+} \space 2 \space 4$, the array $a = [7, 1, 4, 5, 4]$. Then, after performing the operation $\texttt{-} \space 1 \space 10$, the array $a = [6, 0, 3, 4, 3]$.</p><p>Index is curious about the maximum value in the array $a$. Please help her find it after each of the $m$ operations.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 2 \cdot 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n \leq 10^5$, $1 \leq m \leq 10^5$)&nbsp;！ the length of the array and the number of operations.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the initial array $a$.</p><p>Then $m$ lines follow, each line corresponds to the operation, in the following format: $\texttt{c l r}$ ($c \in \{\texttt +, \texttt -\}$, $l$ and $r$ are integers, $1 \leq l \leq r \leq 10^9$)&nbsp;！ the description of the operation.</p><p>Note that the elements $a_i$ <span class="tex-font-style-bf">may not satisfy</span> $1\le a_i\le 10^9$ after some operations, as it is shown in the example.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$, and the sum of $m$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output one single line containing $m$ integers, with the $i$-th of them describing the maximum value of the array after the $i$-th operation.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 2 \cdot 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n \leq 10^5$, $1 \leq m \leq 10^5$)&nbsp;！ the length of the array and the number of operations.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;！ the initial array $a$.</p><p>Then $m$ lines follow, each line corresponds to the operation, in the following format: $\texttt{c l r}$ ($c \in \{\texttt +, \texttt -\}$, $l$ and $r$ are integers, $1 \leq l \leq r \leq 10^9$)&nbsp;！ the description of the operation.</p><p>Note that the elements $a_i$ <span class="tex-font-style-bf">may not satisfy</span> $1\le a_i\le 10^9$ after some operations, as it is shown in the example.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$, and the sum of $m$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output one single line containing $m$ integers, with the $i$-th of them describing the maximum value of the array after the $i$-th operation.</p>





```input1|2,3,4,5,6,7,8,16,17,18,19,20,21,22,26,27,28
5
5 5
1 2 3 2 1
+ 1 3
- 2 3
+ 1 2
+ 2 4
- 6 8
5 5
1 3 3 4 5
+ 1 4
+ 2 3
- 4 5
- 3 3
- 2 6
5 5
1 1 1 1 1
+ 2 3
- 4 5
+ 1 6
- 2 5
+ 1 8
1 1
1
- 1 1
1 1
1000000000
+ 1000000000 1000000000
```




```output1
4 4 4 5 5
5 5 4 4 3
1 1 2 1 2
0
1000000001
```



## Note

<p>In the first test case, the process of the operations is listed below:</p><ul> <li> After the first operation, the array becomes equal $[2,3,4,3,2]$. The maximum value is $4$. </li><li> After the second operation, the array becomes equal $[1,2,4,2,1]$. The maximum value is $4$. </li><li> After the third operation, the array becomes equal $[2,3,4,3,2]$. The maximum value is $4$. </li><li> After the fourth operation, the array becomes equal $[3,4,5,4,3]$. The maximum value is $5$. </li><li> After the fifth operation, the array becomes equal $[3,4,5,4,3]$. The maximum value is $5$.</li></ul><p>In the second test case, the process of the operations is listed below:</p><ul> <li> After the first operation, the array becomes equal $[2,4,4,5,5]$. The maximum value is $5$. </li><li> After the second operation, the array becomes equal $[3,4,4,5,5]$. The maximum value is $5$. </li><li> After the third operation, the array becomes equal $[3,3,3,4,4]$. The maximum value is $4$. </li><li> After the fourth operation, the array becomes equal $[2,2,2,4,4]$. The maximum value is $4$. </li><li> After the fifth operation, the array becomes equal $[1,1,1,3,3]$. The maximum value is $3$.</li></ul>
