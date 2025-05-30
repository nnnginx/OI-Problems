## Description

<div><p>You are given two strings $s$ and $t$ of equal length $n$. In one move, you can swap any two adjacent characters of the string $s$.</p><p>You need to find the minimal number of operations you need to make string $s$ lexicographically smaller than string $t$.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds: </p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul></div><div class="input-specification"><p>The first line of input contains one integer $q$ ($1 \le q \le 10\,000$): the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains the string $s$ consisting of $n$ lowercase English letters.</p><p>The third line of each test case contains the string $t$ consisting of $n$ lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print in a separate line the minimal number of operations you need to make string $s$ lexicographically smaller than string $t$, or $-1$, if it's impossible.</p></div>

## Input

<p>The first line of input contains one integer $q$ ($1 \le q \le 10\,000$): the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line of each test case contains the string $s$ consisting of $n$ lowercase English letters.</p><p>The third line of each test case contains the string $t$ consisting of $n$ lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print in a separate line the minimal number of operations you need to make string $s$ lexicographically smaller than string $t$, or $-1$, if it's impossible.</p>

## Samples

```input1
4
1
a
a
3
rll
rrr
3
caa
aca
5
ababa
aabba
```

```output1
-1
0
2
2
```



