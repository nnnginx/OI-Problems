## Description

<div><p>You are given a string $s$ consisting of lowercase Latin characters. Count the number of nonempty strings $t \neq$ "$\texttt{a}$" such that it is possible to partition$^{\dagger}$ $s$ into some substrings satisfying the following conditions: </p><ul> <li> each substring either equals $t$ or "$\texttt{a}$", and </li><li> at least one substring equals $t$. </li></ul> <p>$^{\dagger}$ A <span class="tex-font-style-it">partition</span> of a string $s$ is an ordered sequence of some $k$ strings $t_1, t_2, \ldots, t_k$ (called <span class="tex-font-style-it">substrings</span>) such that $t_1 + t_2 + \ldots + t_k = s$, where $+$ represents the concatenation operation.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a string $s$ consisting of lowercase Latin characters ($2 \leq |s| \leq 2 \cdot 10^5$).</p><p>The sum of $|s|$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of nonempty strings $t \neq$ "$\texttt{a}$" that satisfy all constraints.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a string $s$ consisting of lowercase Latin characters ($2 \leq |s| \leq 2 \cdot 10^5$).</p><p>The sum of $|s|$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of nonempty strings $t \neq$ "$\texttt{a}$" that satisfy all constraints.</p>





```input1|2,4,6,8
8
aaaaa
baba
cabacb
aaabaaa
bitset
ab
abbaaaabbb
yearnineteeneightyfour
```




```output1
4
4
1
16
1
2
3
1
```



## Note

<p>In the first test case, $t$ can be "$\texttt{aa}$", "$\texttt{aaa}$", "$\texttt{aaaa}$", or the full string.</p><p>In the second test case, $t$ can be "$\texttt{b}$", "$\texttt{bab}$", "$\texttt{ba}$", or the full string.</p><p>In the third test case, the only such $t$ is the full string.</p>
