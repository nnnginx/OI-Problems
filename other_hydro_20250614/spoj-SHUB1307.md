<p>Its 13th of July and its Shubham Gupta's Birthday. Shubham loves to solve DP problem. Anuj ( Shubham's friend ) want to wish him uniquely. So he decorate their Hostel room no. 235 where the floor is divided into <strong>N x M</strong> square tiles, forming a grid with N rows and M columns.</p>
<p>Each square in the grid contains a number of Vodka Shots that Shubham has to drink if he steps on a particular tile. Shubham enters the room on (1, 1)  and has to makes his way to the exit gate on (N, M), drinking the vodka on the way. From the current cell, he can move only to the adjacent cell in East, South or South-East direction i.e. from (i, j) to either (i, j+1) , (i+1, j) or (i+1, j+1).</p>
<p>However, his capacity for the Vodka is limited. If he drink more than <strong>K</strong> Shots, he will be out of control ! Help him find a way to drink as any many Shots as he can, without going out of control.</p>
<h3>Input</h3>
<p>The first line contains <strong>T</strong>. <strong>T</strong> testcases follow.<br> First line of each testcase contains 3 space-separated integers, <strong>N, M, K</strong>.<br> Each of the following <strong>N</strong> lines contain <strong>M</strong> space-separated integers, describing the grid.</p>
<h3>Output</h3>
<p>Print the maximum number of Vodka Shots that he can drink without going out of control or "-1" (without the quotes) if it can not be done i.e. if there does not exist such a path. Print the answer to each testcase in a new line. .</p>
<h3>Constraints:</h3>
<p>1¡ÜT¡Ü10<br> 1¡ÜN,M¡Ü100<br> 1¡ÜK¡Ü500<br> 1 ¡Ü Values in the Grid ¡Ü 50</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 3 7
2 3 1
6 1 9
8 2 3
3 4 9
2 3 4 1
6 5 5 3
5 2 3 4
<strong>Output:</strong>
6
-1
</pre>
<h3>Explanation</h3>
<p>In the first testcase, he can move on squares (1,1) , (2,2) and (3,3) to complete his journey with 6 Shots. In the second testcase, every possible path leads to the drinks of more than 9 Shots.</p>