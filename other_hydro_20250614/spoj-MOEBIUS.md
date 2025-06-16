<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MOEBIUS/en/">English</a></td> 
<td width="50%"><a href="/problems/MOEBIUS/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>
The game of Moebius is not well known, but there are some fanatics who spend their whole day playing it. In this game, the player is to find the way to clear a pair of squares containing x and z on a Moebius with the minimum cost.
</p>

<p>
A Moebius is made from a rectangular M��N paper, namely ABCD. Each face of this paper consists of a rectangular grid of equivalent squares 1��1 . On both grids, columns are sequentially numbered from 1 to N and rows are sequentially numbered from 1 to M, all starting at A corner. In addition, every square (i, j), located at row i and column j, can contain x, z or nothing (empty square). Taking this paper and giving it a half-twist, then joining the ends together, A with C and B with D, to form a single band, we have a Moebius, which has only one surface, for this game.
</p>

<table width="100%">
<tbody><tr>
<td>
<img src="./23447/file/IwwlfF1H.png">
</td>
<td>
<img src="./23447/file/UGtq1tOn.png">
</td>
</tr>
</tbody></table>

<img src="./23447/file/UMQSJOu4.png">

<p>        
One clearance of a pair of squares containing x and z could be executed only if there is a direct path between two squares through consecutive 4 neighboring empty squares with at most two left or right turns. The intermediate empty squares may locate out of the Moebius. The cost to clear a pair of squares containing x and z is the length of the shortest direct path between two squares. After a clearance, the two original squares containing x and z become empty. The figure above shows two consecutive clearances with the cost of 5 and 8 respectively. 
</p>
<p>
Your task is to write a program to perform one clearance to remove a given pair of squares containing x and z, with the minimum total cost using at most one extra intermediate clearance.
</p>

<br>

<h3>Input</h3>
<p>
The input file consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.
</p>
<p>
For each data test, the first line contains 2 integers M and N (1 &lt;= M, N &lt;= 1000) separated by space. The next two lines contain 3-tuples of the form 'C u v' describing the two squares to remove, where C is either 'F' for the front surface or 'B' for the back surface, u (1 &lt;= u &lt;= M) and v (1 &lt;= v &lt;= N) are integer coordinates on the original rectangular surface.
</p>
<p>
The next M lines describing the front surface of the Moebius. The i-th line in these M lines contains N consecutive characters where each character can be x, z or "." ("." for empty), describing the i-th row of the front surface.
</p>
<p>
The next M lines describing the back surface of the Moebius. The j-th line contains N consecutive characters where each character can be x, z or "." ("." for empty), describing the j-th row of the back surface.
</p>

<br>

<h3>Output</h3>
<p>
For each data test, write in one line the minimum total cost. Write '-1' if the given pair cannot be cleared using at most one intermediate clearance.
</p>

<br>

<h3>Example</h3>
<pre><b>Sample Input</b>

1
3 10
F 2 7
B 2 1
.....xxx.z
.....xzx.x
.....xxx.z
.z........
xz........
zz........	

<b>Sample Output</b>

13
</pre>