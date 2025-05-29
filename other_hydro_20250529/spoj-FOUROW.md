<p><img style="float:left; margin-right:30px; margin-bottom:8px; margin-top:2px; margin-left:5px" src="../../../content/numerix:fourow-360.png" alt="Four in a row" width="240" height="220"></p>
<p>You probably know the popular two-players game "Four in a row". Each player gets 21 chips of the same color at the beginning. Then the two players take turns in putting a chip into one of seven slots (each one six cells in height), trying to get at least four of their chips "in a row", i.e. horizontally, vertically or diagonally.<br> Given a series of moves, your task is to first check, if this is a valid game. A game is <em>invalid</em>, if one or more moves are made after a player has already won the game or if more than six chips are put into a single slot. If a game is valid, check if the game is over. A game is over, if one of the players got at least four chips "in a row" with his last move (i.e. he is the winner of the game) or if all slots are filled. If a game is over, check if there is a winner and if so, who it is. If there is a winner, then print the final state of the game.<br> The picture shows the final state of a game, won by the first player (yellow chips).</p>
<h3>Input</h3>
<p>Input starts with a positive integer t&lt;100 in a single line, then t testcases follow. Every testcase starts with "Game #n: ", where n is the number of the game, numbered from 1 to t. Then the description of a game follows, given as a series of digits 1 to 7 indicating the number of the slot (as noted in the picture), in which the player puts his chip. The players are taking turns and the number of moves (i.e. the number of chips put into the slots) will be at most 42.</p>
<h3>Output</h3>
<p>For each testcase print exactly one of the following five lines, where n has to be replaced by the game's number:<br> Game #n is invalid.<br> Game #n is over. There is no winner.<br> Game #n is over. The first player won.<br> Game #n is over. The second player won.<br> Game #n is not over, yet.</p>
<p>If there is a winner, you also have to print a snapshot of the game's final state. A game's state consists of at most six lines representing the (horizontal) rows of the game's grid plus a leading and a trailing line containing seven hyphens.  Every line has a length of exactly seven characters. Use "x" for the chips of the first player, "o" for  those of the second player, whitespaces for all cells without a chip. If a (horizontal) row contains only whitespaces, it must not be printed.</p>
<p>To make it easier to find the winning row in the grid, <em>all</em> chips that belong to the winning  row(s) have to be marked either by "X" (instead of "x", if the first player has won) or by "O" (instead of "o", if the second player has won). Be aware that there can be more than four chips in a winning row and more than one winning row!</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
Game #1: 2143563445575
Game #2: 123456

<strong>Output:</strong>
Game #1 is over. The first player won.
-------
    X  
   Xx  
  Xoo  
oXoxxoo
-------
Game #2 is not over, yet.

</pre>