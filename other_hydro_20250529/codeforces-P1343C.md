## Description

<div><p>Recall that the sequence $b$ is a a subsequence of the sequence $a$ if $b$ can be derived from $a$ by removing zero or more elements without changing the order of the remaining elements. For example, if $a=[1, 2, 1, 3, 1, 2, 1]$, then possible subsequences are: $[1, 1, 1, 1]$, $[3]$ and $[1, 2, 1, 3, 1, 2, 1]$, but not $[3, 2, 3]$ and $[1, 1, 1, 1, 2]$.</p><p>You are given a sequence $a$ consisting of $n$ positive and negative elements (there is no zeros in the sequence).</p><p>Your task is to choose <span class="tex-font-style-bf">maximum by size</span> (length) <span class="tex-font-style-it">alternating</span> subsequence of the given sequence (i.e. the sign of each next element is the opposite from the sign of the current element, like positive-negative-positive and so on or negative-positive-negative and so on). Among all such subsequences, you have to choose one which has the <span class="tex-font-style-bf">maximum sum</span> of elements.</p><p>In other words, if the maximum length of <span class="tex-font-style-it">alternating</span> subsequence is $k$ then your task is to find the <span class="tex-font-style-bf">maximum sum</span> of elements of some <span class="tex-font-style-it">alternating</span> subsequence of length $k$.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of elements in $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9, a_i \ne 0$), where $a_i$ is the $i$-th element of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer ！ the <span class="tex-font-style-bf">maximum sum</span> of the <span class="tex-font-style-bf">maximum by size</span> (length) <span class="tex-font-style-it">alternating</span> subsequence of $a$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of elements in $a$. The second line of the test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9, a_i \ne 0$), where $a_i$ is the $i$-th element of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer ！ the <span class="tex-font-style-bf">maximum sum</span> of the <span class="tex-font-style-bf">maximum by size</span> (length) <span class="tex-font-style-it">alternating</span> subsequence of $a$.</p>

## Samples

```input1
4
5
1 2 3 -1 -2
4
-1 -2 -1 -3
10
-2 8 3 8 -4 -15 5 -2 -3 1
6
1 -1000000000 1 -1000000000 1 -1000000000
```

```output1
2
-1
6
-2999999997
```




## Note

<p>In the first test case of the example, one of the possible answers is $[1, 2, \underline{3}, \underline{-1}, -2]$.</p><p>In the second test case of the example, one of the possible answers is $[-1, -2, \underline{-1}, -3]$.</p><p>In the third test case of the example, one of the possible answers is $[\underline{-2}, 8, 3, \underline{8}, \underline{-4}, -15, \underline{5}, \underline{-2}, -3, \underline{1}]$.</p><p>In the fourth test case of the example, one of the possible answers is $[\underline{1}, \underline{-1000000000}, \underline{1}, \underline{-1000000000}, \underline{1}, \underline{-1000000000}]$.</p>
