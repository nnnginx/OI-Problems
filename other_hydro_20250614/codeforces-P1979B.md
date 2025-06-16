## Description

<div><p>You are given two distinct non-negative integers $x$ and $y$. Consider two infinite sequences $a_1, a_2, a_3, \ldots$ and $b_1, b_2, b_3, \ldots$, where</p><ul> <li> $a_n = n \oplus x$; </li><li> $b_n = n \oplus y$. </li></ul><p>Here, $x \oplus y$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> operation of integers $x$ and $y$.</p><p>For example, with $x = 6$, the first $8$ elements of sequence $a$ will look as follows: $[7, 4, 5, 2, 3, 0, 1, 14, \ldots]$. Note that the indices of elements start with $1$.</p><p>Your task is to find the length of the longest common subsegment$^\dagger$ of sequences $a$ and $b$. In other words, find the maximum integer $m$ such that $a_i = b_j, a_{i + 1} = b_{j + 1}, \ldots, a_{i + m - 1} = b_{j + m - 1}$ for some $i, j \ge 1$.</p><p>$^\dagger$A subsegment of sequence $p$ is a sequence $p_l,p_{l+1},\ldots,p_r$, where $1 \le l \le r$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $x$ and $y$ ($0 \le x, y \le 10^9, x \neq y$)&nbsp;！ the parameters of the sequences.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the length of the longest common subsegment.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $x$ and $y$ ($0 \le x, y \le 10^9, x \neq y$)&nbsp;！ the parameters of the sequences.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the length of the longest common subsegment.</p>





```input1|2,4
4
0 1
12 4
57 37
316560849 14570961
```




```output1
1
8
4
33554432
```



## Note

<p>In the first test case, the first $7$ elements of sequences $a$ and $b$ are as follows:</p><p>$a = [1, 2, 3, 4, 5, 6, 7,\ldots]$</p><p>$b = [0, 3, 2, 5, 4, 7, 6,\ldots]$</p><p>It can be shown that there isn't a positive integer $k$ such that the sequence $[k, k + 1]$ occurs in $b$ as a subsegment. So the answer is $1$.</p><p>In the third test case, the first $20$ elements of sequences $a$ and $b$ are as follows:</p><p>$a = [56, 59, 58, 61, 60, 63, 62, 49, 48, 51, 50, 53, 52, 55, 54, \textbf{41, 40, 43, 42}, 45, \ldots]$</p><p>$b = [36, 39, 38, 33, 32, 35, 34, 45, 44, 47, 46, \textbf{41, 40, 43, 42}, 53, 52, 55, 54, 49, \ldots]$</p><p>It can be shown that one of the longest common subsegments is the subsegment $[41, 40, 43, 42]$ with a length of $4$.</p>
