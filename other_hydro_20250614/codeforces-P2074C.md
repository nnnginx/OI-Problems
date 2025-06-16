## Description

<div><p>This time, the pink soldiers have given you an integer $x$ ($x \ge 2$).</p><p>Please determine if there exists a <span class="tex-font-style-bf">positive</span> integer $y$ that satisfies the following conditions.</p><ul> <li> $y$ is <span class="tex-font-style-bf">strictly</span> less than $x$. </li><li> There exists a <span class="tex-font-style-bf">non-degenerate triangle</span>$^{\text{∗}}$ with side lengths $x$, $y$, $x \oplus y$. Here, $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. </li></ul><p>Additionally, if there exists such an integer $y$, output any.</p><div class="statement-footnote"><p>$^{\text{∗}}$A triangle with side lengths $a$, $b$, $c$ is non-degenerate when $a+b &gt; c$, $a+c &gt; b$, $b+c &gt; a$.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2000$). The description of the test cases follows. </p><p>The only line of each test case contains a single integer $x$ ($2 \le x \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print one integer on a separate line. The integer you must output is as follows:</p><ul> <li> If there exists an integer $y$ satisfying the conditions, output the value of $y$ ($1 \le y &lt; x$); </li><li> Otherwise, output $-1$. </li></ul><p>If there exist multiple integers that satisfy the conditions, you may output any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2000$). The description of the test cases follows. </p><p>The only line of each test case contains a single integer $x$ ($2 \le x \le 10^9$).</p>

## Output

<p>For each test case, print one integer on a separate line. The integer you must output is as follows:</p><ul> <li> If there exists an integer $y$ satisfying the conditions, output the value of $y$ ($1 \le y &lt; x$); </li><li> Otherwise, output $-1$. </li></ul><p>If there exist multiple integers that satisfy the conditions, you may output any.</p>





```input1|2,4,6,8
7
5
2
6
3
69
4
420
```




```output1
3
-1
5
-1
66
-1
320
```



## Note

<p>In the first test case, there exists a non-degenerate triangle with side lengths $3$, $5$, and $3 \oplus 5 = 6$. Therefore, $y=3$ is a valid answer.</p><p>In the second test case, $1$ is the only possible candidate for $y$, but it cannot make a non-degenerate triangle. Therefore, the answer is $-1$.</p>
