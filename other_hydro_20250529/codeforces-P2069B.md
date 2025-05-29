## Description

<div><p>You are given a table of $n$ rows and $m$ columns. Initially, the cell at the $i$-th row and the $j$-th column has color $a_{i, j}$.</p><p>Let's say that two cells are <span class="tex-font-style-it">strangers</span> if they <span class="tex-font-style-bf">don't</span> share a side. Strangers are allowed to touch with corners.</p><p>Let's say that the set of cells is a <span class="tex-font-style-it">set of strangers</span> if all pairs of cells in the set are strangers. Sets with no more than one cell are sets of strangers by definition.</p><p>In one step, you can choose any set of strangers <span class="tex-font-style-bf">such that all cells in it have the same color</span> and paint all of them in some other color. You can choose the resulting color.</p><p>What is the minimum number of steps you need to make the whole table the same color?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Next, $t$ cases follow.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le m \le 700$)&nbsp;！ the number of rows and columns in the table.</p><p>The next $n$ lines contain the colors of cells in the corresponding row $a_{i, 1}, \dots, a_{i, m}$ ($1 \le a_{i, j} \le nm$).</p><p>It's guaranteed that the total sum of $nm$ doesn't exceed $5 \cdot 10^5$ over all test cases.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;！ the minimum number of steps to paint all cells of the table the same color.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Next, $t$ cases follow.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le m \le 700$)&nbsp;！ the number of rows and columns in the table.</p><p>The next $n$ lines contain the colors of cells in the corresponding row $a_{i, 1}, \dots, a_{i, m}$ ($1 \le a_{i, j} \le nm$).</p><p>It's guaranteed that the total sum of $nm$ doesn't exceed $5 \cdot 10^5$ over all test cases.</p>

## Output

<p>For each test case, print one integer&nbsp;！ the minimum number of steps to paint all cells of the table the same color.</p>





```input1|2,3,8,9
4
1 1
1
3 3
1 2 1
2 3 2
1 3 1
1 6
5 4 5 4 4 5
3 4
1 4 2 2
1 4 3 5
6 6 3 5
```




```output1
0
2
1
10
```



## Note

<p>In the first test case, the table is painted in one color from the start.</p><p>In the second test case, you can, for example, choose all cells with color $1$ and paint them in $3$. Then choose all cells with color $2$ and also paint them in $3$.</p><p>In the third test case, you can choose all cells with color $5$ and paint them in color $4$.</p>
