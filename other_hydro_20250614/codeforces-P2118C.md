## Description

<div><p>You are given an array $a$ of $n$ integers. We define the $\text{beauty}$ of a number $x$ to be the number of $1$ bits in its binary representation. We define the beauty of an array to be the sum of beauties of the numbers it contains. </p><p>In one operation, you can select an index $i$&nbsp;$(1 \le i \le n)$ and increase $a_i$ by $1$. </p><p>Find the maximum beauty of the array after doing <span class="tex-font-style-bf">at most</span> $k$ operations.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 5000$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 5000$, $0 \le k \le 10^{18}$)&nbsp;！ the length of the array and the maximal number of operations. </p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots a_n$ ($0 \le a_i \le 10^9$)&nbsp;！denoting the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each test case, output a single integer, the maximum beauty after at most $k$ operations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 5000$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 5000$, $0 \le k \le 10^{18}$)&nbsp;！ the length of the array and the maximal number of operations. </p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots a_n$ ($0 \le a_i \le 10^9$)&nbsp;！denoting the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p>

## Output

<p>For each test case, output a single integer, the maximum beauty after at most $k$ operations.</p>





```input1|2,3,6,7,10,11
5
5 2
0 1 7 2 4
5 3
0 1 7 2 4
1 1
3
3 0
2 0 3
1 100000000000
0
```




```output1
8
9
2
3
36
```



## Note

<p>In the first test case, $a = [0, 1, 7, 2, 4]$. </p><ul> <li> apply the first operation at $i = 1$, the new array is $a = [1, 1, 7, 2, 4]$ </li><li> apply the second operation at $i = 4$, the new array is $a = [1, 1, 7, 3, 4]$ </li></ul> The beauty of this array is $1 + 1 + 3 + 2 + 1 = 8$. One of the other valid solutions with the same beauty is $[0, 1, 7, 3, 5]$.<p>In the third test case, $a = [3]$. Since you are not required to use exactly $k$ operations, it is optimal to do none.</p>
