## Description

<div><p>Let's call a number a <span class="tex-font-style-it">binary decimal</span> if it is a positive integer and all digits in its decimal notation are either $0$ or $1$. For example, $1\,010\,111$ is a binary decimal, while $10\,201$ and $787\,788$ are not.</p><p>Given a number $n$, you are asked whether or not it is possible to represent $n$ as a product of some (not necessarily distinct) binary decimals.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 5 \cdot 10^4$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$).</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if $n$ can be represented as a product of binary decimals, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 5 \cdot 10^4$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$).</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if $n$ can be represented as a product of binary decimals, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,4,6,8,10,12
11
121
1
14641
12221
10110
100000
99
112
2024
12421
1001
```




```output1
YES
YES
YES
YES
YES
YES
NO
NO
NO
NO
YES
```



## Note

<p>The first five test cases can be represented as a product of binary decimals as follows: </p><ul> <li> $121 = 11 \times 11$. </li><li> $1 = 1$ is already a binary decimal. </li><li> $14\,641 = 11 \times 11 \times 11 \times 11$. </li><li> $12\,221 = 11 \times 11 \times 101$. </li><li> $10\,110 = 10\,110$ is already a binary decimal. </li></ul>
