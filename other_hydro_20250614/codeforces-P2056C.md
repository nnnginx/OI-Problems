## Description

<div><p> </p><p>For an integer sequence $a = [a_1, a_2, \ldots, a_n]$, we define $f(a)$ as the length of the longest subsequence$^{\text{∗}}$ of $a$ that is a palindrome$^{\text{†}}$. </p><p>Let $g(a)$ represent the number of subsequences of length $f(a)$ that are palindromes. In other words, $g(a)$ counts the number of palindromic subsequences in $a$ that have the maximum length.</p><p>Given an integer $n$, your task is to find any sequence $a$ of $n$ integers that satisfies the following conditions:</p><ul> <li> $1 \le a_i \le n$ for all $1 \le i \le n$. </li><li> $g(a) &gt; n$ </li></ul><p>It can be proven that such a sequence always exists under the given constraints.</p><div class="statement-footnote"><p>$^{\text{∗}}$A sequence $x$ is a subsequence of a sequence $y$ if $x$ can be obtained from $y$ by the deletion of several (possibly, zero or all) element from arbitrary positions. </p><p>$^{\text{†}}$A palindrome is a sequence that reads the same from left to right as from right to left. For example, $[1, 2, 1, 3, 1, 2, 1]$, $[5, 5, 5, 5]$, and $[4, 3, 3, 4]$ are palindromes, while $[1, 2]$ and $[2, 3, 3, 3, 3]$ are not.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($\color{red}{6} \le n \le 100$)&nbsp;— the length of the sequence.</p><p>Note that there are <span class="tex-font-style-bf">no</span> constraints on the sum of $n$ over all test cases.</p></div><div class="output-specification"><p>For each test case, output $n$ integers $a_1, a_2, \ldots, a_n$, representing an array that satisfies the conditions.</p><p>If there are multiple solutions, you may output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($\color{red}{6} \le n \le 100$)&nbsp;— the length of the sequence.</p><p>Note that there are <span class="tex-font-style-bf">no</span> constraints on the sum of $n$ over all test cases.</p>

## Output

<p>For each test case, output $n$ integers $a_1, a_2, \ldots, a_n$, representing an array that satisfies the conditions.</p><p>If there are multiple solutions, you may output any of them.</p>





```input1|2,4
3
6
9
15
```




```output1
1 1 2 3 1 2
7 3 3 7 5 3 7 7 3
15 8 8 8 15 5 8 1 15 5 8 15 15 15 8
```



## Note

<p>In the first example, one possible solution is $a = [1, 1, 2, 3, 1, 2]$. In this case, $f(a) = 3$ as the longest palindromic subsequence has length $3$. There are $7$ ways to choose a subsequence of length $3$ that is a palindrome, as shown below:</p><ol> <li> $[a_1, a_2, a_5] = [1, 1, 1]$ </li><li> $[a_1, a_3, a_5] = [1, 2, 1]$ </li><li> $[a_1, a_4, a_5] = [1, 3, 1]$ </li><li> $[a_2, a_3, a_5] = [1, 2, 1]$ </li><li> $[a_2, a_4, a_5] = [1, 3, 1]$ </li><li> $[a_3, a_4, a_6] = [2, 3, 2]$ </li><li> $[a_3, a_5, a_6] = [2, 1, 2]$ </li></ol><p>Therefore, $g(a) = 7$, which is greater than $n = 6$. Hence, $a = [1, 1, 2, 3, 1, 2]$ is a valid solution.</p><p>In the second example, one possible solution is $a = [7, 3, 3, 7, 5, 3, 7, 7, 3]$. In this case, $f(a) = 5$. There are $24$ ways to choose a subsequence of length $5$ that is a palindrome. Some examples are $[a_2, a_4, a_5, a_8, a_9] = [3, 7, 5, 7, 3]$ and $[a_1, a_4, a_6, a_7, a_8] = [7, 7, 3, 7, 7]$. Therefore, $g(a) = 24$, which is greater than $n = 9$. Hence, $a = [7, 3, 3, 7, 5, 3, 7, 7, 3]$ is a valid solution.</p><p>In the third example, $f(a) = 7$ and $g(a) = 190$, which is greater than $n = 15$.</p>
