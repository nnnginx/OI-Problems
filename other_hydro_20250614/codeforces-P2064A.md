## Description

<div><p>One day after waking up, your friend challenged you to a brogramming contest. In a brogramming contest, you are given a binary string$^{\text{∗}}$ $s$ of length $n$ and an initially empty binary string $t$. During a brogramming contest, you can make either of the following moves any number of times: </p><ul> <li> remove some suffix$^{\text{†}}$ from $s$ and place it at the end of $t$, or </li><li> remove some suffix from $t$ and place it at the end of $s$. </li></ul> To win the brogramming contest, you must make the <span class="tex-font-style-it">minimum</span> number of moves required to make $s$ contain only the character $\texttt{0}$ and $t$ contain only the character $\texttt{1}$. Find the minimum number of moves required.<div class="statement-footnote"><p>$^{\text{∗}}$A <span class="tex-font-style-it">binary string</span> is a string consisting of characters $\texttt{0}$ and $\texttt{1}$.</p><p>$^{\text{†}}$A string $a$ is a suffix of a string $b$ if $a$ can be obtained from deletion of several (possibly, zero or all) elements from the beginning of $b$.</p></div></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case is an integer $n$ ($1 \le n \le 1000$)&nbsp;— the length of the string $s$.</p><p>The second line of each test case contains the binary string $s$.</p><p>The sum of $n$ across all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each testcase, output the minimum number of moves required.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case is an integer $n$ ($1 \le n \le 1000$)&nbsp;— the length of the string $s$.</p><p>The second line of each test case contains the binary string $s$.</p><p>The sum of $n$ across all test cases does not exceed $1000$.</p>

## Output

<p>For each testcase, output the minimum number of moves required.</p>





```input1|2,3,6,7,10,11
5
5
00110
4
1111
3
001
5
00000
3
101
```




```output1
2
1
1
0
3
```



## Note

<p>An optimal solution to the first test case is as follows:</p><ul> <li> $s = \texttt{00}\color{red}{\texttt{110}}$, $t =$ empty string. </li><li> $s = \texttt{00}$, $t = \texttt{11}\color{red}{\texttt{0}}$. </li><li> $s = \texttt{000}$, $t = \texttt{11}$. </li></ul><p>It can be proven that there is no solution using less than $2$ moves.</p><p>In the second test case, you have to move the whole string from $s$ to $t$ in one move.</p><p>In the fourth test case, you don't have to do any moves.</p>
