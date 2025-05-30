## Description

<div><p>It is given a non-negative integer $x$, the decimal representation of which contains $n$ digits. You need to color <span class="tex-font-style-bf">each</span> its digit in red or black, so that the number formed by the red digits is divisible by $A$, and the number formed by the black digits is divisible by $B$.</p><p><span class="tex-font-style-bf">At least one</span> digit must be colored in each of two colors. Consider, the count of digits colored in red is $r$ and the count of digits colored in black is $b$. Among all possible colorings of the given number $x$, you need to output any such that the value of $|r - b|$ is <span class="tex-font-style-bf">the minimum possible</span>.</p><p>Note that the number $x$ and the numbers formed by digits of each color, <span class="tex-font-style-bf">may contain leading zeros</span>.</p><center> <img class="tex-graphics" src="./32459/file/0BxjQjnR.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Example of painting a number for $A = 3$ and $B = 13$</span> </center><p>The figure above shows an example of painting the number $x = 02165$ of $n = 5$ digits for $A = 3$ and $B = 13$. The red digits form the number $015$, which is divisible by $3$, and the black ones �� $26$, which is divisible by $13$. Note that the absolute value of the difference between the counts of red and black digits is $1$, it is impossible to achieve a smaller value.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10$) �� the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of two lines. The first line contains three integers $n$, $A$, $B$ ($2 \le n \le 40$, $1 \le A, B \le 40$). The second line contains a non-negative integer $x$ containing exactly $n$ digits and probably containing leading zeroes.</p></div><div class="output-specification"><p>For each test case, output in a separate line:</p><ul> <li> <span class="tex-font-style-tt">-1</span> if the desired coloring does not exist; </li><li> a string $s$ of $n$ characters, each of them is a letter '<span class="tex-font-style-tt">R</span>' or '<span class="tex-font-style-tt">B</span>'. If the $i$-th digit of the number $x$ is colored in red, then the $i$-th character of the string $s$ must be the letter '<span class="tex-font-style-tt">R</span>', otherwise the letter '<span class="tex-font-style-tt">B</span>'. </li></ul><p>The number formed by digits colored red should divisible by $A$. The number formed by digits colored black should divisible by $B$. The value $|r-b|$ should be minimal, where $r$ is the count of red digits, $b$ is the count of black digits. If there are many possible answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10$) �� the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of two lines. The first line contains three integers $n$, $A$, $B$ ($2 \le n \le 40$, $1 \le A, B \le 40$). The second line contains a non-negative integer $x$ containing exactly $n$ digits and probably containing leading zeroes.</p>

## Output

<p>For each test case, output in a separate line:</p><ul> <li> <span class="tex-font-style-tt">-1</span> if the desired coloring does not exist; </li><li> a string $s$ of $n$ characters, each of them is a letter '<span class="tex-font-style-tt">R</span>' or '<span class="tex-font-style-tt">B</span>'. If the $i$-th digit of the number $x$ is colored in red, then the $i$-th character of the string $s$ must be the letter '<span class="tex-font-style-tt">R</span>', otherwise the letter '<span class="tex-font-style-tt">B</span>'. </li></ul><p>The number formed by digits colored red should divisible by $A$. The number formed by digits colored black should divisible by $B$. The value $|r-b|$ should be minimal, where $r$ is the count of red digits, $b$ is the count of black digits. If there are many possible answers, print any of them.</p>

## Samples

```input1
4
5 3 13
02165
4 2 1
1357
8 1 1
12345678
2 7 9
90
```

```output1
RBRBR
-1
BBRRRRBB
BR
```




## Note

<p>The first test case is considered in the statement.</p><p>In the second test case, there are no even digits, so it is impossible to form a number from its digits that is divisible by $2$.</p><p>In the third test case, each coloring containing at least one red and one black digit is possible, so you can color $4$ digits in red and $4$ in black ($|4 - 4| = 0$, it is impossible to improve the result).</p><p>In the fourth test case, there is a single desired coloring.</p>
