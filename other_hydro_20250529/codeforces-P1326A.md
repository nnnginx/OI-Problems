## Description

<div><p>You are given a integer $n$ ($n &gt; 0$). Find <span class="tex-font-style-bf">any</span> integer $s$ which satisfies these conditions, or report that there are no such numbers:</p><p>In the decimal representation of $s$: </p><ul> <li> $s &gt; 0$, </li><li> $s$ consists of $n$ digits, </li><li> no digit in $s$ equals $0$, </li><li> $s$ is not divisible by any of it's digits. </li></ul></div><div class="input-specification"><p>The input consists of multiple test cases. The first line of the input contains a single integer $t$ ($1 \leq t \leq 400$), the number of test cases. The next $t$ lines each describe a test case.</p><p>Each test case contains one positive integer $n$ ($1 \leq n \leq 10^5$).</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print an integer $s$ which satisfies the conditions described above, or "<span class="tex-font-style-tt">-1</span>" (without quotes), if no such number exists. If there are multiple possible solutions for $s$, print <span class="tex-font-style-bf">any</span> solution.</p></div>

## Input

<p>The input consists of multiple test cases. The first line of the input contains a single integer $t$ ($1 \leq t \leq 400$), the number of test cases. The next $t$ lines each describe a test case.</p><p>Each test case contains one positive integer $n$ ($1 \leq n \leq 10^5$).</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print an integer $s$ which satisfies the conditions described above, or "<span class="tex-font-style-tt">-1</span>" (without quotes), if no such number exists. If there are multiple possible solutions for $s$, print <span class="tex-font-style-bf">any</span> solution.</p>

## Samples

```input1
4
1
2
3
4
```

```output1
-1
57
239
6789
```




## Note

<p>In the first test case, there are no possible solutions for $s$ consisting of one digit, because any such solution is divisible by itself.</p><p>For the second test case, the possible solutions are: $23$, $27$, $29$, $34$, $37$, $38$, $43$, $46$, $47$, $49$, $53$, $54$, $56$, $57$, $58$, $59$, $67$, $68$, $69$, $73$, $74$, $76$, $78$, $79$, $83$, $86$, $87$, $89$, $94$, $97$, and $98$.</p><p>For the third test case, one possible solution is $239$ because $239$ is not divisible by $2$, $3$ or $9$ and has three digits (none of which equals zero).</p>
