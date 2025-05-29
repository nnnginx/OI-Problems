## Description

<div><p>You are given an integer sequence $a_1, a_2, \ldots, a_n$. Let $S$ be the set of all possible non-empty subsequences of $a$ without duplicate elements. Your goal is to find the longest sequence in $S$. If there are multiple of them, find the one that minimizes lexicographical order after multiplying terms at odd positions by $-1$.</p><p>For example, given $a = [3, 2, 3, 1]$, $S = \{[1], [2], [3], [2, 1], [2, 3], [3, 1], [3, 2], [2, 3, 1], [3, 2, 1]\}$. Then $[2, 3, 1]$ and $[3, 2, 1]$ would be the longest, and $[3, 2, 1]$ would be the answer since $[-3, 2, -1]$ is lexicographically smaller than $[-2, 3, -1]$.</p><p>A sequence $c$ is a subsequence of a sequence $d$ if $c$ can be obtained from $d$ by the deletion of several (possibly, zero or all) elements.</p><p>A sequence $c$ is lexicographically smaller than a sequence $d$ if and only if one of the following holds:</p><ul><li> $c$ is a prefix of $d$, but $c \ne d$;</li><li> in the first position where $c$ and $d$ differ, the sequence $c$ has a smaller element than the corresponding element in $d$.</li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 5 \cdot 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 3 \cdot 10^5$) ！ the length of $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) ！ the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the answer in the following format:</p><p>Output an integer $m$ in the first line ！ the length of $b$.</p><p>Then output $m$ integers $b_1, b_2, \ldots, b_m$ in the second line ！ the sequence $b$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 5 \cdot 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 3 \cdot 10^5$) ！ the length of $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) ！ the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output the answer in the following format:</p><p>Output an integer $m$ in the first line ！ the length of $b$.</p><p>Then output $m$ integers $b_1, b_2, \ldots, b_m$ in the second line ！ the sequence $b$.</p>





```input1|2,3,6,7
4
4
3 2 1 3
4
1 1 1 1
9
3 2 1 3 2 1 3 2 1
1
1
```




```input2|2,3,6,7,10,11,14,15,18,19
10
2
1 2
10
5 2 1 7 9 7 2 5 5 2
2
1 2
10
2 2 8 7 7 9 8 1 9 6
9
9 1 7 5 8 5 6 4 1
3
3 3 3
6
1 6 4 4 6 5
6
3 4 4 5 3 3
10
4 1 4 5 4 5 10 1 5 1
7
1 2 1 3 2 4 6
```




```output1
3
3 2 1
1
1
3
3 1 2
1
1
```




```output2
2
1 2
5
5 1 9 7 2
2
1 2
6
2 7 9 8 1 6
7
9 1 7 5 8 6 4
1
3
4
1 4 6 5
3
4 5 3
4
5 4 10 1
5
2 1 3 4 6
```



## Note

<p>In the first example, $S = \{[1], [2], [3], [1, 3], [2, 1], [2, 3], [3, 1], [3, 2], [2, 1, 3], [3, 2, 1]\}$. Among them, $[2, 1, 3]$ and $[3, 2, 1]$ are the longest and $[-3, 2, -1]$ is lexicographical smaller than $[-2, 1, -3]$, so $[3, 2, 1]$ is the answer.</p><p>In the second example, $S = \{[1]\}$, so $[1]$ is the answer.</p>
