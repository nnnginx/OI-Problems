## Description

<div><p>Duelists Mouf and Fouad enter the arena, which is an $n \times m$ grid!</p><p>Fouad's monster starts at cell $(a, b)$, where rows are numbered $1$ to $n$ and columns $1$ to $m$.</p><p>Mouf and Fouad will keep duelling until the grid consists of only one cell.</p><p>In each turn: </p><ul> <li> Mouf first cuts the grid along a row or column line into two parts, discarding the part without Fouad's monster. Note that the grid must have at least two cells; otherwise, the game has already ended. </li><li> After that, in the same turn, Fouad moves his monster to any cell (possibly the same one it was in) within the remaining grid. </li></ul><center> <img class="tex-graphics" src="./37531/file/GBDEYTAG.png" style="max-width: 100.0%;max-height: 100.0%;" width="531px">   <span class="tex-font-size-small"><span class="tex-font-style-it">Visualization of the phases of the fourth test case.</span></span> </center><p>Mouf wants to minimize the number of turns, while Fouad wants to maximize them. How many turns will this epic duel last if both play optimally?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first and only line of each test case contains four integers $n$, $m$, $a$, and $b$ ($2 \le n, m \le 10^9$, $1 \le a \le n$, $1 \le b \le m$) ！ denoting the number of rows, the number of columns, the starting row of the monster, and the starting column of the monster, respectively.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number of turns this epic duel will last if both play optimally.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first and only line of each test case contains four integers $n$, $m$, $a$, and $b$ ($2 \le n, m \le 10^9$, $1 \le a \le n$, $1 \le b \le m$) ！ denoting the number of rows, the number of columns, the starting row of the monster, and the starting column of the monster, respectively.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number of turns this epic duel will last if both play optimally.</p>





```input1|2,4,6,8
8
2 2 1 1
3 3 2 2
2 7 1 4
2 7 2 2
8 9 4 6
9 9 5 5
2 20 2 11
22 99 20 70
```




```output1
2
4
4
3
6
8
6
10
```



## Note

<p>In the first test case, one possible duel sequence is as follows:</p><ul> <li> Turn 1: Mouf cuts the grid horizontally along the line between the rows $1$ and $2$, removing the bottom half and leaving a $1 \times 2$ grid. </li><li> Turn 1: Fouad's monster is at the cell $(1,1)$. </li><li> Turn 2: Mouf cuts the $1 \times 2$ grid again, removes one column, and isolates the cell $(1,1)$. </li></ul><p>The duel is completed in $2$ turns.</p><p>In the fourth case, one possible duel sequence is as follows:</p><ul> <li> Turn 1: Mouf cuts the grid vertically along the line between the columns $2$ and $3$, splitting it into a $2 \times 2$ and a $2 \times 5$ field, then removes the $2 \times 5$ part. </li><li> Turn 1: Fouad moves the monster to the cell $(1,1)$. </li><li> From this point on, the duel plays out just like the first test case！two more turns trim down the grid from $2 \times 2$ to a single $1 \times 1$ cell. </li></ul><p>In total, the duel is completed in $3$ turns.</p><p>You can refer to the pictures mentioned in the problem statement for illustrations of the fourth test case.</p>
