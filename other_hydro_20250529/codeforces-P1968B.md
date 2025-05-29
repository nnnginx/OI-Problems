## Description

<div><p>You are given two binary strings $a$ and $b$. A binary string is a string consisting of the characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p><p>Your task is to determine the maximum possible number $k$ such that a prefix of string $a$ of length $k$ is a subsequence of string $b$.</p><p>A sequence $a$ is a subsequence of a sequence $b$ if $a$ can be obtained from $b$ by the deletion of several (possibly, zero or all) elements.</p></div><div class="input-specification"><p>The first line consists of a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1\le n,m \le 2 \cdot 10^5$)&nbsp;！ the length of string $a$ and the length of string $b$, respectively.</p><p>The second line of each test case contains a binary string $a$ of length $n$.</p><p>The third line of each test case contains a binary string $b$ of length $m$.</p><p>It is guaranteed that the sum of values $n$ over all test cases does not exceed $2 \cdot 10^5$. Similarly, the sum of values $m$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single number ！ the maximum $k$, such that the first $k$ characters of $a$ form a subsequence of $b$.</p></div>

## Input

<p>The first line consists of a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1\le n,m \le 2 \cdot 10^5$)&nbsp;！ the length of string $a$ and the length of string $b$, respectively.</p><p>The second line of each test case contains a binary string $a$ of length $n$.</p><p>The third line of each test case contains a binary string $b$ of length $m$.</p><p>It is guaranteed that the sum of values $n$ over all test cases does not exceed $2 \cdot 10^5$. Similarly, the sum of values $m$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single number ！ the maximum $k$, such that the first $k$ characters of $a$ form a subsequence of $b$.</p>





```input1|2,3,4,8,9,10,14,15,16
6
5 4
10011
1110
3 3
100
110
1 3
1
111
4 4
1011
1111
3 5
100
11010
3 1
100
0
```




```output1
2
2
1
1
3
0
```



## Note

<p>In the first example, the string '$10$' is a subsequence of '$1\color{red}11\color{red}0$' but the string '$100$' is not. So the answer is $2$.</p><p>In the fifth example, $a$='$100$', $b$='$1\color{red}{10}1\color{red}0$', whole string $a$ is a subsequence of string $b$. So the answer is $3$.</p><p>In the sixth example, string $b$ does not contain '$1$' so the answer is $0$.</p>
