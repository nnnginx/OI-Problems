## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>You are given a grid with $n$ rows and $m$ columns. You need to fill each cell with a unique integer from $1$ to $n \cdot m$.</p><p>After filling the grid, you will play a game on this grid against the interactor. Players take turns selecting one of the previously unselected cells from the grid, with the interactor going first.</p><p>On the first turn, the interactor can choose any cell from the grid. After that, any chosen cell must be orthogonally adjacent to at least one previously selected cell. Two cells are considered orthogonally adjacent if they share an edge. The game continues until all cells have been selected.</p><p>Your goal is to let the sum of numbers in the cells selected by you be <span class="tex-font-style-bf">strictly</span> less than the sum of numbers in the cells selected by the interactor.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains two integers $n$ and $m$ ($4 \le n, m \le 10$)&nbsp;！ the number of rows and columns in the grid.</p></div><div><h2>Interaction</h2><p>First, output $n$ lines, each containing $m$ integers, representing the integers that you filled in the grid. Each integer from $1$ to $n \cdot m$ should appear exactly once.</p><p>Then, the game begins. The interactor and you take turns outputting coordinates to select a cell for $n \times m$ turns, with the interactor starting first.</p><p>On each player's (either you or the interactor) turn, the player will output two integers $i$ and $j$ ($1 \le i \le n$, $1 \le j \le m$), denoting that the player has selected the cell on the $i$-th row and $j$-th column. This cell should not have been selected in a previous round. Additionally, if it is not the first turn, the cell must be orthogonally adjacent to at least one previously selected cell.</p><p>If any of your outputs are invalid, the jury will output "<span class="tex-font-style-tt">-1</span>" and you will receive a <span class="tex-font-style-bf">Wrong Answer</span> verdict.</p><p>At the end of all $n \cdot m$ turns, if the sum of numbers in the cells selected by you is not strictly less than the sum of numbers in the cells selected by the interactor, the jury will output "<span class="tex-font-style-tt">-1</span>" and you will receive a <span class="tex-font-style-bf">Wrong Answer</span> verdict.</p><p>If your program has received a <span class="tex-font-style-bf">Wrong Answer</span> verdict, it must terminate immediately. Otherwise, you may receive an arbitrary verdict because your solution might be reading from a closed stream.</p><p>After outputting, do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">In this problem, hacks are disabled.</span></p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains two integers $n$ and $m$ ($4 \le n, m \le 10$)&nbsp;！ the number of rows and columns in the grid.</p>





```input1
1
4 4




3 4

4 4

4 2

4 1

1 4

1 2

2 2

2 1
```




```output1
2 3 4 10
12 6 11 15
5 13 16 8
9 7 1 14

2 4

4 3

3 3

3 1

1 3

1 1

2 3

3 2
```



## Note

<p>Note that this is an example game and does not necessarily represent the optimal strategy for both players.</p><p>First, we fill a $4 \times 4$ grid with unique integers from $1$ to $16$ in the following way:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$4$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$10$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$12$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$6$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$11$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$15$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$5$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$13$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$16$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$8$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$9$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$7$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$14$</td></tr></tbody></table> </center><p>Next, the game begins.</p><ol> <li> The interactor first selects $(3, 4)$, which is the number $8$. For this selection, the interactor could choose any number. From the next selection onwards, each chosen number has to be adjacent to any previously selected number. </li><li> We select $(2, 4)$, which is the number $15$, adjacent to $(3, 4)$. </li><li> The interactor selects $(4, 4)$, which is the number $14$, adjacent to $(3, 4)$. </li><li> We select $(4, 3)$, which is the number $1$, adjacent to $(4, 4)$. </li><li> $\ldots$ </li><li> This is continued until all numbers are selected. </li></ol><p>In the end, the numbers we selected were $[15, 1, 16, 5, 4, 2, 11, 13]$, and the numbers selected by the interactor were $[8, 14, 7, 9, 10, 3, 6, 12]$. The sum of the numbers we selected is $67$, which is less than the sum of the numbers selected by the interactor $69$. Therefore, we have won this game.</p>
