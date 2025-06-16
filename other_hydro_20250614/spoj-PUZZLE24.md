<p>Daniel likes to play a special board game, called 24 puzzle. 24 puzzle is such a game that there are tiles with the number 1 to 23 in a play board like the follows:</p>
<pre> #  #
######
 ####
 ####
######
 #  #
</pre>
<p>The ��#�� denotes the positions that the tiles may be placed on. There are 24 possible positions in total, so one of them is not occupied with the tile. We denote the empty position by zero.</p>
<p>Daniel could move the tiles adjacent to the empty position to it. In this way Daniel can reorder the number tiles of the game. He plays with this game by setting up a target states initially, and then trying to do some move to achieve the target. Soon he finds that not all target states can be achieved by the move.</p>
<p>He asks for your help, to determine whether he set up an impossible target or not.</p>
<h3>Input</h3>
<p>The first line of input contains an integer denoting the number of test cases.</p>
<p>For each test case, the first line contains 24 integers denoting the initial states of the game board. The numbers  describes the tiles from top to bottom, left to right. And the empty position is indicated by zero. You can assume that the number of each tiles are different, and there must be exactly one empty position. The second line of test case also contains 24 integers denoting the target states.</p>
<h3>Output</h3>
<p>For each test case, if the target is impossible to achieve, output <strong>Y</strong> in a single line, otherwise, output <strong>N</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
3 1 2 0 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
3 0 2 1 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23

<strong>Output:</strong>
N
Y
</pre>