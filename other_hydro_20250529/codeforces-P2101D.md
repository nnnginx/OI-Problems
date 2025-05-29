## Description

<div><p>    </p><p>An array $b$ of length $|b|$ is <span class="tex-font-style-it">cute</span> if the sum of the length of its Longest Increasing Subsequence (LIS) and the length of its Longest Decreasing Subsequence (LDS)$^{\text{∗}}$ is <span class="tex-font-style-bf">exactly</span> one more than the length of the array. More formally, the array $b$ is cute if $\operatorname{LIS}(b) + \operatorname{LDS}(b) = |b| + 1$.</p><p>You are given a permutation $a$ of length $n$$^{\text{†}}$. Your task is to count the number of non-empty subarrays$^{\text{‡}}$ of permutation $a$ that are cute.</p><div class="statement-footnote"><p>$^{\text{∗}}$A sequence $x$ is a subsequence of a sequence $y$ if $x$ can be obtained from $y$ by the deletion of several (possibly, zero or all) element from arbitrary positions. </p><p>The longest increasing (decreasing) subsequence of an array is the longest subsequence such that its elements are ordered in strictly increasing (decreasing) order.</p><p>$^{\text{†}}$A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array). </p><p>$^{\text{‡}}$An array $x$ is a subarray of an array $y$ if $x$ can be obtained from $y$ by the deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2 \cdot 10^5 $)&nbsp;— the length of permutation $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of permutation $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, output the number of cute non-empty subarrays of permutation $a$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 2 \cdot 10^5 $)&nbsp;— the length of permutation $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of permutation $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case, output the number of cute non-empty subarrays of permutation $a$.</p>





```input1|2,3,6,7,10,11
5
3
3 1 2
5
2 3 4 5 1
4
3 4 1 2
7
1 2 3 4 5 6 7
10
7 8 2 4 5 10 1 3 6 9
```




```output1
6
15
9
28
36
```



## Note

<p>In the first test case, all of the $6$ non-empty subarrays are cute:</p><ul><li> $[3]$: $\operatorname{LIS}([3]) + \operatorname{LDS}([3]) = 1 + 1 = 2$.</li><li> $[1]$: $\operatorname{LIS}([1]) + \operatorname{LDS}([1]) = 1 + 1 = 2$.</li><li> $[2]$: $\operatorname{LIS}([2]) + \operatorname{LDS}([2]) = 1 + 1 = 2$.</li><li> $[3, 1]$: $\operatorname{LIS}([3, 1]) + \operatorname{LDS}([3, 1]) = 1 + 2 = 3$.</li><li> $[1, 2]$: $\operatorname{LIS}([1, 2]) + \operatorname{LDS}([1, 2]) = 2 + 1 = 3$.</li><li> $[3, 1, 2]$: $\operatorname{LIS}([3, 1, 2]) + \operatorname{LDS}([3, 1, 2]) = 2 + 2 = 4$.</li></ul><p>In the second test case, one of the cute subarrays is $[2, 3, 4, 5, 1]$ as $\operatorname{LIS}([2, 3, 4, 5, 1]) = 4$ and $\operatorname{LDS}([2, 3, 4, 5, 1]) = 2$, which satisfies $4 + 2 = 5 + 1$.</p>
