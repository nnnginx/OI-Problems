<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/LAZYCOWS/en/">English</a></td>
<td width="50%"><a href="/problems/LAZYCOWS/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Farmer John regrets having applied high-grade fertilizer to his pastures since the grass now grows so quickly that his cows no longer need to move around when they graze. As a result, the cows have grown quite large and lazy... and winter is approaching.</p>
<p>Farmer John wants to build a set of barns to provide shelter for his immobile cows and believes that he needs to build his barns around the cows based on their current locations since they won't walk to a barn, no matter how close or comfortable.</p>
<p>The cows' grazing pasture is represented by a 2 x B (1 &lt;= B &lt;= 15,000,000) array of cells, some of which contain a cow and some of which are empty.  N (1 &lt;= N &lt;= 1000) cows occupy the cells in this pasture:</p>
<p>&nbsp;</p>
<pre>-------------------------------------------------------
|     | cow |     |     |     | cow | cow | cow | cow |
-------------------------------------------------------
|     | cow | cow | cow |     |     |     |     |     |
-------------------------------------------------------
</pre>
<p>Ever the frugal agrarian, Farmer John would like to build a set of just K (1 &lt;= K &lt;= N) rectangular barns (oriented with walls parallel to the pasture's edges) whose total area covers the minimum possible number of cells.  Each barn covers a rectangular group of cells in their entirety, and no two barns may overlap.  Of course, the barns must cover all of the cells containing cows.</p>
<p>By way of example, in the picture above if K=2 then the optimal solution contains a 2x3 barn and a 1x4 barn and covers a total of 10 units of area.</p>
<h3>Input</h3>
<p>The first line of the input contains integer t representing the number of test cases. Then t cases follow. Each case has the following form:</p>
<ul>
<li> Line 1: Three space-separated integers, N, K, and B. </li>
<li> Lines 2..N+1: Two space-separated integers in the range (1,1) to         (2,B) giving the  coordinates of the cell containing each cow.          No cell contains more than one cow. </li>
</ul>
<h3>Output</h3>
<p>For each test case, output the minimum area required by the K barns in order to cover all of the cows.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
8 2 9
1 2
1 6
1 7
1 8
1 9
2 2
2 3
2 4

<strong>Output:</strong>
10
<p>
<strong>Input details:</strong>
As pictured above.
</p><p>
<strong>Output details:</strong>
As discussed above.
</p></pre>
<p> </p>