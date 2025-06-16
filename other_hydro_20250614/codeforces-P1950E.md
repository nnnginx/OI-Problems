## Description

<div><p>You are given a string $s$ of length $n$ consisting of lowercase Latin characters. Find the length of the shortest string $k$ such that several (possibly one) copies of $k$ can be concatenated together to form a string with the same length as $s$ and, at most, one different character.</p><p>More formally, find the length of the shortest string $k$ such that $c = \underbrace{k + \cdots + k}_{x\rm\ \text{times}}$ for some <span class="tex-font-style-it">positive integer</span> $x$, strings $s$ and $c$ has the same length and $c_i \neq s_i$ for at most one $i$ (i.e. there exist $0$ or $1$ such positions).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;！ the length of string $s$.</p><p>The second line of each test case contains the string $s$, consisting of lowercase Latin characters.</p><p>The sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, print the length of the shortest string $k$ satisfying the constraints in the statement.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;！ the length of string $s$.</p><p>The second line of each test case contains the string $s$, consisting of lowercase Latin characters.</p><p>The sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, print the length of the shortest string $k$ satisfying the constraints in the statement.</p>





```input1|2,3,6,7,10,11
5
4
abaa
4
abba
13
slavicgslavic
8
hshahaha
20
stormflamestornflame
```




```output1
1
4
13
2
10
```



## Note

<p>In the first test case, you can select $k = \texttt{a}$ and $k+k+k+k = \texttt{aaaa}$, which only differs from $s$ in the second position.</p><p>In the second test case, you cannot select $k$ of length one or two. We can have $k = \texttt{abba}$, which is equal to $s$.</p>
