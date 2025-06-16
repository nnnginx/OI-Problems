## Description

<div><p><span class="tex-font-style-it">One can notice the following remarkable mathematical fact: the number $2025$ can be represented as $(20+25)^2$.</span></p><p>You are given a year represented by a string $s$, consisting of exactly $4$ characters. Thus, leading zeros are allowed in the year representation. For example, "0001", "0185", "1375" are valid year representations. You need to express it in the form $(a + b)^2$, where $a$ and $b$ are <span class="tex-font-style-bf">non-negative integers</span>, or determine that it is impossible.</p><p>For example, if $s$ = "0001", you can choose $a = 0$, $b = 1$, and write the year as $(0 + 1)^2 = 1$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;¡ª the number of test cases.</p><p>The following lines describe the test cases.</p><p>The only line of each test case contains a string $s$, consisting of exactly $4$ characters. Each character is a digit from $0$ to $9$.</p></div><div class="output-specification"><p>On a separate line for each test case, output: </p><ul> <li> Two numbers $a$ and $b$ ($a, b \ge 0$) such that $(a + b)^2 = s$, if they exist. If there are multiple suitable pairs, you may output any of them. </li><li> The number $-1$ otherwise. </li></ul></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;¡ª the number of test cases.</p><p>The following lines describe the test cases.</p><p>The only line of each test case contains a string $s$, consisting of exactly $4$ characters. Each character is a digit from $0$ to $9$.</p>

## Output

<p>On a separate line for each test case, output: </p><ul> <li> Two numbers $a$ and $b$ ($a, b \ge 0$) such that $(a + b)^2 = s$, if they exist. If there are multiple suitable pairs, you may output any of them. </li><li> The number $-1$ otherwise. </li></ul>





```input1|2,4,6
5
0001
1001
1000
4900
2025
```




```output1
0 1
-1
-1
34 36
20 25
```


