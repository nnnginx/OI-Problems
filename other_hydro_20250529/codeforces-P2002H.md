## Description

<div><p><span class="tex-font-style-it">It's been a long summer's day, with the constant chirping of cicadas and the heat which never seemed to end. Finally, it has drawn to a close. The showdown has passed, the gates are open, and only a gentle breeze is left behind.</span></p><p><span class="tex-font-style-it">Your predecessors had taken their final bow; it's your turn to take the stage.</span></p><p>Sorting through some notes that were left behind, you found a curious statement named <span class="tex-font-style-bf">Problem 101</span>:</p><ul> <li> Given a positive integer sequence $a_1,a_2,\ldots,a_n$, you can operate on it any number of times. In an operation, you choose three consecutive elements $a_i,a_{i+1},a_{i+2}$, and merge them into one element $\max(a_i+1,a_{i+1},a_{i+2}+1)$. Please calculate the maximum number of operations you can do without creating an element greater than $m$. </li></ul><p>After some thought, you decided to propose the following problem, named <span class="tex-font-style-bf">Counting 101</span>:</p><ul> <li> Given $n$ and $m$. For each $k=0,1,\ldots,\left\lfloor\frac{n-1}{2}\right\rfloor$, please find the number of integer sequences $a_1,a_2,\ldots,a_n$ with elements in $[1, m]$, such that when used as input for <span class="tex-font-style-bf">Problem 101</span>, the answer is $k$. As the answer can be very large, please print it modulo $10^9+7$. </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le10^3$). The description of the test cases follows. </p><p>The only line of each test case contains two integers $n$, $m$ ($1\le n\le 130$, $1\le m\le 30$).</p></div><div class="output-specification"><p>For each test case, output $\left\lfloor\frac{n+1}{2}\right\rfloor$ numbers. The $i$-th number is the number of valid sequences such that when used as input for <span class="tex-font-style-bf">Problem 101</span>, the answer is $i-1$, modulo $10^9+7$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le10^3$). The description of the test cases follows. </p><p>The only line of each test case contains two integers $n$, $m$ ($1\le n\le 130$, $1\le m\le 30$).</p>

## Output

<p>For each test case, output $\left\lfloor\frac{n+1}{2}\right\rfloor$ numbers. The $i$-th number is the number of valid sequences such that when used as input for <span class="tex-font-style-bf">Problem 101</span>, the answer is $i-1$, modulo $10^9+7$.</p>





```input1|2
2
3 2
10 10
```




```output1
6 2 
1590121 23399118 382293180 213020758 379696760
```



## Note

<p>In the first test case, there are $2^3=8$ candidate sequences. Among them, you can operate on $[1,2,1]$ and $[1,1,1]$ once; you cannot operate on the other $6$ sequences.</p>
