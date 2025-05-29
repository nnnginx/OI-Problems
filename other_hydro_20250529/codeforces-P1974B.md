## Description

<div><p>Polycarp has a string $s$, which consists of lowercase Latin letters. He encodes this string using the following algorithm:</p><ul> <li> first, he constructs a new auxiliary string $r$, which consists of all distinct letters of the string $s$, written in alphabetical order; </li><li> then the encoding happens as follows: each character in the string $s$ is replaced by its symmetric character from the string $r$ (the first character of the string $r$ will be replaced by the last, the second by the second from the end, and so on). </li></ul><p>For example, encoding the string $s$="<span class="tex-font-style-tt">codeforces</span>" happens as follows:</p><ul> <li> the string $r$ is obtained as "<span class="tex-font-style-tt">cdefors</span>"; </li><li> the first character $s_1$='<span class="tex-font-style-tt">c</span>' is replaced by '<span class="tex-font-style-tt">s</span>'; </li><li> the second character $s_2$='<span class="tex-font-style-tt">o</span>' is replaced by '<span class="tex-font-style-tt">e</span>'; </li><li> the third character $s_3$='<span class="tex-font-style-tt">d</span>' is replaced by '<span class="tex-font-style-tt">r</span>'; </li><li> ... </li><li> the last character $s_{10}$='<span class="tex-font-style-tt">s</span>' is replaced by '<span class="tex-font-style-tt">c</span>'. </li></ul><center> <img class="tex-graphics" src="./34669/file/HHflHMJE.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The string $r$ and replacements for $s$="<span class="tex-font-style-tt">codeforces</span>".</span> </center><p>Thus, the result of encoding the string $s$="<span class="tex-font-style-tt">codeforces</span>" is the string "<span class="tex-font-style-tt">serofedsoc</span>".</p><p>Write a program that performs decoding ！ that is, restores the original string $s$ from the encoding result.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the string $b$.</p><p>The second line of each test case contains a string $b$ of length $n$, consisting of lowercase Latin letters ！ the result of encoding the original string $s$.</p><p>It is guaranteed that the sum of the values of $n$ over all test cases in the test does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the string $s$ from which the encoding result $b$ was obtained.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the string $b$.</p><p>The second line of each test case contains a string $b$ of length $n$, consisting of lowercase Latin letters ！ the result of encoding the original string $s$.</p><p>It is guaranteed that the sum of the values of $n$ over all test cases in the test does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the string $s$ from which the encoding result $b$ was obtained.</p>





```input1|2,3,6,7,10,11
5
10
serofedsoc
3
ttf
9
tlrhgmaoi
1
w
15
hnndledmnhlttin
```




```output1
codeforces
fft
algorithm
w
meetinthemiddle
```


