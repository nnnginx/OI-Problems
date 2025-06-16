## Description

<div><p>For the final of the first Olympiad by IT Campus "NEIMARK", a rectangular venue was prepared. You may assume that the venue is divided into $n$ rows, each containing $m$ spots for participants' desks. A total of $k$ participants have registered for the final, and each participant will sit at an individual desk. Now, the organizing committee must choose the locations for the desks in the venue.</p><p>Each desk occupies one of the $m$ spots in a row. Moreover, if several desks occupy consecutive spots in the same row, we call such a group of desks a <span class="tex-font-style-it">bench</span>, and the number of desks in the group is the bench's length. For example, seating $7$ participants on a $3 \times 4$ venue (with $n = 3, m = 4$) can be arranged as follows:</p><center> <img class="tex-graphics" src="./37200/file/kCZTVuiJ.png" style="max-width: 100.0%;max-height: 100.0%;" width="266px"> </center><p>In the figure above, the first row has one bench of length $3$, the second row has one bench of length $2$, and the third row has two benches of length $1$.</p><p>The organizing committee wants to choose the locations so that the length of the longest bench is as small as possible. In particular, the same $7$ desks can be arranged in a more optimal way, so that the lengths of all benches do not exceed $2$:</p><center> <img class="tex-graphics" src="./37200/file/4b5BSviN.png" style="max-width: 100.0%;max-height: 100.0%;" width="266px"> </center><p>Given the integers $n$, $m$, and $k$, determine the minimum possible length of the longest bench.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). The description of the test cases follows.</p><p>A single line of each test case contains three positive integers&nbsp;！ $n$, $m$, $k$ ($1 \leq n, m, k \leq 10^9$, $k \leq n\cdot m$).</p></div><div class="output-specification"><p>For each test case, output a single number&nbsp;！ the minimum possible length of the longest bench.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). The description of the test cases follows.</p><p>A single line of each test case contains three positive integers&nbsp;！ $n$, $m$, $k$ ($1 \leq n, m, k \leq 10^9$, $k \leq n\cdot m$).</p>

## Output

<p>For each test case, output a single number&nbsp;！ the minimum possible length of the longest bench.</p>





```input1|2,4,6
5
3 4 7
5 5 5
1 13 2
2 4 7
1 5 4
```




```output1
2
1
1
4
2
```


