## Description

<div><p>Monocarp visited a retro arcade club with arcade cabinets. There got curious about the "Catch the Coin" cabinet.</p><p>The game is pretty simple. The screen represents a coordinate grid such that: </p><ul> <li> the X-axis is directed from left to right; </li><li> the Y-axis is directed from bottom to top; </li><li> the center of the screen has coordinates $(0, 0)$. </li></ul><p>At the beginning of the game, the character is located in the center, and $n$ coins appear on the screen&nbsp;！ the $i$-th coin is at coordinates $(x_i, y_i)$. The coordinates of all coins are different and not equal to $(0, 0)$.</p><p>In one second, Monocarp can move the character in one of eight directions. If the character is at coordinates $(x, y)$, then it can end up at any of the coordinates $(x, y + 1)$, $(x + 1, y + 1)$, $(x + 1, y)$, $(x + 1, y - 1)$, $(x, y - 1)$, $(x - 1, y - 1)$, $(x - 1, y)$, $(x - 1, y + 1)$.</p><p>If the character ends up at the coordinates with a coin, then Monocarp collects that coin.</p><p>After Monocarp makes a move, all coins fall down by $1$, that is, they move from $(x, y)$ to $(x, y - 1)$. You can assume that the game field is infinite in all directions.</p><p>Monocarp wants to collect at least one coin, but cannot decide which coin to go for. Help him determine, for each coin, whether he can collect it.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 500$)&nbsp;！ the number of coins.</p><p>In the $i$-th of the next $n$ lines, two integers $x_i$ and $y_i$ ($-50 \le x_i, y_i \le 50$) are written&nbsp;！ the coordinates of the $i$-th coin. The coordinates of all coins are different. No coin is located at $(0, 0)$.</p></div><div class="output-specification"><p>For each coin, print "<span class="tex-font-style-tt">YES</span>" if Monocarp can collect it. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 500$)&nbsp;！ the number of coins.</p><p>In the $i$-th of the next $n$ lines, two integers $x_i$ and $y_i$ ($-50 \le x_i, y_i \le 50$) are written&nbsp;！ the coordinates of the $i$-th coin. The coordinates of all coins are different. No coin is located at $(0, 0)$.</p>

## Output

<p>For each coin, print "<span class="tex-font-style-tt">YES</span>" if Monocarp can collect it. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1|
5
24 42
-2 -1
-1 -2
0 -50
15 0
```




```output1
YES
YES
NO
NO
YES
```



## Note

<p>Pay attention to the second coin in the example. Monocarp can first move from $(0, 0)$ to $(-1, -1)$. Then the coin falls $1$ down and ends up at $(-2, -2)$. Finally, Monocarp moves to $(-2, -2)$ and collects the coin.</p>
