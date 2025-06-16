## Description

<div><p>You received an $n\times m$ grid from a mysterious source. The source also gave you a magic positive integer constant $k$.</p><p>The source told you to color the grid with some colors, satisfying the following condition:</p><ul> <li> If $(x_1,y_1)$, $(x_2,y_2)$ are two distinct cells with the same color, then $\max(|x_1-x_2|,|y_1-y_2|)\ge k$. </li></ul><p>You don't like using too many colors. Please find the minimum number of colors needed to color the grid.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le1000$). The description of the test cases follows.</p><p>The only line of each test case consists of three positive integers $n$, $m$, $k$ ($1\le n,m,k\le10^4$)&nbsp;！ the dimensions of the grid and the magic constant.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the minimum number of colors needed to color the grid.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\le t\le1000$). The description of the test cases follows.</p><p>The only line of each test case consists of three positive integers $n$, $m$, $k$ ($1\le n,m,k\le10^4$)&nbsp;！ the dimensions of the grid and the magic constant.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the minimum number of colors needed to color the grid.</p>





```input1|2,4,6
6
3 3 2
5 1 10000
7 3 4
3 2 7
8 9 6
2 5 4
```




```output1
4
5
12
6
36
8
```



## Note

<p>In the first test case, one of the optimal constructions is:</p><center> <img class="tex-graphics" src="./34868/file/NeTHtblc.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second test case, the color of all cells must be pairwise different, so the answer is $5$.</p>
