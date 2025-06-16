## Description

<div><p>You are given three digits $a$, $b$, and $c$. Determine whether they form a stair, a peak, or neither. </p><ul> <li> A <span class="tex-font-style-it">stair</span> satisfies the condition $a&lt;b&lt;c$. </li><li> A <span class="tex-font-style-it">peak</span> satisfies the condition $a&lt;b&gt;c$. </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains three digits $a$, $b$, $c$ ($0 \leq a$, $b$, $c \leq 9$).</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">STAIR</span>" if the digits form a stair, "<span class="tex-font-style-tt">PEAK</span>" if the digits form a peak, and "<span class="tex-font-style-tt">NONE</span>" otherwise (output the strings without quotes).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains three digits $a$, $b$, $c$ ($0 \leq a$, $b$, $c \leq 9$).</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">STAIR</span>" if the digits form a stair, "<span class="tex-font-style-tt">PEAK</span>" if the digits form a peak, and "<span class="tex-font-style-tt">NONE</span>" otherwise (output the strings without quotes).</p>





```input1|2,4,6,8
7
1 2 3
3 2 1
1 5 3
3 4 1
0 0 0
4 1 7
4 5 7
```




```output1
STAIR
NONE
PEAK
PEAK
NONE
NONE
STAIR
```


