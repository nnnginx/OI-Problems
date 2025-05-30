<p>One of the secret chambers in Hogwarts is full of philosopher��s stones. The floor of the chamber is covered by h �� w square tiles, where there are h rows of tiles from front (first row) to back (last row) and w columns of tiles from left to right. Each tile has 1 to 100 stones on it.

Harry has to grab as many philosopher��s stones as possible, subject to the following restrictions:
</p><ul><li>He starts by choosing any tile in the first row, and collects the philosopher��s stones on that tile. Then, he moves to a tile in the next row, collects the philosopher��s stones on the tile, and so on until he reaches the last row.</li>
<li>
When he moves from one tile to a tile in the next row, he can only move to the tile just below it or diagonally to the left or right.</li></ul>

Given the values of h and w, and the number of philosopher��s stones on each tile, write a program to compute the maximum possible number of philosopher��s stones Harry can grab in one single trip from the first row to the last row.

<h3>Input</h3>
<p>The first line consists of a single integer T, the number of test cases. In each of the test cases, the first line has two integers. The first integer h (1 &lt;= h &lt;= 100) is the number of rows of tiles on the floor. The second integer w (1 &lt;= w &lt;= 100) is the number of columns of tiles on the floor.
Next, there are h lines of inputs. The i-th line of these, specifies the number of philosopher��s stones in each tile of the i-th row from the front. Each line has w integers, where each integer m (0 &lt;= m &lt;= 100) is the number of philosopher��s stones on that tile. The integers are separated by a space character.
</p><h3>Output</h3>
<p>The output should consist of T lines, (1 &lt;= T &lt;= 100), one for each test case. Each line consists of a single integer, which is the maximum possible number of philosopher��s stones Harry can grab, in one single trip from the first row to the last row for the corresponding test case.
</p><h3>Example</h3>

<pre><b>Input:</b>
1
6 5
3 1 7 4 2
2 1 3 1 1
1 2 2 1 8
2 2 1 5 3
2 1 4 4 4
5 2 7 5 1

<b>Output:</b>
32 	

//7+1+8+5+4+7=32
</pre>