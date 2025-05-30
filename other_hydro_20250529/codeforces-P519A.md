## Description

<div><p><span class="tex-font-style-it">A and B are preparing themselves for programming contests.</span></p><p>To train their logical thinking and solve problems better, A and B decided to play chess. During the game A wondered whose position is now stronger.</p><p>For each chess piece we know its weight: </p><ul> <li> the queen's weight is 9, </li><li> the rook's weight is 5, </li><li> the bishop's weight is 3, </li><li> the knight's weight is 3, </li><li> the pawn's weight is 1, </li><li> the king's weight isn't considered in evaluating position. </li></ul><p>The player's weight equals to the sum of weights of all his pieces on the board.</p><p>As A doesn't like counting, he asked you to help him determine which player has the larger position weight.</p></div><div class="input-specification"><p>The input contains eight lines, eight characters each ！ the board's description.</p><p>The white pieces on the board are marked with uppercase letters, the black pieces are marked with lowercase letters.</p><p>The white pieces are denoted as follows: the queen is represented is '<span class="tex-font-style-tt">Q</span>', the rook ！ as '<span class="tex-font-style-tt">R</span>', the bishop ！ as'<span class="tex-font-style-tt">B</span>', the knight ！ as '<span class="tex-font-style-tt">N</span>', the pawn ！ as '<span class="tex-font-style-tt">P</span>', the king ！ as '<span class="tex-font-style-tt">K</span>'.</p><p>The black pieces are denoted as '<span class="tex-font-style-tt">q</span>', '<span class="tex-font-style-tt">r</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">n</span>', '<span class="tex-font-style-tt">p</span>', '<span class="tex-font-style-tt">k</span>', respectively.</p><p>An empty square of the board is marked as '<span class="tex-font-style-tt">.</span>' (a dot). </p><p>It is <span class="tex-font-style-bf">not guaranteed</span> that the given chess position can be achieved in a real game. Specifically, there can be an arbitrary (possibly zero) number pieces of each type, the king may be under attack and so on.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">White</span>" (without quotes) if the weight of the position of the white pieces is more than the weight of the position of the black pieces, print "<span class="tex-font-style-tt">Black</span>" if the weight of the black pieces is more than the weight of the white pieces and print "<span class="tex-font-style-tt">Draw</span>" if the weights of the white and black pieces are equal.</p></div>


## Input

<p>The input contains eight lines, eight characters each ！ the board's description.</p><p>The white pieces on the board are marked with uppercase letters, the black pieces are marked with lowercase letters.</p><p>The white pieces are denoted as follows: the queen is represented is '<span class="tex-font-style-tt">Q</span>', the rook ！ as '<span class="tex-font-style-tt">R</span>', the bishop ！ as'<span class="tex-font-style-tt">B</span>', the knight ！ as '<span class="tex-font-style-tt">N</span>', the pawn ！ as '<span class="tex-font-style-tt">P</span>', the king ！ as '<span class="tex-font-style-tt">K</span>'.</p><p>The black pieces are denoted as '<span class="tex-font-style-tt">q</span>', '<span class="tex-font-style-tt">r</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">n</span>', '<span class="tex-font-style-tt">p</span>', '<span class="tex-font-style-tt">k</span>', respectively.</p><p>An empty square of the board is marked as '<span class="tex-font-style-tt">.</span>' (a dot). </p><p>It is <span class="tex-font-style-bf">not guaranteed</span> that the given chess position can be achieved in a real game. Specifically, there can be an arbitrary (possibly zero) number pieces of each type, the king may be under attack and so on.</p>


## Output

<p>Print "<span class="tex-font-style-tt">White</span>" (without quotes) if the weight of the position of the white pieces is more than the weight of the position of the black pieces, print "<span class="tex-font-style-tt">Black</span>" if the weight of the black pieces is more than the weight of the white pieces and print "<span class="tex-font-style-tt">Draw</span>" if the weights of the white and black pieces are equal.</p>


## Samples

```input1
...QK...
........
........
........
........
........
........
...rk...

```

```output1
White

```






```input2
rnbqkbnr
pppppppp
........
........
........
........
PPPPPPPP
RNBQKBNR

```

```output2
Draw

```






```input3
rppppppr
...k....
........
........
........
........
K...Q...
........

```

```output3
Black

```




## Note

<p>In the first test sample the weight of the position of the white pieces equals to 9, the weight of the position of the black pieces equals 5.</p><p>In the second test sample the weights of the positions of the black and the white pieces are equal to 39.</p><p>In the third test sample the weight of the position of the white pieces equals to 9, the weight of the position of the black pieces equals to 16.</p>

