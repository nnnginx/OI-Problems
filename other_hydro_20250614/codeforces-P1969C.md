## Description

<div><p>You are given an integer array $a$ of length $n$.</p><p>You can perform the following operation: choose an element of the array and replace it with any of its neighbor's value.</p><p>For example, if $a=[3, 1, 2]$, you can get one of the arrays $[3, 3, 2]$, $[3, 2, 2]$ and $[1, 1, 2]$ using one operation, but not $[2, 1, 2$] or $[3, 4, 2]$. </p><p>Your task is to calculate the minimum possible total sum of the array if you can perform the aforementioned operation at most $k$ times.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5$; $0 \le k \le 10$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the minimum possible total sum of the array if you can perform the aforementioned operation at most $k$ times.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 3 \cdot 10^5$; $0 \le k \le 10$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>Additional constraint on the input: the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the minimum possible total sum of the array if you can perform the aforementioned operation at most $k$ times.</p>





```input1|2,3,6,7
4
3 1
3 1 2
1 3
5
4 2
2 2 1 3
6 3
4 1 2 2 4 3
```




```output1
4
5
5
10
```



## Note

<p>In the first example, one of the possible sequences of operations is the following: $[3, 1, 2] \rightarrow [1, 1, 2$].</p><p>In the second example, you do not need to apply the operation.</p><p>In the third example, one of the possible sequences of operations is the following: $[2, 2, 1, 3] \rightarrow [2, 1, 1, 3] \rightarrow [2, 1, 1, 1]$.</p><p>In the fourth example, one of the possible sequences of operations is the following: $[4, 1, 2, 2, 4, 3] \rightarrow [1, 1, 2, 2, 4, 3] \rightarrow [1, 1, 1, 2, 4, 3] \rightarrow [1, 1, 1, 2, 2, 3]$.</p>
