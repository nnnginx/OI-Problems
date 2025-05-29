## Description

<div><p>You have an array $a$ of length $n$ consisting of <span class="tex-font-style-bf">non-zero</span> integers. Initially, you have $0$ coins, and you will do the following until $a$ is empty: </p><ul> <li> Let $m$ be the current size of $a$. Select an integer $i$ where $1 \le i \le m$, gain $|a_i|$$^{\text{∗}}$ coins, and then: <ul> <li> if $a_i &lt; 0$, then replace $a$ with $[a_1,a_2,\ldots,a_{i - 1}]$ (that is, delete the suffix beginning with $a_i$); </li><li> otherwise, replace $a$ with $[a_{i + 1},a_{i + 2},\ldots,a_m]$ (that is, delete the prefix ending with $a_i$). </li></ul> </li></ul><p>Find the maximum number of coins you can have at the end of the process.</p><div class="statement-footnote"><p>$^{\text{∗}}$Here $|a_i|$ represents the absolute value of $a_i$: it equals $a_i$ when $a_i &gt; 0$ and $-a_i$ when $a_i &lt; 0$.</p></div></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of $a$.</p><p>The second line of each testcase contains $n$ integers $a_1,a_2,\ldots,a_n$ ($-10^9 \le a_i \le 10^9$, $a_i \ne 0$).</p><p>The sum of $n$ across all testcases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum number of coins you can have at the end of the process.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of $a$.</p><p>The second line of each testcase contains $n$ integers $a_1,a_2,\ldots,a_n$ ($-10^9 \le a_i \le 10^9$, $a_i \ne 0$).</p><p>The sum of $n$ across all testcases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the maximum number of coins you can have at the end of the process.</p>





```input1|2,3,6,7
3
6
3 1 4 -1 -5 -9
6
-10 -3 -17 1 19 20
1
1
```




```output1
23
40
1
```



## Note

<p>An example of how to get $23$ coins in the first testcase is as follows: </p><ul> <li> $a = [3, 1, 4, -1, -5, \color{red}{-9}] \xrightarrow{i = 6} a = [3, 1, 4, -1, -5] $, and get $9$ coins. </li><li> $a = [\color{red}{3}, 1, 4, -1, -5] \xrightarrow{i = 1} a = [1, 4, -1, -5] $, and get $3$ coins. </li><li> $a = [\color{red}{1}, 4, -1, -5] \xrightarrow{i = 1} a = [4, -1, -5] $, and get $1$ coin. </li><li> $a = [4, -1, \color{red}{-5}] \xrightarrow{i = 3} a = [4, -1] $, and get $5$ coins. </li><li> $a = [4, \color{red}{-1}] \xrightarrow{i = 2} a = [4] $, and get $1$ coin. </li><li> $a = [\color{red}{4}] \xrightarrow{i = 1} a = [] $, and get $4$ coins. </li></ul> After all the operations, you have $23$ coins.<p>An example of how to get $40$ coins in the second testcase is as follows: </p><ul> <li> $a = [-10, -3, -17, \color{red}{1}, 19, 20] \xrightarrow{i = 4} a = [19, 20] $, and get $1$ coin. </li><li> $a = [\color{red}{19}, 20] \xrightarrow{i = 1} a = [20] $, and get $19$ coins. </li><li> $a = [\color{red}{20}] \xrightarrow{i = 1} a = [] $, and get $20$ coins. </li></ul> After all the operations, you have $40$ coins.
