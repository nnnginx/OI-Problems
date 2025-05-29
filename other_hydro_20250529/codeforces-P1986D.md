## Description

<div><p>You are given a string $s$ of length $n &gt; 1$, consisting of digits from $0$ to $9$. You must insert exactly $n - 2$ symbols $+$ (addition) or $\times$ (multiplication) into this string to form a valid arithmetic expression.</p><p>In this problem, the symbols cannot be placed before the first or after the last character of the string $s$, and two symbols cannot be written consecutively. Also, note that the order of the digits in the string cannot be changed. Let's consider $s = 987009$:</p><ul><li> From this string, the following arithmetic expressions can be obtained: $9 \times 8 + 70 \times 0 + 9 = 81$, $98 \times 7 \times 0 + 0 \times 9 = 0$, $9 + 8 + 7 + 0 + 09 = 9 + 8 + 7 + 0 + 9 = 33$. Note that the number $09$ is considered valid and is simply transformed into $9$.</li><li> From this string, the following arithmetic expressions cannot be obtained: $+9 \times 8 \times 70 + 09$ (symbols should only be placed between digits), $98 \times 70 + 0 + 9$ (since there are $6$ digits, there must be exactly $4$ symbols).</li></ul><p>The result of the arithmetic expression is calculated according to the rules of mathematics&nbsp;！ first all multiplication operations are performed, then addition. You need to find the minimum result that can be obtained by inserting exactly $n - 2$ addition or multiplication symbols into the given string $s$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. Then follows their description.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 20$)&nbsp;！ the length of the string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of digits from $0$ to $9$.</p></div><div class="output-specification"><p>For each test case, output the minimum result of the arithmetic expression that can be obtained by inserting exactly $n - 2$ addition or multiplication symbols into the given string.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. Then follows their description.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 20$)&nbsp;！ the length of the string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of digits from $0$ to $9$.</p>

## Output

<p>For each test case, output the minimum result of the arithmetic expression that can be obtained by inserting exactly $n - 2$ addition or multiplication symbols into the given string.</p>





```input1|2,3,6,7,10,11,14,15,18,19,22,23,26,27,30,31,34,35
18
2
10
2
74
2
00
2
01
3
901
3
101
5
23311
6
987009
7
1111111
20
99999999999999999999
20
00000000000000000000
4
0212
18
057235283621345395
4
1112
20
19811678487321784121
4
1121
4
2221
3
011
```




```output1
10
74
0
1
9
1
19
0
11
261
0
0
0
12
93
12
24
0
```



## Note

<p>In the first four test cases, we cannot add symbols, so the answer will be the original number.</p><p>In the fifth test case, the optimal answer looks as follows: $9 \times 01 = 9 \times 1 = 9$.</p><p>In the sixth test case, the optimal answer looks as follows: $1 \times 01 = 1 \times 1 = 1$.</p><p>In the seventh test case, the optimal answer looks as follows: $2 + 3 + 3 + 11 = 19$.</p><p>In the eighth test case, one of the optimal answers looks as follows: $98 \times 7 \times 0 + 0 \times 9 = 0$.</p>
