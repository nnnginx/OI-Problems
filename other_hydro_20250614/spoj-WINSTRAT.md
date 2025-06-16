<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/WINSTRAT/en/">English</a></td> 
<td width="50%"><a href="/problems/WINSTRAT/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>
A table has n rows labeled by numbers from 0 to n-1 and n columns also labeled by numbers from 0 to n-1. The coordinate of a cell belonging to the ith row and jth column is (i,j). Each cell has a value of 0 or 1. In this table, there are m cells having the value of 0. The remaining cells in the table have the values of 1. Two players play a game by making moves in turn until no more moves can be made. The first player will make the move first. Each player can only make one move at each step. The player who cannot make a move loses and the other player wins the game. A legal move is an action to flip the value (from 0 to 1 or from 1 to 0) of four cells at four corners of a rectangle inside the table which satisfies the following conditions:
</p>
<ul>
<li>the rectangle is has more than 1 row and more than 1 column,</li>
<li>the cell with the highest row-column coordinates among the four cells must have the value of 0.</li>
<li>Given the values of cells in the table, your task is to write a program to help the first player to find a winning strategy so that he will win the game no matter how the other player plays.</li>
</ul>
<h3>Input</h3>
<p>The input file consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.
</p>
<p>
For each data set, the first line contains an integer n (0 &lt; n &lt; 1000) representing the size of the table. The next line contains an integer m (0 &lt; m &lt;100). Each of the next m lines contains two integers x, y (0 ¡Ü x,y &lt; n)  separated by space representing the coordinates of a cell with the value of 0.
</p>
<h3>Output</h3>
<p>
For each data test, write in one line 1 if there exists a winning strategy for the first player with the given table or 0 otherwise.
</p>
<h3>Example</h3>
<pre><b>Sample Input</b>
4
100
1
0 0 
100
3
0 1
0 20
0 30 
100
2
2 3
3 2
10
2
1 2 
2 3	

<b>Sample Output</b>
0
0
0
1
</pre>