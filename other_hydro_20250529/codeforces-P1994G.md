## Description

<div><p>After winning another Bed Wars game, Masha and Olya wanted to relax and decided to play a new game. Masha gives Olya an array $a$ of length $n$ and a number $s$. Now Olya's task is to find a non-negative number $x$ such that $\displaystyle\sum_{i=1}^{n} a_i \oplus x = s$. But she is very tired after a tight round, so please help her with this.</p><p>But this task seemed too simple to them, so they decided to make the numbers larger (up to $2^k$) and provide you with their binary representation.</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n, k, n \cdot k \le 2 \cdot 10^6$)&nbsp;！ the length of the array $a$ and the length of the binary representation of all numbers.</p><p>The second line contains a string of length $k$, consisting of zeros and ones&nbsp;！ the binary representation of the number $s$, starting from the most significant bits.</p><p>The next $n$ lines also contain strings of length $k$, consisting of zeros and ones, the $i$-th of these strings contains the binary representation of the number $a_i$, starting from the most significant bits.</p><p>It is guaranteed that the sum of the values $n \cdot k$ for all test cases does not exceed $2 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output a string of length $k$ on a separate line, consisting of zeros or ones&nbsp;！ the binary representation of any suitable number $x$ ($x \ge 0$), starting from the most significant bits, or $-1$ if such $x$ does not exist.</p></div>

## Input

<p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n, k, n \cdot k \le 2 \cdot 10^6$)&nbsp;！ the length of the array $a$ and the length of the binary representation of all numbers.</p><p>The second line contains a string of length $k$, consisting of zeros and ones&nbsp;！ the binary representation of the number $s$, starting from the most significant bits.</p><p>The next $n$ lines also contain strings of length $k$, consisting of zeros and ones, the $i$-th of these strings contains the binary representation of the number $a_i$, starting from the most significant bits.</p><p>It is guaranteed that the sum of the values $n \cdot k$ for all test cases does not exceed $2 \cdot 10^6$.</p>

## Output

<p>For each test case, output a string of length $k$ on a separate line, consisting of zeros or ones&nbsp;！ the binary representation of any suitable number $x$ ($x \ge 0$), starting from the most significant bits, or $-1$ if such $x$ does not exist.</p>





```input1|2,3,4,5,6,7,12,13,14,15,16,17,18
4
4 5
01011
01110
00110
01100
01111
2 8
00101001
10111111
10011110
5 4
0101
0010
0000
0000
0010
0011
6 5
00011
10110
11001
01010
11100
10011
10000
```




```output1
01110
10011010
0010
-1
```



## Note

<p>In the first test case, $s = 11, a = [14, 6, 12, 15]$, if $x = 14$, then $\displaystyle\sum_{i=1}^{n} a_i \oplus x = (14 \oplus 14) + (6 \oplus 14) + (12 \oplus 14) + (15 \oplus 14) = 0 + 8 + 2 + 1 = 11 = s$.</p><p>In the second test case, $s = 41, a = [191, 158]$, if $x = 154$, then $\displaystyle\sum_{i=1}^{n} a_i \oplus x = (191 \oplus 154) + (158 \oplus 154) = 37 + 4 = 41 = s$.</p>
