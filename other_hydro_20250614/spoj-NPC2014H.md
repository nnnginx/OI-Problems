<p>There is a matrix with size N x M where each cell contains an integer. An arithmetic rectangle is a rectangle inside the matrix so that each row and column is an arithmetic progression. An arithmetic progression is a sequence so that each number minus the number before it is the same. Given a matrix, find the largest arithmetic rectangle, which is the arithmetic rectangle containing the most number of cells. For example, the largest arithmetic rectangles of the matrix below consists of 9 cells:</p>
<p style="text-align: center;"><img src="../../../content/andypertamax:NPC2014H-matrix" alt="5,3,5,7/2,4,4,4/3,5,3,1/6,3,2,4" width="112" height="112"></p>
<h3>Input</h3>
<p>First line of input is T, the number of test cases. Each test case starts with N and M. The next N lines each containing M integers &nbsp;A<sub>ij</sub>&nbsp;representing the value of each cell of the matrix. Each input file will not exceed 20 MB in size.</p>
<h3>Output</h3>
<p>For each test case output the number of cells in the largest arithmetic rectangle in the matrix.</p>
<h3>Sample Input</h3>
<pre>2
4 4
5 3 5 7
2 4 4 4
3 5 3 1
6 3 2 4
2 3
0 1 2
1 2 3</pre>
<h3>Sample Output</h3>
<pre>9
6</pre>
<div style="border: 1px solid #FC0; background-color: #FFC; padding: 5px; margin-bottom: 10px;">
<h3>Constraint</h3>
<ul>
<li> 1 ¡Ü T ¡Ü 10000</li>
<li> 1 ¡Ü N, M ¡Ü 3000</li>
<li> 0 ¡Ü A<sub>ij</sub> ¡Ü 1000000000</li>
</ul>
</div>
<p><strong>Input file is huge, is faster I/O (scanf for C)</strong></p>