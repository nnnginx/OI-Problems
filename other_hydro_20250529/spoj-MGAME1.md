<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MGAME1/en/">English</a></td> 
<td width="50%"><a href="/problems/MGAME1/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<b>Note : C,S,B are used instead of H,F,I, respectively, in test case. </b>

<pre>Hal and Dave are playing an interesting game on a rectangular 
chess like board consisting of squares arranged in R rows and C columns. 
Here are the rules of the game:
•	There is only one piece on a board alternately moved by the 
players.
•	One move of the piece consists of moving it to an adjacent square
in one of following directions: down, right or diagonally right–down.
•	Some squares on a board are ‘forbidden’, i.e. the piece cannot
enter such squares.
•	A square may contain at most one of the following: a 
hamburger, french fries, ice cream. A player who moves the piece to
a square with a hamburger receives 1 point, with french fries 3 points
and with ice cream 5 points.
•	The game ends when a player who should make a move cannot 
make it (because piece would fall off of board or enter a forbidden 
square in all three directions).
•	If at the end of a game both players have same number of 
points, then the one who cannot make a legal move lost that game.
•	If at the end of a game players have different numbers of 
points, then the player with more points won the game.
•	Both players have 0 points at the beginning of a game. Hal 
makes first move. The initial position of the piece is a square that 
is not forbidden and it does not contain any food.

Since there is a finite number of sequence of moves finishing any 
given game, it can be proved that for any given initial position of 
the piece either Dave or Hal can win no matter how the other player 
plays, i.e. he has a winning strategy.
A board, positions of forbidden squares, positions of squares with 
food and some initial positions are given. Write a program that 
will determine for each given initial position which player has a 
winning strategy.

</pre>
<h3>Input</h3>
<pre>The first line of input file contains two integers R, number of rows
(2 ≤ R ≤ 100) and C, number of columns (2 ≤ C ≤ 100) of a board, 
separated by a space character.
Each of next R lines contains a sequence of C characters representing 
a corresponding row of the board. Forbidden squares are represented 
with ‘#’ character. Squares containing food are represented 
with letters H (hamburger), F (french fries) and I (ice cream). Other 
squares are represented with a dot character (‘.’).
The next line 
contains an integer N, 1 ≤ N ≤ 100, the number of given initial positions 
for which a program should find which player has a winning strategy.
Each of the following N lines contain two integers A (1 ≤ A ≤ R) and 
B (1 ≤ B ≤ C), separated with a space character, which determine a 
row and a column of an initial position of a piece. 
Rows are numbered from up to down with number from 1 to R, and 
columns are numbered from left to right with numbers from 1 to C.
 
</pre>
<h3>Output</h3>
<pre>Output file should contain N lines. The ith line should contain name 
of a player (i.e. DAVE or HAL) having a winning strategy for ith given 
initial position.
</pre>
<h3>Sample</h3>
<pre>GAME.IN

3 4
.H#.
I...
##H.
3
1 1
1 4
2 3

GAME.OUT

HAL
DAVE
HAL

GAME.IN

4 5
.#...
#.#.F
.#..F
.#...
3
3 1
3 3
1 5

GAME.OUT

HAL
HAL
HAL

GAME.IN

5 6
##..#.
..#FH#
..#..#
###...
.....I
4
2 1
5 1
1 4
1 6

GAME.OUT

HAL
HAL
DAVE
DAVE

</pre>