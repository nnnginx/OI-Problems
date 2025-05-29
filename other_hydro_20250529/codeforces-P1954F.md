## Description

<div><p>Let's say that two strings $a$ and $b$ are <span class="tex-font-style-bf">equal</span> if you can get the string $b$ by cyclically shifting string $a$. For example, the strings <span class="tex-font-style-tt">0100110</span> and <span class="tex-font-style-tt">1100100</span> are equal, while <span class="tex-font-style-tt">1010</span> and <span class="tex-font-style-tt">1100</span> are not.</p><p>You are given a binary string $s$ of length $n$. Its first $c$ characters are <span class="tex-font-style-tt">1</span>-s, and its last $n - c$ characters are <span class="tex-font-style-tt">0</span>-s.</p><p>In one operation, you can replace one <span class="tex-font-style-tt">0</span> with <span class="tex-font-style-tt">1</span>.</p><p>Calculate the number of unique strings you can get using no more than $k$ operations. Since the answer may be too large, print it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first and only line contains three integers $n$, $c$ and $k$ ($1 \le n \le 3000$; $1 \le c \le n$; $0 \le k \le n - c$)&nbsp;！ the length of string $s$, the length of prefix of <span class="tex-font-style-tt">1</span>-s and the maximum number of operations.</p></div><div class="output-specification"><p>Print the single integer&nbsp;！ the number of <span class="tex-font-style-bf">unique</span> strings you can achieve performing no more than $k$ operations, modulo $10^9 + 7$.</p></div>

## Input

<p>The first and only line contains three integers $n$, $c$ and $k$ ($1 \le n \le 3000$; $1 \le c \le n$; $0 \le k \le n - c$)&nbsp;！ the length of string $s$, the length of prefix of <span class="tex-font-style-tt">1</span>-s and the maximum number of operations.</p>

## Output

<p>Print the single integer&nbsp;！ the number of <span class="tex-font-style-bf">unique</span> strings you can achieve performing no more than $k$ operations, modulo $10^9 + 7$.</p>





```input1|
1 1 0
```




```input2|
3 1 2
```




```input3|
5 1 1
```




```input4|
6 2 2
```




```input5|
24 3 11
```




```output1
1
```




```output2
3
```




```output3
3
```




```output4
7
```




```output5
498062
```



## Note

<p>In the first test case, the only possible string is <span class="tex-font-style-tt">1</span>.</p><p>In the second test case, the possible strings are: <span class="tex-font-style-tt">100</span>, <span class="tex-font-style-tt">110</span>, and <span class="tex-font-style-tt">111</span>. String <span class="tex-font-style-tt">101</span> is equal to <span class="tex-font-style-tt">110</span>, so we don't count it.</p><p>In the third test case, the possible strings are: <span class="tex-font-style-tt">10000</span>, <span class="tex-font-style-tt">11000</span>, <span class="tex-font-style-tt">10100</span>. String <span class="tex-font-style-tt">10010</span> is equal to <span class="tex-font-style-tt">10100</span>, and <span class="tex-font-style-tt">10001</span> is equal to <span class="tex-font-style-tt">11000</span>.</p>
