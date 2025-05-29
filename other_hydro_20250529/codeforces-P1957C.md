## Description

<div><p>You are given an $n \times n$ chessboard where you and the computer take turns alternatingly to place white rooks &amp; black rooks on the board respectively. While placing rooks, you have to ensure that no two rooks attack each other. Two rooks attack each other if they share the same row or column <span class="tex-font-style-bf">regardless of color</span>.</p><p>A valid move is placing a rook on a position ($r$, $c$) such that it doesn't attack any other rook.</p><p>You start first, and when you make a valid move in your turn, placing a white rook at position ($r$, $c$), the computer will mirror you and place a black rook at position ($c$, $r$) in its turn. If $r = c$, then the computer can't mirror your move, and skips its turn.</p><p>You have already played $k$ moves with the computer (the computer tries to mirror these moves too), and you must continue playing the game until there are no valid moves remaining. How many different final configurations are possible when you continue the game after the $k$ moves? It is guaranteed that the $k$ moves and the implied computer moves are valid. Since the answer may be large, print it modulo $10^9+7$.</p><p>Two configurations are considered different if there exists a coordinate ($r$, $c$) which has a rook in one configuration, but not in the other <span class="tex-font-style-bf">or</span> the color of the rook on the coordinate is different.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 3 \cdot 10^5$, $0 \leq k \leq n$)&nbsp;！ the size of the chessboard and the number of moves you have already played respectively.</p><p>Each of the next $k$ lines of the test case contains two integers $r_i$ and $c_i$, denoting the $i$-th move you made.</p><p>It is guaranteed that the $k$ moves and the implied computer moves are valid.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer on a new line&nbsp;！ the total number of possible final configurations modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 3 \cdot 10^5$, $0 \leq k \leq n$)&nbsp;！ the size of the chessboard and the number of moves you have already played respectively.</p><p>Each of the next $k$ lines of the test case contains two integers $r_i$ and $c_i$, denoting the $i$-th move you made.</p><p>It is guaranteed that the $k$ moves and the implied computer moves are valid.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer on a new line&nbsp;！ the total number of possible final configurations modulo $10^9+7$.</p>





```input1|2,3,6,7,8,9,10
3
4 1
1 2
8 1
7 6
1000 4
4 4
952 343
222 333
90 91
```




```output1
3
331
671968183
```



## Note

<p>In the first test case, we have a $4 \times 4$ grid and you've already played $1$ move. After you and the computer play a turn, we have a white rook at ($1$, $2$), and a black rook at ($2$, $1$). There are three possible configurations from this state&nbsp;！</p><ol> <li> You place a white rook at ($3$, $4$) and the computer places a black rook at ($4$, $3$) as a response. </li><li> You place a white rook at ($4$, $3$) and the computer places a black rook at ($3$, $4$) as a response. </li><li> You place a white rook at ($3$, $3$) and then at ($4$, $4$), or the other way around. They both result in the same configuration. </li></ol><center> <img class="tex-graphics" src="./34586/file/59KDhxjc.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
