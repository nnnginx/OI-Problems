<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/TABLIC/en/">English</a></td> 
<td width="50%"><a href="/problems/TABLIC/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>Ivo has an N¡ÁN table. The table has the integers 1 through N<sup>2</sup> inscribed in row-major order. The following operations can be done on the table:</p>
<p>1. Rotate a row ¨C all cells in a single row are rotated right, so that the number in the last column moves to the first.</p>
<p>2. Rotate a column ¨C all cells in a single column are rotated down, so that the number in the last
row moves to the first.</p>
<p>Ivo occasionally feels the urge to move a number X to cell (R, C) and proceeds as follows:</p>
<ul>
<li>While X is not in column C, rotate the row it is in.</li>
<li>While X is not in row R, rotate the column it is in.</li>
</ul>
<p>Ivo wants to move K numbers one after another. Write a program that calculates the number of
rotations needed.</p>
<h3>Input</h3>
<p>The first line contains two integers N (2 ¡Ü N ¡Ü 10 000) and K (1 ¡Ü K ¡Ü 1000), the table dimension and
the number of moves.</p>
<p>Each of the following K lines contains three integers X (1 ¡Ü X ¡Ü N<sup>2</sup>), R and C (1 ¡Ü R, C ¡Ü N), the
description of one move Ivo wants to make. Ivo does the moves in the order in which they are given.</p>

<h3>Output</h3>
<p>Output K lines; for each move, output the number of rotations needed.</p>

<h3>Example</h3>

<pre>Input
4 1
6 3 4

Output
3


Input
4 2
6 3 4
6 2 2

Output
3
5


Input
5 3
1 2 2
2 2 2
12 5 5

Output
2
5
3
</pre>