## Description

<div><p>For each integer $x$ from $1$ to $n$, we will form the string $S(x)$ according to the following rules:</p><ul> <li> compute $(x+1)$; </li><li> write $x$ and $x+1$ next to each other in the decimal system without separators and leading zeros; </li><li> in the resulting string, sort all digits in non-decreasing order. </li></ul><p>For example, the string $S(139)$ is <span class="tex-font-style-tt">011349</span> (before sorting the digits, it is <span class="tex-font-style-tt">139140</span>). The string $S(99)$ is <span class="tex-font-style-tt">00199</span>.</p><p>Your task is to count the number of distinct strings among $S(1), S(2), \dots, S(n)$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>Each test case consists of one line containing a single integer $n$ ($1 \le n \le 10^{9} - 2$).</p></div><div class="output-specification"><p>For each test case, output a single integer ！ the number of distinct strings among $S(1), S(2), \dots, S(n)$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases.</p><p>Each test case consists of one line containing a single integer $n$ ($1 \le n \le 10^{9} - 2$).</p>

## Output

<p>For each test case, output a single integer ！ the number of distinct strings among $S(1), S(2), \dots, S(n)$.</p>





```input1|2
2
42
1337
```




```output1
42
948
```


