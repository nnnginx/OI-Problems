## Description

<div><p>You are given two grids of numbers $a$ and $b$, with $n$ rows and $m$ columns. All the values in the grid are $0$, $1$ or $2$.</p><p>You can perform the following operation on $a$ any number of times: </p><ul> <li> Pick any subrectangle in the grid with length and width $\ge 2$. You are allowed to choose the entire grid as a subrectangle. </li><li> The subrectangle has four corners. Take any pair of diagonally opposite corners of the chosen subrectangle and add $1$ to their values modulo $3$. </li><li> For the pair of corners not picked, add $2$ to their values modulo $3$. </li></ul><p>Note that the operation only changes the values of the corners of the picked subrectangle.</p><p>Is it possible to convert the grid $a$ into grid $b$ by applying the above operation any number of times (possibly zero)?</p></div><div class="input-specification"><p>The first line contains an integer $t$, the number of testcases ($1 \le t \le 250$).</p><p>For each testcase:</p><p>The first line contains two integers $n$ and $m$, the number of rows and columns in the grid ($2 \le n,m \le 500$).</p><p>Each of the next n lines contain m characters ！ the $j$-th character of the $i$-th line represents $a_{i,j}$.</p><p>Each of the next n lines contain m characters ！ the $j$-th character of the $i$-th line represents $b_{i,j}$ ($0 \le a_{i,j}, b_{i,j} \le 2$).</p><p>It is guaranteed that the sum of $n$ over all test cases and the sum of $m$ over all test cases do not exceed $500$.</p></div><div class="output-specification"><p>For each test case print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to convert grid $a$ into grid $b$ and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>The first line contains an integer $t$, the number of testcases ($1 \le t \le 250$).</p><p>For each testcase:</p><p>The first line contains two integers $n$ and $m$, the number of rows and columns in the grid ($2 \le n,m \le 500$).</p><p>Each of the next n lines contain m characters ！ the $j$-th character of the $i$-th line represents $a_{i,j}$.</p><p>Each of the next n lines contain m characters ！ the $j$-th character of the $i$-th line represents $b_{i,j}$ ($0 \le a_{i,j}, b_{i,j} \le 2$).</p><p>It is guaranteed that the sum of $n$ over all test cases and the sum of $m$ over all test cases do not exceed $500$.</p>

## Output

<p>For each test case print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to convert grid $a$ into grid $b$ and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,4,5,6,7,8,18,19,20,21,22,23,24,25,26,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,56,57,58,59,60
7
3 3
000
000
000
111
111
111
4 4
0000
0000
0000
0000
2100
1200
0012
0021
4 4
1020
1200
1210
0000
0000
1200
2200
0000
3 3
012
012
012
010
111
011
8 8
00000000
00000000
00000000
00000000
00000000
00000000
00000000
10000000
00000000
01200000
02010000
00102000
00020100
00001020
00000210
10000000
2 7
0000000
0000000
2220111
0111222
2 7
0000000
0100010
2220111
1210202
```




```output1
YES
YES
YES
NO
YES
NO
YES
```



## Note

<p>In the first testcase, grid $a$ can be converted into $b$ in the following manner:</p><p>$\begin{matrix}\fbox{0} &amp; 0 &amp; \fbox{0}\\ 0 &amp; 0 &amp; 0\\ \fbox{0} &amp; 0 &amp; \fbox{0}\end{matrix} \Rightarrow \begin{matrix}1 &amp; 0 &amp; 2\\ 0 &amp; \fbox{0} &amp; \fbox{0}\\ 2 &amp; \fbox{0} &amp; \fbox{1}\end{matrix} \Rightarrow \begin{matrix}1 &amp; 0 &amp; 2\\ \fbox{0} &amp; \fbox{1} &amp; 2\\ \fbox{2} &amp; \fbox{2} &amp; 2\end{matrix} \Rightarrow \begin{matrix}1 &amp; \fbox{0} &amp; \fbox{2}\\ 1 &amp; 0 &amp; 2\\ 1 &amp; \fbox{0} &amp; \fbox{2}\end{matrix} \Rightarrow \begin{matrix}1 &amp; 1 &amp; 1\\ 1 &amp; \fbox{0} &amp; \fbox{2}\\ 1 &amp; \fbox{2} &amp; \fbox{0}\end{matrix} \Rightarrow \begin{matrix}1 &amp; 1 &amp; 1\\ 1 &amp; 1 &amp; 1\\ 1 &amp; 1 &amp; 1\end{matrix}$</p><p>Here, in each operation, the top-right and bottom-left corners highlighted by a box are incremented by $2$ modulo $3$, while the top-left and bottom-right corners are incremented by $1$ modulo $3$.</p><p>In the fourth testcase, it can be proven that it is not possible to convert grid $a$ into grid $b$ using the above-mentioned operations any number of times.</p>
