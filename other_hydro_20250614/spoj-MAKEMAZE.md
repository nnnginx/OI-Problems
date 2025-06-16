<p style="text-align: center;">&nbsp;</p>
<p style="text-align: center;">&nbsp;</p>
<p style="text-align: center;"><strong><span style="font-size: medium;">MAZE MAKING</span></strong></p>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: left;"><span style="font-size: small;">There are many algorithms to generate maze. (<a href="http://en.wikipedia.org/wiki/Maze_generation_algorithm">http://en.wikipedia.org/wiki/Maze_generation_algorithm</a>). After generating the maze we¡¯ve to validate whether it¡¯s a valid maze or not. A valid maze has exactly one entry point and exactly one exit point (exactly 2 openings in the edges) and there must be atleast one path from the entry point to exit point.</span></p>
<p style="text-align: center;"><span style="font-size: small;"><img src="../../../content/cegprakash:makemaze.png" alt="" width="300" height="300"></span></p>
<p style="text-align: left;"><span style="font-size: small;">Given a maze, just find whether the maze is "valid" or "invalid".</span></p>
<p style="text-align: left;"><span style="font-size: small;"><br></span></p>
<p style="text-align: left;"><span style="font-size: x-small;"><strong><span style="font-size: small;">Input Specification:</span></strong></span></p>
<p style="text-align: left;"><span style="font-size: small;">The first line consists of an integer t, the number of test cases. Then for each test case, the first line consists of two integers m and n, the number of rows and columns in the maze. Then contains the description of the matrix M of order mxn. M[i][j]=# represents a wall and M[i][j]='.' represents a space.<br></span></p>
<p style="text-align: left;"><span style="font-size: x-small;"><strong><span style="font-size: small;">Output Specification:</span></strong></span></p>
<p style="text-align: left;"><span style="font-size: small;"><strong>&nbsp;</strong>For each test case find whether the maze is "valid" or "invalid".</span></p>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: left;"><span style="font-size: small;"><strong>Input Constraints:</strong></span></p>
<p style="text-align: left;"><span style="font-size: small;"><br></span></p>
<p style="text-align: left;"><span style="font-size: small;">1&lt;=t&lt;=10000</span></p>
<p style="text-align: left;"><span style="font-size: small;">1&lt;=m&lt;=20</span></p>
<p style="text-align: left;"><span style="font-size: small;">1&lt;=n&lt;=20</span></p>
<p style="text-align: left;"><span style="font-size: small;"><br></span></p>
<p style="text-align: left;"><span style="font-size: x-small;"><span style="font-size: small;">Sample Input:</span></span></p>
<pre>6
4 4
####
#...
#.##
#.##
5 5
#.###
#..##
##..#
#.#.#
###.#
1 1
.
5 1
#
#
.
.
#
2 2
#.
.#
3 4
#..#
#.##
#.##
</pre>
<p style="text-align: left;"><span style="font-size: x-small;"><span style="font-size: small;">Sample Output:</span></span></p>
<pre>valid
valid
invalid
valid
invalid
invalid
</pre>