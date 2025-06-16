<p><img title="KNIGHTS level C3" src="./23067/file/9VzyLaH9.png" alt="" width="160" height="161"></p>
<p>The image above is an example of a level in Arzola's videogame 'KNIGHTS'. The rules are very simple. The player is given a chess board, where each square is either empty, contains a wall, or contains a knight of one of three colours. Some squares are also marked with a colour - the player beats the level if all marked squares contain a knight of their respective colour at the same time. To accomplish this, the player can select any knight and place him on an empty square using the classic chess knight move (2 squares in one direction, 1 square in a direction perpendicular to the first).</p>
<p>You will help test a few new level designs for this game. Given a starting configuration and several goal configurations (depicting which squares contain which knight), find the minimum number of moves required to get to those goal configurations.</p>
<h3>Input</h3>
<p>The first line contains two integers <strong>1 ¡Ü r,c &lt; 24</strong>.</p>
<p>The following <strong>r </strong>lines contain <strong>c</strong>&nbsp;characters each, describing the starting configuration of the level. The characters in the grid will be '<em>#'</em>&nbsp;for wall, '<em>.' </em>for an empty square, and 'R', 'B' and 'Y' for a red, blue and yellow knight, respectively. <strong>The number of squares that are not walls will be at most 12.</strong></p>
<p>A blank line follows, followed by a line with an integer <strong>1 ¡Ü q ¡Ü 75,000</strong>&nbsp;- the number of suggested goal configurations for this level. You may assume that <strong>q*r*c ¡Ü 10<sup>6</sup>.</strong></p>
<p><strong>q </strong>descriptions of goal configurations follow, separated by blank lines. Each description will be <strong>r</strong>&nbsp;rows consisting of <strong>c </strong>characters, from the same set as the starting configuration. You may assume that the walls are at the same places as in the starting configuration, and that the number of knights of each colour is the same as the number of knights of that colour in the starting configuration.</p>
<h3>Output</h3>
<p>For each suggested goal configuration, if it is not reachable from the starting configuration in any number of moves, output <strong>-1.</strong></p>
<p>Otherwise, output the minimum number of moves required to reach that goal configuration from the starting configuration.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 4
#BYY
..R#
.BYR

4
#BYY
..R#
.BYR

#.YY
..R#
BBYR

#Y.Y
B.R#
.YRB

#..R
YYB#
YBR.

<strong>Output:</strong>
0
1
19
-1

</pre>