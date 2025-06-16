## Description

<div><p>Vlad is planning to hold $m$ rounds next month. Each round should contain one problem of difficulty levels '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">C</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">E</span>', '<span class="tex-font-style-tt">F</span>', and '<span class="tex-font-style-tt">G</span>'.</p><p>Vlad already has a bank of $n$ problems, where the $i$-th problem has a difficulty level of $a_i$. There may not be enough of these problems, so he may have to come up with a few more problems.</p><p>Vlad wants to come up with as few problems as possible, so he asks you to find the minimum number of problems he needs to come up with in order to hold $m$ rounds.</p><p>For example, if $m=1$, $n = 10$, $a=$ '<span class="tex-font-style-tt">BGECDCBDED</span>', then he needs to come up with two problems: one of difficulty level '<span class="tex-font-style-tt">A</span>' and one of difficulty level '<span class="tex-font-style-tt">F</span>'.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 50$, $1 \le m \le 5$)&nbsp;！ the number of problems in the bank and the number of upcoming rounds, respectively.</p><p>The second line of each test case contains a string $a$ of $n$ characters from '<span class="tex-font-style-tt">A</span>' to '<span class="tex-font-style-tt">G</span>'&nbsp;！ the difficulties of the problems in the bank.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of problems that need to come up with to hold $m$ rounds.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 50$, $1 \le m \le 5$)&nbsp;！ the number of problems in the bank and the number of upcoming rounds, respectively.</p><p>The second line of each test case contains a string $a$ of $n$ characters from '<span class="tex-font-style-tt">A</span>' to '<span class="tex-font-style-tt">G</span>'&nbsp;！ the difficulties of the problems in the bank.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of problems that need to come up with to hold $m$ rounds.</p>





```input1|2,3,6,7
3
10 1
BGECDCBDED
10 2
BGECDCBDED
9 1
BBCDEFFGG
```




```output1
2
5
1
```


