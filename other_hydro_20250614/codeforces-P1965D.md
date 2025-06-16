## Description

<div><p>There is a hidden array $a$ of $n$ positive integers. You know that $a$ is a <span class="tex-font-style-bf">palindrome</span>, or in other words, for all $1 \le i \le n$, $a_i = a_{n + 1 - i}$. You are given the sums of all but one of its distinct subarrays, in arbitrary order. The subarray whose sum is not given can be any of the $\frac{n(n+1)}{2}$ distinct subarrays of $a$.</p><p>Recover any possible palindrome $a$. The input is chosen such that there is always at least one array $a$ that satisfies the conditions.</p><p>An array $b$ is a subarray of $a$ if $b$ can be obtained from $a$ by the deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 200$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 1000$)&nbsp;！ the size of the array $a$.</p><p>The next line of each test case contains $\frac{n(n+1)}{2} - 1$ integers $s_i$ ($1\leq s_i \leq 10^9$)&nbsp;！ all but one of the subarray sums of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p><p>Additional constraint on the input: There is always at least one valid solution.</p><p><span class="tex-font-style-bf">Hacks are disabled for this problem.</span></p></div><div class="output-specification"><p>For each test case, print one line containing $n$ positive integers $a_1, a_2, \cdots a_n$&nbsp;！ any valid array $a$. Note that $a$ must be a palindrome.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 200$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 1000$)&nbsp;！ the size of the array $a$.</p><p>The next line of each test case contains $\frac{n(n+1)}{2} - 1$ integers $s_i$ ($1\leq s_i \leq 10^9$)&nbsp;！ all but one of the subarray sums of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p><p>Additional constraint on the input: There is always at least one valid solution.</p><p><span class="tex-font-style-bf">Hacks are disabled for this problem.</span></p>

## Output

<p>For each test case, print one line containing $n$ positive integers $a_1, a_2, \cdots a_n$&nbsp;！ any valid array $a$. Note that $a$ must be a palindrome.</p><p>If there are multiple solutions, print any.</p>





```input1|2,3,6,7,10,11,14,15
7
3
1 2 3 4 1
4
18 2 11 9 7 11 7 2 9
4
5 10 5 16 3 3 13 8 8
4
8 10 4 6 4 20 14 14 6
5
1 2 3 4 5 4 3 2 1 1 2 3 2 1
5
1 1 2 2 2 3 3 3 3 4 5 5 6 8
3
500000000 1000000000 500000000 500000000 1000000000
```




```output1
1 2 1 
7 2 2 7 
3 5 5 3 
6 4 4 6 
1 1 1 1 1 
2 1 2 1 2 
500000000 500000000 500000000
```



## Note

<p>For the first example case, the subarrays of $a = [1, 2, 1]$ are: </p><ul> <li> $[1]$ with sum $1$, </li><li> $[2]$ with sum $2$, </li><li> $[1]$ with sum $1$, </li><li> $[1, 2]$ with sum $3$, </li><li> $[2, 1]$ with sum $3$, </li><li> $[1, 2, 1]$ with sum $4$. </li></ul> So the full list of subarray sums is $1, 1, 2, 3, 3, 4$, and the sum that is missing from the input list is $3$.<p>For the second example case, the missing subarray sum is $4$, for the subarray $[2, 2]$.</p><p>For the third example case, the missing subarray sum is $13$, because there are two subarrays with sum $13$ ($[3, 5, 5]$ and $[5, 5, 3]$) but $13$ only occurs once in the input.</p>
