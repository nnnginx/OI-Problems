## Description

<div><p>There is a $n\times m$ grid with each cell initially white. You have to color all the cells one-by-one. After you color a cell, all the <span class="tex-font-style-bf">colored cells</span> furthest from it receive a penalty. Find a coloring order, where no cell has more than $3$ penalties.</p><p><span class="tex-font-style-bf">Note that $n$ and $m$ are both odd.</span></p><p>The distance metric used is the <a href="https://en.wikipedia.org/wiki/Chebyshev_distance">chessboard distance</a> while we decide ties between cells with <a href="https://en.wikipedia.org/wiki/Taxicab_geometry#Formal_definition">Manhattan distance</a>. Formally, a cell $(x_2, y_2)$ is further away than $(x_3, y_3)$ from a cell $(x_1, y_1)$ if one of the following holds: </p><ul> <li> $\max\big(\lvert x_1 - x_2 \rvert, \lvert y_1 - y_2 \rvert\big)&gt;\max\big(\lvert x_1 - x_3 \rvert, \lvert y_1 - y_3 \rvert\big)$ </li><li> $\max\big(\lvert x_1 - x_2 \rvert, \lvert y_1 - y_2 \rvert\big)=\max\big(\lvert x_1 - x_3 \rvert, \lvert y_1 - y_3 \rvert\big)$ <span class="tex-font-style-bf">and</span> $\lvert x_1 - x_2 \rvert + \lvert y_1 - y_2 \rvert&gt;\lvert x_1 - x_3 \rvert + \lvert y_1 - y_3 \rvert$ </li></ul><p>It can be proven that at least one solution always exists.</p><center> <img class="tex-graphics" src="./37714/file/4UKt3JL9.png" style="zoom: 100.0%;max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Example showing penalty changes after coloring the center of a $5 \times 5$ grid. The numbers indicate the penalty of the cells.</span> </center> </div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains two <span class="tex-font-style-bf">odd</span> integers $n$ and $m$ ($1 \le n, m \le 4999$) ¡ª the number of rows and columns. </p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each test case, output $n \cdot m$ lines where the $i$-th line should contain the coordinates of the $i$-th cell in your coloring order. If there are multiple solutions, print any of them.</p><p>The empty lines in the example output are just for increased readability. You're not required to print them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains two <span class="tex-font-style-bf">odd</span> integers $n$ and $m$ ($1 \le n, m \le 4999$) ¡ª the number of rows and columns. </p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $5000$.</p>

## Output

<p>For each test case, output $n \cdot m$ lines where the $i$-th line should contain the coordinates of the $i$-th cell in your coloring order. If there are multiple solutions, print any of them.</p><p>The empty lines in the example output are just for increased readability. You're not required to print them.</p>





```input1|2,4
3
3 3
1 1
1 5
```




```output1
2 1
2 3
2 2
1 1
3 2
3 3
3 1
1 3
1 2

1 1

1 2
1 4
1 5
1 1
1 3
```



## Note

<p>In the first test case, the grid can be colored as follows:</p><center> <img class="tex-graphics" src="./37714/file/4uHEIfIL.png" style="zoom: 100.0%;max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The numbers indicate the penalty of the cells.</span> </center>
