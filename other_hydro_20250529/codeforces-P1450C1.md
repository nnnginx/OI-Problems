## Description

<div><p><span class="tex-font-style-bf">The only difference between the easy and hard versions is that tokens of type <span class="tex-font-style-tt">O</span> do not appear in the input of the easy version.</span></p><p><span class="tex-font-style-it">Errichto gave Monogon the following challenge in order to intimidate him from taking his top contributor spot on Codeforces.</span></p><p>In a Tic-Tac-Toe grid, there are $n$ rows and $n$ columns. Each cell of the grid is either empty or contains a token. There are two types of tokens: <span class="tex-font-style-tt">X</span> and <span class="tex-font-style-tt">O</span>. If there exist three tokens of the same type consecutive in a row or column, it is a winning configuration. Otherwise, it is a draw configuration.</p><center> <img class="tex-graphics" src="./31635/file/4Ti9ccqT.png" style="max-width: 100.0%;max-height: 100.0%;"> The patterns in the first row are winning configurations. The patterns in the second row are draw configurations. </center><p>In an operation, you can change an <span class="tex-font-style-tt">X</span> to an <span class="tex-font-style-tt">O</span>, or an <span class="tex-font-style-tt">O</span> to an <span class="tex-font-style-tt">X</span>. Let $k$ denote the total number of tokens in the grid. Your task is to make the grid a <span class="tex-font-style-bf">draw</span> in at most $\lfloor \frac{k}{3}\rfloor$ (rounding down) operations.</p><p>You are <span class="tex-font-style-bf">not required</span> to minimize the number of operations.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 100$) �� the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 300$) �� the size of the grid.</p><p>The following $n$ lines each contain a string of $n$ characters, denoting the initial grid. The character in the $i$-th row and $j$-th column is '<span class="tex-font-style-tt">.</span>' if the cell is empty, or it is the type of token in the cell: '<span class="tex-font-style-tt">X</span>' or '<span class="tex-font-style-tt">O</span>'.</p><p>It is guaranteed that not all cells are empty.</p><p>In the easy version, the character '<span class="tex-font-style-tt">O</span>' does not appear in the input.</p><p>The sum of $n$ across all test cases does not exceed $300$.</p></div><div class="output-specification"><p>For each test case, print the state of the grid after applying the operations.</p><p>We have proof that a solution always exists. If there are multiple solutions, print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 100$) �� the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\le n\le 300$) �� the size of the grid.</p><p>The following $n$ lines each contain a string of $n$ characters, denoting the initial grid. The character in the $i$-th row and $j$-th column is '<span class="tex-font-style-tt">.</span>' if the cell is empty, or it is the type of token in the cell: '<span class="tex-font-style-tt">X</span>' or '<span class="tex-font-style-tt">O</span>'.</p><p>It is guaranteed that not all cells are empty.</p><p>In the easy version, the character '<span class="tex-font-style-tt">O</span>' does not appear in the input.</p><p>The sum of $n$ across all test cases does not exceed $300$.</p>

## Output

<p>For each test case, print the state of the grid after applying the operations.</p><p>We have proof that a solution always exists. If there are multiple solutions, print any.</p>

## Samples

```input1
3
3
.X.
XXX
.X.
6
XX.XXX
XXXXXX
XXX.XX
XXXXXX
XX.X.X
XXXXXX
5
XXX.X
.X..X
XXX.X
..X..
..X..
```

```output1
.X.
XOX
.X.
XX.XXO
XOXXOX
OXX.XX
XOOXXO
XX.X.X
OXXOXX
XOX.X
.X..X
XXO.O
..X..
..X..
```




## Note

<p>In the first test case, there are initially three '<span class="tex-font-style-tt">X</span>' consecutive in the second row and the second column. By changing the middle token to '<span class="tex-font-style-tt">O</span>' we make the grid a draw, and we only changed $1\le \lfloor 5/3\rfloor$ token.</p><p>In the second test case, we change only $9\le \lfloor 32/3\rfloor$ tokens, and there does not exist any three '<span class="tex-font-style-tt">X</span>' or '<span class="tex-font-style-tt">O</span>' consecutive in a row or column, so it is a draw.</p><p>In the third test case, we change only $3\le \lfloor 12/3\rfloor$ tokens, and the resulting grid is a draw.</p>
