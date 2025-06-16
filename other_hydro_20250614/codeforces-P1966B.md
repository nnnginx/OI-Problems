## Description

<div><p>There is an $n \times m$ grid of white and black squares. In one operation, you can select any two squares of the same color, and color all squares in the subrectangle between them that color.</p><p>Formally, if you select positions $(x_1, y_1)$ and $(x_2, y_2)$, both of which are currently the same color $c$, set the color of all $(x, y)$ where $\min(x_1, x_2) \le x \le \max(x_1, x_2)$ and $\min(y_1, y_2) \le y \le \max(y_1, y_2)$ to $c$.</p><p>This diagram shows a sequence of two possible operations on a grid:</p><center> <img class="tex-graphics" src="./34608/file/4kBgHxNp.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Is it possible for all squares in the grid to be the same color, after performing any number of operations (possibly zero)?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 500$)&nbsp;！ the number of rows and columns in the grid, respectively.</p><p>Each of the next $n$ lines contains $m$ characters '<span class="tex-font-style-tt">W</span>' and '<span class="tex-font-style-tt">B</span>'&nbsp;！ the initial colors of the squares of the grid. </p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $3\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if it is possible to make all squares in the grid the same color, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 500$)&nbsp;！ the number of rows and columns in the grid, respectively.</p><p>Each of the next $n$ lines contains $m$ characters '<span class="tex-font-style-tt">W</span>' and '<span class="tex-font-style-tt">B</span>'&nbsp;！ the initial colors of the squares of the grid. </p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $3\cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if it is possible to make all squares in the grid the same color, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,4,12,13,17,18,19,20,26,27,28,29,30
8
2 1
W
B
6 6
WWWWBW
WBWWWW
BBBWWW
BWWWBB
WWBWBB
BBBWBW
1 1
W
2 2
BB
BB
3 4
BWBW
WBWB
BWBW
4 2
BB
BB
WW
WW
4 4
WWBW
BBWB
WWBB
BBBB
1 5
WBBWB
```




```output1
NO
YES
YES
YES
YES
NO
YES
NO
```



## Note

<p>In the first example, it is impossible to ever change the color of any square with an operation, so we output <span class="tex-font-style-tt">NO</span>.</p><p>The second example is the case pictured above. As shown in that diagram, it is possible for all squares to be white after two operations, so we output <span class="tex-font-style-tt">YES</span>.</p><p>In the third and fourth examples, all squares are already the same color, so we output <span class="tex-font-style-tt">YES</span>.</p><p>In the fifth example we can do everything in two operations. First, select positions $(2, 1)$ and $(1, 4)$ and color all squares with $1 \le x \le 2$ and $1 \le y \le 4$ to white. Then, select positions $(2, 1)$ and $(3, 4)$ and color all squares with $2 \le x \le 3$ and $1 \le y \le 4$ to white. After these two operations all squares are white.</p>
