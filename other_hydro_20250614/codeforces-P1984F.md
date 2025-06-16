## Description

<div><p>There is a hidden array $a_1, a_2, \ldots, a_n$ of length $n$ whose elements are integers between $-m$ and $m$, inclusive.</p><p>You are given an array $b_1, b_2, \ldots, b_n$ of length $n$ and a string $s$ of length $n$ consisting of the characters $\texttt{P}$, $\texttt{S}$, and $\texttt{?}$.</p><p>For each $i$ from $1$ to $n$ inclusive, we must have: </p><ul> <li> If $s_i = \texttt{P}$, $b_i$ is the sum of $a_1$ through $a_i$. </li><li> If $s_i = \texttt{S}$, $b_i$ is the sum of $a_i$ through $a_n$. </li></ul><p>Output the number of ways to replace all $\texttt{?}$ in $s$ with either $\texttt{P}$ or $\texttt{S}$ such that there exists an array $a_1, a_2, \ldots, a_n$ with elements not exceeding $m$ by absolute value satisfying the constraints given by the array $b_1, b_2, \ldots, b_n$ and the string $s$.</p><p>Since the answer may be large, output it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 2 \cdot 10^3$, $2 \leq m \leq 10^{9}$)&nbsp;！ the length of the hidden array $a_1, a_2, \ldots, a_n$ and the maximum absolute value of an element $a_i$.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of characters $\texttt{P}$, $\texttt{S}$, and $\texttt{?}$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($|b_i| \leq m \cdot n$).</p><p>The sum of $n$ over all test cases does not exceed $5 \cdot 10^3$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of ways to replace all $\texttt{?}$ in $s$ with either $\texttt{P}$ or $\texttt{S}$ that result in the existence of a valid array $a_1, a_2, \ldots, a_n$, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^3$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 2 \cdot 10^3$, $2 \leq m \leq 10^{9}$)&nbsp;！ the length of the hidden array $a_1, a_2, \ldots, a_n$ and the maximum absolute value of an element $a_i$.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of characters $\texttt{P}$, $\texttt{S}$, and $\texttt{?}$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($|b_i| \leq m \cdot n$).</p><p>The sum of $n$ over all test cases does not exceed $5 \cdot 10^3$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of ways to replace all $\texttt{?}$ in $s$ with either $\texttt{P}$ or $\texttt{S}$ that result in the existence of a valid array $a_1, a_2, \ldots, a_n$, modulo $998\,244\,353$.</p>





```input1|2,3,4,8,9,10,14,15,16
6
4 10
PSPP
1 9 8 10
4 1000000000
????
1 1 1 4000000000
8 1000000000
?P?SSP?P
-857095623 -1424391899 -851974476 673437144 471253851 -543483033 364945701 -178537332
4 7
PPSS
4 2 1 3
9 20
?????????
1 2 3 4 5 6 7 8 9
3 1000000000
P??
-145463248 -974068460 -1287458396
```




```output1
1
0
2
1
14
1
```



## Note

<p>In the first test case, we can see that the following array satisfies all constraints, thus the answer is $1$: </p><ol> <li> $\texttt{P}$&nbsp;！ ${[\color{red}{\textbf{1}},3,4,2]}$: sum of $1$. </li><li> $\texttt{S}$&nbsp;！ ${[1,\color{red}{\textbf{3},4,2}]}$: sum of $9$. </li><li> $\texttt{P}$&nbsp;！ ${[\color{red}{1,3,\textbf{4}},2]}$: sum of $8$. </li><li> $\texttt{P}$&nbsp;！ ${[\color{red}{1,3,4,\textbf{2}}]}$: sum of $10$. </li></ol><p>In the second test case, it can be shown that no array $a$ with all $|a_i| \leq m = 10^9$ satisfies all constraints.</p>
