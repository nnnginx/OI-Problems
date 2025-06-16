## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><a href="https://soundcloud.com/patrick-deng-392681004/trade-winds-ft-alex-zhu">Trade Winds - Patrick Deng</a></span></div><div class="epigraph-source">⠀</div></div><p>Let's call an array $a$ <span class="tex-font-style-it">sorted</span> if $a_1 \leq a_2 \leq \ldots \leq a_{n - 1} \leq a_{n}$.</p><p>You are given two of Farmer John's favorite integers, $n$ and $k$. He challenges you to find any array $a_1, a_2, \ldots, a_{n}$ satisfying the following requirements:</p><ul> <li> $1 \leq a_i \leq 10^9$ for each $1 \leq i \leq n$; </li><li> Out of the $n$ total cyclic shifts of $a$, exactly $k$ of them are sorted.$^\dagger$ </li></ul><p>If there is no such array $a$, output $-1$.</p><p>$^\dagger$The $x$-th ($1 \leq x \leq n$) <span class="tex-font-style-bf">cyclic shift</span> of the array $a$ is $a_x, a_{x+1} \ldots a_n, a_1, a_2 \ldots a_{x - 1}$. If $c_{x, i}$ denotes the $i$'th element of the $x$'th cyclic shift of $a$, exactly $k$ such $x$ should satisfy $c_{x,1} \leq c_{x,2} \leq \ldots \leq c_{x, n - 1} \leq c_{x, n}$.</p><p>For example, the cyclic shifts for $a = [1, 2, 3, 3]$ are the following:</p><ul> <li> $x = 1$: $[1, 2, 3, 3]$ (sorted); </li><li> $x = 2$: $[2, 3, 3, 1]$ (not sorted); </li><li> $x = 3$: $[3, 3, 1, 2]$ (not sorted); </li><li> $x = 4$: $[3, 1, 2, 3]$ (not sorted). </li></ul></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases.</p><p>Each test case contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 10^3$)&nbsp;— the length of $a$ and the number of sorted cyclic shifts $a$ must have.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^3$.</p></div><div class="output-specification"><p>For each test case, print a single line: </p><ul> <li> if there is a valid array $a$, output $n$ integers, representing $a_1, a_2, \ldots, a_{n}$; </li><li> otherwise, output $-1$. </li></ul><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases.</p><p>Each test case contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 10^3$)&nbsp;— the length of $a$ and the number of sorted cyclic shifts $a$ must have.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^3$.</p>

## Output

<p>For each test case, print a single line: </p><ul> <li> if there is a valid array $a$, output $n$ integers, representing $a_1, a_2, \ldots, a_{n}$; </li><li> otherwise, output $-1$. </li></ul><p>If there are multiple solutions, print any of them.</p>





```input1|2,4
3
2 2
3 1
3 2
```




```output1
1 1
69420 69 420
-1
```



## Note

<p>In the first testcase, $a = [1, 1]$ satisfies $n = 2, k = 2$:</p><p>The two cyclic shifts of $a$ are $[a_1, a_2]$ and $[a_2, a_1]$, which are both $[1, 1]$ and are sorted.</p><p>In the second testcase, $a = [69\,420, 69, 420]$ satisfies $n = 3, k = 1$:</p><p>The three cyclic shifts of $a$ are $[a_1, a_2, a_3]$, $[a_2, a_3, a_1]$, $[a_3, a_1, a_2]$, which are $[69\,420, 69, 420]$, $[69, 420, 69\,420]$, and $[420, 69\,420, 69]$, respectively. </p><p>Only $[69, 420, 69\,420]$ is sorted.</p>
