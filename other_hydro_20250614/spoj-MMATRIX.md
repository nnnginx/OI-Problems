<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MMATRIX/en/">English</a></td>
<td width="50%"><a href="/problems/MMATRIX/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<pre>Given an n×n matrix A, whose entries Ai,j are integer numbers ( 0 ≤ i &lt; n,
0 ≤ j &lt; n ). An operation SHIFT at row i ( 0 ≤ i &lt; n ) will move the integers
in the row one position right, and the rightmost integer will wrap around
to the leftmost column.
</pre>
<p><img src="../../../../../content/simes:MMATRIX.png" border="0"></p>
<pre>You can do the SHIFT operation at arbitrary row, and as many times as you like. 
Define Cj=A0,j+A1,j+..+A(n-1),j and M = max {Cj|0&lt;=j &lt; n } . 
Cj is the sum of all number in column ith.
Your job is to minimize M. 
</pre>
<h3>Input</h3>
<pre>The input consists of several test cases. The ﬁrst line of each test case 
contains an integer n. Each of the following n lines contains n integers, 
indicating the matrix A. The input is terminated by a single line with 
an integer −1. You may assume that 1 ≤ n ≤ 7 and |Ai,j| &lt; 10^4.

Sample Input
2
4 6
3 7
3
1 2 3
4 5 6
7 8 9
-1
</pre>
<h3>Output</h3>
<pre> 
For each test case, print a line containing the minimum value of the maximum
of column sums.

Sample output
11
15
</pre>
<p> </p>