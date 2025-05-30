## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The differences between the two versions are the constraints on $n, m, b_0$ and the time limit. You can make hacks only if both versions are solved.</span></p><p>Little R has counted many sets before, and now she decides to count arrays.</p><p>Little R thinks an array $b_0, \ldots, b_n$ consisting of non-negative integers is <span class="tex-font-style-it">continuous</span> if and only if, for each $i$ such that $1 \leq i \leq n$, $\lvert b_i - b_{i-1} \rvert = 1$ is satisfied. She likes continuity, so she only wants to generate continuous arrays.</p><p>If Little R is given $b_0$ and $a_1, \ldots, a_n$, she will try to generate a non-negative continuous array $b$, which has no similarity with $a$. More formally, for all $1 \leq i \leq n$, $a_i \neq b_i$ holds.</p><p>However, Little R does not have any array $a$. Instead, she gives you $n$, $m$ and $b_0$. She wants to count the different integer arrays $a_1, \ldots, a_n$ satisfying:</p><ul> <li> $1 \leq a_i \leq m$; </li><li> At least one non-negative continuous array $b_0, \ldots, b_n$ can be generated. </li></ul><p><span class="tex-font-style-bf">Note that $b_i \geq 0$, but the $b_i$ can be arbitrarily large.</span></p><p>Since the actual answer may be enormous, please just tell her the answer modulo $998\,244\,353$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t\ (1 \leq t \leq 10^4)$. The description of the test cases follows.</p><p>The first and only line of each test case contains three integers $n$, $m$, and $b_0$ ($1 \leq n \leq 2 \cdot 10^6$, $1 \leq m \leq 2 \cdot 10^6$, $0 \leq b_0 \leq 2\cdot 10^6$)&nbsp;�� the length of the array $a_1, \ldots, a_n$, the maximum possible element in $a_1, \ldots, a_n$, and the initial element of the array $b_0, \ldots, b_n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceeds $10^7$.</p></div><div class="output-specification"><p>For each test case, output a single line containing an integer: the number of different arrays $a_1, \ldots, a_n$ satisfying the conditions, modulo $998\,244\,353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t\ (1 \leq t \leq 10^4)$. The description of the test cases follows.</p><p>The first and only line of each test case contains three integers $n$, $m$, and $b_0$ ($1 \leq n \leq 2 \cdot 10^6$, $1 \leq m \leq 2 \cdot 10^6$, $0 \leq b_0 \leq 2\cdot 10^6$)&nbsp;�� the length of the array $a_1, \ldots, a_n$, the maximum possible element in $a_1, \ldots, a_n$, and the initial element of the array $b_0, \ldots, b_n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceeds $10^7$.</p>

## Output

<p>For each test case, output a single line containing an integer: the number of different arrays $a_1, \ldots, a_n$ satisfying the conditions, modulo $998\,244\,353$.</p>





```input1|2,4,6
6
3 2 1
5 5 3
13 4 1
100 6 7
100 11 3
1000 424 132
```




```output1
6
3120
59982228
943484039
644081522
501350342
```



## Note

<p>In the first test case, for example, when $a = [1, 2, 1]$, we can set $b = [1, 0, 1, 0]$. When $a = [1, 1, 2]$, we can set $b = [1, 2, 3, 4]$. In total, there are $6$ valid choices of $a_1, \ldots, a_n$: in fact, it can be proved that only $a = [2, 1, 1]$ and $a = [2, 1, 2]$ make it impossible to construct a non-negative continuous $b_0, \ldots, b_n$, so the answer is $2^3 - 2 = 6$.</p>
