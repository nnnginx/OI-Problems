## Description

<div><p>There is a binary string $a$ of length $n$. In one operation, you can select any prefix of $a$ with an <span class="tex-font-style-bf">equal</span> number of $0$ and $1$ symbols. Then all symbols in the prefix are inverted: each $0$ becomes $1$ and each $1$ becomes $0$.</p><p>For example, suppose $a=0111010000$. </p><ul> <li> In the first operation, we can select the prefix of length $8$ since it has four $0$'s and four $1$'s: $[01110100]00\to [10001011]00$. </li><li> In the second operation, we can select the prefix of length $2$ since it has one $0$ and one $1$: $[10]00101100\to [01]00101100$. </li><li> It is illegal to select the prefix of length $4$ for the third operation, because it has three $0$'s and one $1$. </li></ul><p>Can you transform the string $a$ into the string $b$ using some finite number of operations (possibly, none)?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 10^4$) �� the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 3\cdot 10^5$) �� the length of the strings $a$ and $b$.</p><p>The following two lines contain strings $a$ and $b$ of length $n$, consisting of symbols $0$ and $1$.</p><p>The sum of $n$ across all test cases does not exceed $3\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if it is possible to transform $a$ into $b$, or "<span class="tex-font-style-tt">NO</span>" if it is impossible. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 10^4$) �� the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 3\cdot 10^5$) �� the length of the strings $a$ and $b$.</p><p>The following two lines contain strings $a$ and $b$ of length $n$, consisting of symbols $0$ and $1$.</p><p>The sum of $n$ across all test cases does not exceed $3\cdot 10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if it is possible to transform $a$ into $b$, or "<span class="tex-font-style-tt">NO</span>" if it is impossible. You can print each letter in any case (upper or lower).</p>

## Samples

```input1
5
10
0111010000
0100101100
4
0000
0000
3
001
000
12
010101010101
100110011010
6
000111
110100
```

```output1
YES
YES
NO
YES
NO
```




## Note

<p>The first test case is shown in the statement.</p><p>In the second test case, we transform $a$ into $b$ by using zero operations.</p><p>In the third test case, there is no legal operation, so it is impossible to transform $a$ into $b$.</p><p>In the fourth test case, here is one such transformation: </p><ul> <li> Select the length $2$ prefix to get $100101010101$. </li><li> Select the length $12$ prefix to get $011010101010$. </li><li> Select the length $8$ prefix to get $100101011010$. </li><li> Select the length $4$ prefix to get $011001011010$. </li><li> Select the length $6$ prefix to get $100110011010$. </li></ul><p>In the fifth test case, the only legal operation is to transform $a$ into $111000$. From there, the only legal operation is to return to the string we started with, so we cannot transform $a$ into $b$.</p>
