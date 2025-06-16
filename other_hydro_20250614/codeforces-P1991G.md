## Description

<div><p>You are given a grid consisting of $n$ rows and $m$ columns, where each cell is initially white. Additionally, you are given an integer $k$, where $1 \le k \le \min(n, m)$.</p><p>You will process $q$ operations of two types: </p><ul> <li> $\mathtt{H}$ (horizontal operation)&nbsp;！ You choose a $1 \times k$ rectangle completely within the grid, where all cells in this rectangle are white. Then, all cells in this rectangle are changed to black. </li><li> $\mathtt{V}$ (vertical operation)&nbsp;！ You choose a $k \times 1$ rectangle completely within the grid, where all cells in this rectangle are white. Then, all cells in this rectangle are changed to black. </li></ul><p>After each operation, if any rows or columns become completely black, all cells in these rows and columns are <span class="tex-font-style-bf">simultaneously</span> reset to white. Specifically, if all cells in the row and column a cell is contained in become black, all cells in both the row and column will be reset to white.</p><p>Choose the rectangles in a way that you can perform all given operations, or determine that it is impossible.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains four integers $n$, $m$, $k$, and $q$ ($1 \le n, m \le 100$, $1 \le k \le \min(n, m)$, $1 \le q \le 1000$)&nbsp;！ the number of rows and columns in the grid, the size of the operation rectangle, and the number of operations, respectively.</p><p>The second line of each test case contains a string $s$ of length $q$, consisting only of characters $\mathtt{H}$ and $\mathtt{V}$&nbsp;！ the sequence of operation types.</p><p>It is guaranteed that the sum of $q$ over all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, output a single integer $-1$ if it is impossible to perform all the operations.</p><p>Otherwise, output $q$ lines. Each line contains two integers $i$, $j$ ($1 \le i \le n$, $1 \le j \le m$)&nbsp;！ the coordinates of the top-left cell of the operation rectangle.</p><p>If there are multiple solutions, output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains four integers $n$, $m$, $k$, and $q$ ($1 \le n, m \le 100$, $1 \le k \le \min(n, m)$, $1 \le q \le 1000$)&nbsp;！ the number of rows and columns in the grid, the size of the operation rectangle, and the number of operations, respectively.</p><p>The second line of each test case contains a string $s$ of length $q$, consisting only of characters $\mathtt{H}$ and $\mathtt{V}$&nbsp;！ the sequence of operation types.</p><p>It is guaranteed that the sum of $q$ over all test cases does not exceed $1000$.</p>

## Output

<p>For each test case, output a single integer $-1$ if it is impossible to perform all the operations.</p><p>Otherwise, output $q$ lines. Each line contains two integers $i$, $j$ ($1 \le i \le n$, $1 \le j \le m$)&nbsp;！ the coordinates of the top-left cell of the operation rectangle.</p><p>If there are multiple solutions, output any of them.</p>





```input1|2,3
1
4 5 3 6
HVVHHV
```




```output1
1 1
2 1
1 1
2 3
3 3
2 2
```



## Note

<center> <img class="tex-graphics" src="./34795/file/X3rygLsw.png" style="max-width: 100.0%;max-height: 100.0%;" width="416px"> <span class="tex-font-style-it">Illustration of example.</span> </center><p>The first operation is horizontal. The operation rectangle starts at $(1,1)$ and is a $1 \times 3$ rectangle. After the operation, cells $(1,1)$, $(1,2)$, and $(1,3)$ become black.</p><p>The second operation is vertical. The operation rectangle starts at $(2,1)$ and is a $3 \times 1$ rectangle. After the operation, cells $(2,1)$, $(3,1)$, and $(4,1)$ become black. At this point, the first column becomes completely black, so all cells in the first column are reset to white.</p><p>The third operation is vertical. The operation rectangle starts at $(1,1)$ and is a $3 \times 1$ rectangle. After the operation, cells $(1,1)$, $(2,1)$, and $(3,1)$ become black.</p><p>The fourth operation is horizontal. The operation rectangle starts at $(2,3)$ and is a $1 \times 3$ rectangle. After the operation, cells $(2,3)$, $(2,4)$, and $(2,5)$ become black.</p><p>The fifth operation is horizontal. The operation rectangle starts at $(3,3)$ and is a $1 \times 3$ rectangle. After the operation, cells $(3,3)$, $(3,4)$, and $(3,5)$ become black.</p><p>The sixth operation is vertical. The operation rectangle starts at $(2,2)$ and is a $3 \times 1$ rectangle. After the operation, cells $(2,2)$, $(3,2)$, and $(4,2)$ become black. At this point, two rows and one column become completely black, so all cells in these rows and the column are reset to white.</p>
