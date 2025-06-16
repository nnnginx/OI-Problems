<p>Duck is a young boy who likes to explore the world. Recently, he found an underground place on the Internet and plans to visit. But it is not an easy task because he will have to excavate a tunnel which is a very physical work. Whenever Duck moves one unit, his energy is reduced by one unit, so the exploration cost is increased by one. Luckily, there may be exactly one (or no) existing tunnel or underground space, in this case, Duck can move inside that region without excavating, hence no exploration cost is increased.</p>
<p>You are give an underground map, which is represented as a matrix of <strong>N</strong> rows and <strong>M</strong> columns. The matrix consisting of '<strong>#</strong>' (Rock, visit to there requiring excavation and increase 1 cost), '<strong>.</strong>' (existing tunnel or space, move between them without increasing cost), '<strong>S</strong>' (Starting point), and '<strong>F</strong>' (Destination). For example, from # to # / # to . / . to # / S to . / S to # / . to F / # to F / S to F will increase 1 unit of cost, only from . to . will increase no cost.</p>
<p>Given the maximum cost <strong>D</strong>, You task is divided into two parts: 1. Check whether it is possible to reach F from S without spending more than D cost. 2. Output the new map, keep showing 'S' and 'F', and the cells that can be visited within the minimum cost required to reach F (inclusive) are represented by '.', otherwises '#'. Because Duck is not allowed to pass through F, in some cases, it is impossible to get to some cells. Those cells will be represented by '#' as well. Initially, the exploration cost at S is 0, and Duck can only move in four directions (Up, Down, Left, Right), no diagonal move is allowed.</p>
<h3>Input</h3>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line is the number of test cases T. (1 &lt;= T &lt;= 40)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each test case, it starts with three integers N (Number of rows), M (Number of columns), D (Maximum cost). (1 &lt;= N, M &lt;= 200 / 0 &lt;= D &lt;= M + N)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The following N lines, each line consisting of M characters, including S, F, either # or . or both, representing the map.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">It is guaranteed that no two separated tunnels allowed (that is at most one or none), and N and M will not both equal 1.</div>
<p>The first line is the number of test cases <strong>T</strong>. (1 ¡Ü&nbsp;T ¡Ü&nbsp;40)</p>
<p>For each test case, it starts with three integers <strong>N</strong> (Number of rows), <strong>M</strong> (Number of columns), <strong>D</strong> (Maximum cost Duck can spend). (1 ¡Ü&nbsp;N, M ¡Ü&nbsp;200, 0 ¡Ü&nbsp;D ¡Ü&nbsp;M + N)</p>
<p>The following N lines, each line consisting of M characters, either&nbsp;<strong>S</strong>, <strong>F</strong>, <strong>#</strong> or <strong>.</strong>&nbsp;, representing the map.</p>
<p>It is guaranteed that no two separated tunnels allowed (at most one, all '.' cells are connected with at least one adjacent edge, or no '.' exists at all), and N and M will not both equal 1.</p>
<h3>Output</h3>
<p>For each test case, in the first line, output the word POSSIBLE or IMPOSSIBLE indicating if it is possible to reach F from S within D cost (inclusive).</p>
<p>Then, output N lines containing M characters (S, F, #, .) representing the new map, indicating which cells can be visited without exceeding the minimum cost required to reach F, which not necessarily equal D.</p>
<p>Print a blank line after each test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3

8 8 8
########
#####S##
#.######
#...#..#
###...##
#####.##
########
#####F##

1 10 6
S####.F###

6 9 4
#########
#S###...#
#######.#
##.......
#########
######F##


<strong>Output:</strong>
POSSIBLE
#.......
.....S..
........
........
........
#.......
###....#
#####F##

POSSIBLE
S.....F###

IMPOSSIBLE
.........
.S.......
.........
.........
.........
......F..

</pre>
<h3>Explanation</h3>
<p>In case 1, the cost matrix is:<br><span style="font-size: xx-small;"> 54432123<br> 43321012<br> 32332123<br> 32223223<br> 43322234<br> 54433234<br> 65544345<br> 76655456</span><br>We can see that the minimum cost required to reach F from S is 4, which is less than 8, so output POSSIBLE.<br>For the new map, we keep the S and F, and those cells with minimum cost less than or equal to 4 is represented by '.', otherwise '#'.&nbsp;</p>
<p>In case 2, the cost matrix is <span style="font-size: xx-small;">0123456-1-1-1</span>, because we cannot pass through F, but it is impossible to reach the three most right cells without passing through F, so the minimum cost for those cells are both -1.&nbsp;</p>
<p>In case 3, the cost matrix is:<br><span style="font-size: xx-small;"> 212344445<br> 101233334<br> 212344434<br> 323333333<br> 434444444<br> 545555555</span><br> The answer is impossible because the minimum cost at F is 5 which is more than 4.<br> However, no cell has minimum cost more than 5, so they are all represented by '.', except S and F.</p>