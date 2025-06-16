<p>A ninja is practicing and he is very fast he can make two cuts in one second and his master give he a new challenge. The master take a cube, thrown through the air and quickly says four numbers. The ninja has to think fast to make two cuts and get desired values.<br><br>
Given a cube of size N*N*N, he need to cut it into four entire pieces of size A, B, C and D. He needs to divide the cube in these pieces with only two cuts, one vertical and one horizontal.<br><br>
</p><h3>Input</h3>
<p>The input consists in multiple test cases.<br>
Each test case begins a line containing five integers N (2 &lt;= N &lt;= 1000000), A, B, C y D (1 &lt;= A, B, C, D &lt;= 2^63).<br>
The end of input is indicated by a line with five zeros. This is not a part of any test cases.<br>
</p><h3>Output</h3>
<p>For each test case print "Possible" if it is possible to obtain the pieces and print "Impossible" if it is not possible to obtain the pieces with two cuts.<br><br>
</p><h3>Example</h3>
<pre><b>Input:</b>
2 5 1 1 1
2 2 2 2 2
3 12 3 6 6
0 0 0 0 0

<b>Output:</b>
Impossible
Possible
Possible

</pre>