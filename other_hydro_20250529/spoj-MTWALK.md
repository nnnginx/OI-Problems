<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MTWALK/en/">English</a></td>
<td width="50%"><a href="/problems/MTWALK/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p>
</p><p>Farmer John and Bessie the cow have embarked on one of those 'active' vacations. They spend entire days walking in the mountains and then, at the end of the day, they tire and return to their vacation cabin.</p>
<p>Since climbing requires a lot of energy and they are already tired, they wish to return to the cabin using a path that has the least difference between its highest and lowest elevations, no matter how long that path is. Help FJ find this easy-to-traverse path.</p>
<p>The map of the mountains is given by an N x N (2 &lt;= N &lt;= 100) matrix of integer elevations (0 &lt;= any elevation &lt;= 110) FJ and Bessie are currently at the upper left position (row 1, column 1) and the cabin is at the lower right (row N, column N). They can travel right, left, toward the top, or toward the bottom of the grid. They can not travel on a diagonal.</p>
<h3>Input</h3>
<ul>
<li>Line 1: The single integer, N </li>
<li>Lines 2..N+1: Each line contains N integers, each of which specifies a square's height. Line 2 contains the first (top) row of the grid; line 3 contains the second row, and so on. The first number on the line corresponds to the first (left) column of the grid, and so on. </li>
</ul>
<h3>Output</h3>
<p>An integer that is the minimal height difference on the optimal path.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
1 1 3 6 8
1 2 2 5 5
4 4 0 3 3
8 0 2 3 4
4 3 0 2 1

<strong>Output:</strong>
2
</pre>