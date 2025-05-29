## Description

<div><p>You are given an array $a$ of length $n$ and a number $k$.</p><p>A subarray is defined as a sequence of one or more consecutive elements of the array. You need to split the array $a$ into $k$ non-overlapping subarrays $b_1, b_2, \dots, b_k$ such that the union of these subarrays equals the entire array. Additionally, you need to maximize the value of $x$, which is equal to the minimum MEX$(b_i)$, for $i \in [1..k]$.</p><p>MEX$(v)$ denotes the smallest non-negative integer that is not present in the array $v$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ $(1\leq t\leq 10^4)$ &nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ $(1\leq k \leq n \leq 2 \cdot 10^5)$ &nbsp;！ the length of the array and the number of segments to split the array into.</p><p>The second line of each test case contains $n$ integers $a_i$ $(0\leq a_i\leq 10^9)$ &nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each query, output a single number &nbsp;！ the maximum value $x$ such that there exists a partition of the array $a$ into $k$ subarrays where the minimum MEX equals $x$.</p></div>

## Input

<p>The first line contains an integer $t$ $(1\leq t\leq 10^4)$ &nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$, $k$ $(1\leq k \leq n \leq 2 \cdot 10^5)$ &nbsp;！ the length of the array and the number of segments to split the array into.</p><p>The second line of each test case contains $n$ integers $a_i$ $(0\leq a_i\leq 10^9)$ &nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each query, output a single number &nbsp;！ the maximum value $x$ such that there exists a partition of the array $a$ into $k$ subarrays where the minimum MEX equals $x$.</p>





```input1|2,3,6,7,10,11,14,15
7
1 1
0
5 1
0 1 3 2 4
6 2
2 1 0 0 1 2
5 5
0 0 0 0 0
5 2
2 3 4 5 6
6 2
0 0 1 1 2 2
4 4
1 0 0 0
```




```output1
1
5
3
1
0
1
0
```


