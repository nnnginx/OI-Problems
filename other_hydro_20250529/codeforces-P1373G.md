## Description

<div><p>You are given a chessboard consisting of $n$ rows and $n$ columns. Rows are numbered from bottom to top from $1$ to $n$. Columns are numbered from left to right from $1$ to $n$. The cell at the intersection of the $x$-th column and the $y$-th row is denoted as $(x, y)$. Furthermore, the $k$-th column is a special column. </p><p>Initially, the board is empty. There are $m$ changes to the board. During the $i$-th change one pawn is added or removed from the board. The current board is good if we can move all pawns to the special column by the followings rules:</p><ul> <li> Pawn in the cell $(x, y)$ can be moved to the cell $(x, y + 1)$, $(x - 1, y + 1)$ or $(x + 1, y + 1)$; </li><li> You can make as many such moves as you like; </li><li> Pawns can not be moved outside the chessboard; </li><li> Each cell can not contain more than one pawn. </li></ul><p>The current board may not always be good. To fix it, you can add new rows to the board. New rows are added at the top, i. e. they will have numbers $n+1, n+2, n+3, \dots$.</p><p>After each of $m$ changes, print one integer — the minimum number of rows which you have to add to make the board good.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $k$ and $m$ ($1 \le n, m \le 2 \cdot 10^5; 1 \le k \le n$) — the size of the board, the index of the special column and the number of changes respectively.</p><p>Then $m$ lines follow. The $i$-th line contains two integers $x$ and $y$ ($1 \le x, y \le n$) — the index of the column and the index of the row respectively. If there is no pawn in the cell $(x, y)$, then you add a pawn to this cell, otherwise — you remove the pawn from this cell.</p></div><div class="output-specification"><p>After each change print one integer — the minimum number of rows which you have to add to make the board good.</p></div>

## Input

<p>The first line contains three integers $n$, $k$ and $m$ ($1 \le n, m \le 2 \cdot 10^5; 1 \le k \le n$) — the size of the board, the index of the special column and the number of changes respectively.</p><p>Then $m$ lines follow. The $i$-th line contains two integers $x$ and $y$ ($1 \le x, y \le n$) — the index of the column and the index of the row respectively. If there is no pawn in the cell $(x, y)$, then you add a pawn to this cell, otherwise — you remove the pawn from this cell.</p>

## Output

<p>After each change print one integer — the minimum number of rows which you have to add to make the board good.</p>

## Samples

```input1
5 3 5
4 4
3 5
2 4
3 4
3 5
```

```output1
0
1
2
2
1
```



