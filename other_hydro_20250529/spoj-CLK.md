<p> In Martin Gardner's book «Mathematical Games» the game of «Chomp!» is described as follows. 
<br><br>
For the game of «Chomp!» you need some pieces which are initially placed on a rectangular playing field and removed from it during the game. (If you are playing on paper then you can use a grid with zeros and cross them out during the game instead.) The game is played by 2 players, and moves are made in turns.
<br><br>
Each turn is played as follows. The player chooses one piece, and removes all pieces which lie in the top-right rectangle, i.e., the rectangle having the chosen piece as the bottom-left corner. Thus, turn by turn, the players bite off pieces of the rectangular cookie, biting into it from the north-east (and the game takes its name from the chomp of their jaws). The winner is the player who forces his/her opponent to chomp the last, poisoned piece in the bottom left corner of the initial field.
<br><br>
</p><center><img src="/ZEL08/content/Click.gif" alt="Game Chomp"><br><i>Fig 1. Example of one particular game in "Chomp!". In the initial state the pieces make up a 5х6 rectangle</i></center>
<br>
<p>Those are the rules. And now imagine the following situation. Two players begin to play the game of «Chomp!» on a 10x10 rectangular field. You can see an intermediate position which was obtained after some turn. The opponents are thinking deeply. How the game will end is not clear, because it's humans who are playing, not computers… By the way, talking of computers: write a program, which for the given position output its outcome. Is the player whose turn it is to move able to win, even if his/her opponent uses the best possible strategy?

</p><h3>Input</h3>
<p>The first line of input contains the total number of tests M, followed by M lines, with ten numbers on each of them (describing a single position on the playing field). These ten numbers are separated by spaces and describe the number of pieces in each column (columns are enumerated from left to right).

</p><h3>Output</h3>
<p>You must output exactly M lines, containing the letter W if it is possible for the player who takes the next turn to win (even in case of the best possible strategy for the other player), or L otherwise.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
2 2 0 0 0 0 0 0 0 0
2 1 0 0 0 0 0 0 0 0
10 10 10 10 10 10 10 10 10 10

<b>Output:</b>
W
L
W
</pre>
<h3>Problem author: Filimonenkov D.O.</h3>