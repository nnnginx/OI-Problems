## Description

<div><p>You are given an array $a$ consisting of $n$ integers.</p><p>Let the function $f(b)$ return the minimum number of operations needed to make an array $b$ a palindrome. The operations you can make are:</p><ul> <li> choose two adjacent elements $b_i$ and $b_{i+1}$, remove them, and replace them with a single element equal to $(b_i + b_{i + 1})$; </li><li> or choose an element $b_i &gt; 1$, remove it, and replace it with two positive integers $x$ and $y$ ($x &gt; 0$ and $y &gt; 0$) such that $x + y = b_i$. </li></ul><p>For example, from an array $b=[2, 1, 3]$, you can obtain the following arrays in one operation: $[1, 1, 1, 3]$, $[2, 1, 1, 2]$, $[3, 3]$, $[2, 4]$, or $[2, 1, 2, 1]$.</p><p>Calculate $\displaystyle \left(\sum_{1 \le l \le r \le n}{f(a[l..r])}\right)$, where $a[l..r]$ is the subarray of $a$ from index $l$ to index $r$, inclusive. In other words, find the sum of the values of the function $f$ for all subarrays of the array $a$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;�� the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$).</p><p>Additional constraint on the input: the sum of $n$ over all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;�� the sum of the values of the function $f$ for all subarrays of the array $a$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;�� the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$).</p><p>Additional constraint on the input: the sum of $n$ over all test cases does not exceed $2000$.</p>

## Output

<p>For each test case, print a single integer&nbsp;�� the sum of the values of the function $f$ for all subarrays of the array $a$.</p>





```input1|2,3,6,7
4
3
2 1 3
4
1 1 1 1
5
4 2 3 1 5
4
1 2 1 2
```




```output1
3
0
14
5
```


