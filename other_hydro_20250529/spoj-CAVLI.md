<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/CAVLI/en/">English</a></td> 
<td width="50%"><a href="/problems/CAVLI/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>Mirko found a wooden board and N nails in his attic. Mirko hammered the nails into the board as fast
as possible. The board can be modeled by a coordinate plane and the nails as points in it. No two nails
have the same x or the same y coordinate.</p> <p>
In order to keep having fun, Mirko stole his sister's elastic hair band, spread it over all nails and then let
go.The elastic, naturally, tightened around the nails.</p>
<p>
Mirko then repeats these steps while there are at least three nails in the board:
</p><ul>
<li>1. Write down the area of the shape enclosed by the hair band.
</li><li>2. Picks the leftmost, rightmost, topmost or bottommost nail in the board.
</li><li>3. Remove the chosen nail from the board; the elastic tightens again around the remaining nails.
</li></ul>
Write a program that calculates the numbers written in step 1 of each iteration,if we know the nail Mirko picks in step 2 of each iteration.
<h3>Input</h3>
<p>The first line contains the integer N (3 ¡Ü N ¡Ü 300 000), the number of nails.</p> <p>
Each of the following N lines contains two integers separated by a space, the coordinates of a nail. All
coordinates will be between 1 and 1 000 000 000. No two nails will share the same x or y coordinate.</p> <p>
The next line contains N-2 letters 'L', 'R', 'U' or 'D'. The letters represent the nails Mirko picked in
order:
</p><ul>
<li> 'L' for the leftmost nail (smallest x coordinate),
</li><li> 'R' for the rightmost nail (largest x coordinate),
</li><li> 'U' for the topmost nail (largest y coordinate),
</li><li> 'D' for the bottommost nail (smallest y coordinate).
</li></ul>
<h3>Output</h3>
<p>
Output N-2 numbers, each on a separate line. The numbers are, in order, the areas that Mirko wrote
down. Output numbers with one digit after the decimal point.

</p><h3>Example</h3>

<pre><b>Input:</b>
8
1 6
2 4
3 1
4 2
5 7
6 5
7 9
8 3
URDLUU

<b>Output:</b>
34.0
24.0
16.5
14.0
9.5
5.0
</pre>