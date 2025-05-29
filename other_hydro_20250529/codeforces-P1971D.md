## Description

<div><p>You are given a binary string$^{\dagger}$. Please find the minimum number of pieces you need to cut it into, so that the resulting pieces can be rearranged into a sorted binary string.</p><center> <img class="tex-graphics" src="./34655/file/wh6XPt9Y.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that: </p><ul> <li> each character must lie in exactly one of the pieces; </li><li> the pieces must be contiguous substrings of the original string; </li><li> you must use all the pieces in the rearrangement. </li></ul><p>$^{\dagger}$ A <span class="tex-font-style-it">binary string</span> is a string consisting of characters $\texttt{0}$ and $\texttt{1}$. A <span class="tex-font-style-it">sorted binary string</span> is a binary string such that all characters $\texttt{0}$ come before all characters $\texttt{1}$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 500$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a single string $s$ ($1 \leq |s| \leq 500$) consisting of characters $\texttt{0}$ and $\texttt{1}$, where $|s|$ denotes the length of the string $s$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of pieces needed to be able to rearrange the string into a sorted binary string.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 500$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a single string $s$ ($1 \leq |s| \leq 500$) consisting of characters $\texttt{0}$ and $\texttt{1}$, where $|s|$ denotes the length of the string $s$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of pieces needed to be able to rearrange the string into a sorted binary string.</p>





```input1|2,4,6
6
11010
00000000
1
10
0001111
0110
```




```output1
3
1
1
2
1
2
```



## Note

<p>The first test case is pictured in the statement. It can be proven that you can't use fewer than $3$ pieces.</p><p>In the second and third test cases, the binary string is already sorted, so only $1$ piece is needed.</p><p>In the fourth test case, you need to make a single cut between the two characters and rearrange them to make the string $\texttt{01}$.</p>
