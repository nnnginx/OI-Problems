## Description

<div><p>Ashish has two strings $a$ and $b$, each of length $n$, and an integer $k$. The strings only contain lowercase English letters.</p><p>He wants to convert string $a$ into string $b$ by performing some (possibly zero) operations on $a$.</p><p>In one move, he can either </p><ul> <li> choose an index $i$ ($1 \leq i\leq n-1$) and swap $a_i$ and $a_{i+1}$, or </li><li> choose an index $i$ ($1 \leq i \leq n-k+1$) and if $a_i, a_{i+1}, \ldots, a_{i+k-1}$ are <span class="tex-font-style-bf">all equal</span> to some character $c$ ($c \neq$ '<span class="tex-font-style-tt">z</span>'), replace each one with the next character $(c+1)$, that is, '<span class="tex-font-style-tt">a</span>' is replaced by '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">b</span>' is replaced by '<span class="tex-font-style-tt">c</span>' and so on. </li></ul><p>Note that he can perform any number of operations, and the operations can only be performed on string $a$. </p><p>Help Ashish determine if it is possible to convert string $a$ into $b$ after performing some (possibly zero) operations on it.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;�� the number of test cases. The description of each test case is as follows.</p><p>The first line of each test case contains two integers $n$ ($2 \leq n \leq 10^6$) and $k$ ($1 \leq k \leq n$).</p><p>The second line of each test case contains the string $a$ of length $n$ consisting of lowercase English letters.</p><p>The third line of each test case contains the string $b$ of length $n$ consisting of lowercase English letters.</p><p>It is guaranteed that the sum of values $n$ among all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" if Ashish can convert $a$ into $b$ after some moves, else print "<span class="tex-font-style-tt">No</span>".</p><p>You may print the letters of the answer in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;�� the number of test cases. The description of each test case is as follows.</p><p>The first line of each test case contains two integers $n$ ($2 \leq n \leq 10^6$) and $k$ ($1 \leq k \leq n$).</p><p>The second line of each test case contains the string $a$ of length $n$ consisting of lowercase English letters.</p><p>The third line of each test case contains the string $b$ of length $n$ consisting of lowercase English letters.</p><p>It is guaranteed that the sum of values $n$ among all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" if Ashish can convert $a$ into $b$ after some moves, else print "<span class="tex-font-style-tt">No</span>".</p><p>You may print the letters of the answer in any case (upper or lower).</p>

## Samples

```input1
4
3 3
abc
bcd
4 2
abba
azza
2 1
zz
aa
6 2
aaabba
ddddcc
```

```output1
No
Yes
No
Yes
```




## Note

<p>In the first test case it can be shown that it is impossible to convert $a$ into $b$.</p><p>In the second test case,</p><p>"<span class="tex-font-style-tt">a<span class="tex-font-style-bf">bb</span>a</span>" $\xrightarrow{\text{inc}}$ "<span class="tex-font-style-tt">a<span class="tex-font-style-bf">cc</span>a</span>" $\xrightarrow{\text{inc}}$ $\ldots$ $\xrightarrow{\text{inc}}$ "<span class="tex-font-style-tt">azza</span>".</p><p>Here "swap" denotes an operation of the first type, and "inc" denotes an operation of the second type.</p><p>In the fourth test case,</p><p>"<span class="tex-font-style-tt">aaab<span class="tex-font-style-bf">ba</span></span>" $\xrightarrow{\text{swap}}$ "<span class="tex-font-style-tt">aaa<span class="tex-font-style-bf">ba</span>b</span>" $\xrightarrow{\text{swap}}$ "<span class="tex-font-style-tt"><span class="tex-font-style-bf">aa</span>aabb</span>" $\xrightarrow{\text{inc}}$ $\ldots$ $\xrightarrow{\text{inc}}$ "<span class="tex-font-style-tt">dd<span class="tex-font-style-bf">aa</span>bb</span>" $\xrightarrow{\text{inc}}$ $\ldots$ $\xrightarrow{\text{inc}}$ "<span class="tex-font-style-tt">dddd<span class="tex-font-style-bf">bb</span></span>" $\xrightarrow{\text{inc}}$ $\ldots$ $\xrightarrow{\text{inc}}$ "<span class="tex-font-style-tt">ddddcc</span>".</p>
