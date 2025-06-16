## Description

<div><p>A binary string $s$ of length $n$ is given. A binary string is a string consisting only of the characters '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">0</span>'.</p><p>You can choose an integer $k$ ($1 \le k \le n$) and then apply the following operation any number of times: choose $k$ consecutive characters of the string and invert them, i.e., replace all '<span class="tex-font-style-tt">0</span>' with '<span class="tex-font-style-tt">1</span>' and vice versa.</p><p>Using these operations, you need to make all the characters in the string equal to '<span class="tex-font-style-tt">1</span>'.</p><p>For example, if $n=5$, $s=00100$, you can choose $k=3$ and proceed as follows: </p><ul> <li> choose the substring from the $1$-st to the $3$-rd character and obtain $s=\color{blue}{110}00$; </li><li> choose the substring from the $3$-rd to the $5$-th character and obtain $s=11\color{blue}{111}$; </li></ul><p>Find the maximum value of $k$ for which it is possible to make all the characters in the string equal to '<span class="tex-font-style-tt">1</span>' using the described operations. Note that the number of operations required to achieve this is not important.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 5000$)&nbsp;！ the length of the string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of the characters '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">0</span>'.</p><p>It is guaranteed that the sum of the values $n^2$ over all test cases in the test does not exceed $25 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output the maximum integer $k$ ($1 \le k \le n$) for which it is possible to obtain a string $s$ consisting only of the characters '<span class="tex-font-style-tt">1</span>' using the described operations.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 5000$)&nbsp;！ the length of the string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of the characters '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">0</span>'.</p><p>It is guaranteed that the sum of the values $n^2$ over all test cases in the test does not exceed $25 \cdot 10^6$.</p>

## Output

<p>For each test case, output the maximum integer $k$ ($1 \le k \le n$) for which it is possible to obtain a string $s$ consisting only of the characters '<span class="tex-font-style-tt">1</span>' using the described operations.</p>





```input1|2,3,6,7,10,11
5
5
00100
5
01000
7
1011101
3
000
2
10
```




```output1
3
2
4
3
1
```


