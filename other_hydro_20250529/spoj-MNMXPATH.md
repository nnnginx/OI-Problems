<p>I have been asked to set a problem by spoj, what do I do now ? Lets see the standard stuff in most of the programming contests and make one problem out of it. Hmm... many problems are having Binary digits, Grids, Paths, Coins, Maximize or Minimize something, so let me mix them all now in to one problem, the one problem to rule them all ;) <br><br> Lets have a grid of size <strong>N</strong> x <strong>M</strong> having N rows and M columns, and put gold coins in it. How many in each cell ? , lets involve binary here. I'll give you two binary strings <strong>A</strong>[1...N] and <strong>B</strong>[1...M]. Cell (i,j) (1-based indexing) Row-i and Column-j in the grid contains A[i] * B[j] gold coins. From a cell (i,j), you can move to any of the 4 adjacent cells (i-1,j), (i+1,j), (i,j-1), (i,j+1) in one step. I want a path of <em>minimum length</em> from top-left cell (1,1) to bottom-right cell (N,M), and the value of this path = number of gold coins it covers. Find the maximum value of such a path. Not every one wants to become a Raja, also find the minimum value of such a path.</p>
<h3>Input</h3>
<p>First line contains T [ number of test cases, around 10 ]. T cases follow, each having 2 lines, "N A" and "M B" (quotes for clarity only). [ 1 &lt;= N,M &lt;= 100,000 and each character in A, B is either 0 or 1 ]</p>
<h3>Output</h3>
<p>For each test case, print the maximum value of a path followed by the minimum value of a path, in the same line, separated by a single space. Output of each case should be in a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>4 1001<br>3 110<br>5 01111<br>3 110<br><br><strong>Output:</strong><br>3 1<br>5 0<br><br><strong>Explanation:</strong><br>Case 1 : A Maximum path in bold<br><table border="0">
<tbody><tr><td><strong>1</strong></td><td><strong>1</strong></td><td>0</td></tr>
<tr><td>0</td><td><strong>0</strong></td><td>0</td></tr>
<tr><td>0</td><td><strong>0</strong></td><td>0</td></tr>
<tr><td>1</td><td><strong>1</strong></td><td><strong>0</strong></td></tr>
</tbody></table><br>Case 1 : A Minimum path in bold<br><table border="0">
<tbody><tr><td><strong>1</strong></td><td>1</td><td>0</td></tr>
<tr><td><strong>0</strong></td><td><strong>0</strong></td><td>0</td></tr>
<tr><td>0</td><td><strong>0</strong></td><td><strong>0</strong></td></tr>
<tr><td>1</td><td>1</td><td><strong>0</strong></td></tr>
</tbody></table><br></pre>