## Description

<div><p>In C++, the conditional operator <span class="tex-font-style-tt">?:</span> is used as the value of <span class="tex-font-style-tt">x?y:z</span> is $y$ if $x$ is true; otherwise, the value is $z$. $x$, $y$, and $z$ may also be expressions. It is right-associated; that is, <span class="tex-font-style-tt">a?b:c?d:e</span> is equivalent to <span class="tex-font-style-tt">a?b:(c?d:e)</span>. $0$ means false and $1$ means true.</p><p>Given a binary string with length $2n+1$, you need to show whether the value of the expression can be $1$ after inserting $n$ conditional operators into the string. You can use parentheses. For example, the string <span class="tex-font-style-tt">10101</span> can be transformed into <span class="tex-font-style-tt">(1?0:1)?0:1</span>, whose value is $1$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10\,000)$, the number of test cases. The description of the test cases follows.</p><p>In the first line of each test case, there is a single integer $n$ ($1 \le n \le 1.5 \cdot 10^5)$.</p><p>In the second line of each test case, there is a binary string of length $2n + 1$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $1.5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, on the first line, output <span class="tex-font-style-tt">Yes</span> if the string can be transformed into an expression of value $1$; otherwise, output <span class="tex-font-style-tt">No</span>.</p><p>If the answer is <span class="tex-font-style-tt">Yes</span>, output the expression on the second line. You can use parentheses, but the order of the characters in the original string must remain the same. The length of your expression must be no more than $10n+1000$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10\,000)$, the number of test cases. The description of the test cases follows.</p><p>In the first line of each test case, there is a single integer $n$ ($1 \le n \le 1.5 \cdot 10^5)$.</p><p>In the second line of each test case, there is a binary string of length $2n + 1$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $1.5 \cdot 10^5$.</p>

## Output

<p>For each test case, on the first line, output <span class="tex-font-style-tt">Yes</span> if the string can be transformed into an expression of value $1$; otherwise, output <span class="tex-font-style-tt">No</span>.</p><p>If the answer is <span class="tex-font-style-tt">Yes</span>, output the expression on the second line. You can use parentheses, but the order of the characters in the original string must remain the same. The length of your expression must be no more than $10n+1000$.</p>





```input1|2,3
2
2
10101
2
00000
```




```output1
Yes
(1?0:1)?(0):1
No
```



## Note

<p>The first test case&nbsp;¡ª is the one mentioned in the problem description.</p><p>In the second test case, it is clear that regardless of how the conditional operator is used, the result will always be zero.</p>
