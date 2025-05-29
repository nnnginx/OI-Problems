<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MCQUERY/en/">English</a></td> 
<td width="50%"><a href="/problems/MCQUERY/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>You are given a weighted undirected graph with edge weight denoting the capacity of the edge. </p>
<p>Now given a number x, output how many unordered (s,t) pairs are there in the graph such that minCut(s,t) &lt;= x. </p>
<p>A Cut is a partition of the vertices of a graph into two sets such that s and t belong to different set after the partition. </p>
<p>In weighted graphs, the size of a cut is defined to be the sum of weights of the edges crossing the cut. minCut is a cut whose size is the least possible.</p>

<h3>Input</h3>
<p>First line contains T, the number of test cases.</p> <p>For each test case the first line contains two integers n and m, denoting the number of vertices and the number of edges in the graph.</p>
<p> Next m lines contain 3 integers u,v,c denoting an undirected of capacity c between vertices u and v; 1 &lt;= u,v &lt;= n.</p> 
<p>Next line contains q, the number of queries. Next q line contains one number each which denotes the input x for ith query.</p><p>
Note: there can be multiple edges between a pair of vertices. </p>

<h3>Output</h3>
<p>The output for each test case should consist of q lines with one integers in each of them denoting the number of unordered (s,t) pairs corresponding to that query. Output a blank line BETWEEN the test cases.
</p>
<p>Note: The timelimit for the problem is somewhat strict. </p>

<h3>Example</h3>

<pre><b>Input:</b>
1
5 0
1
0

<b>Output:</b>
10
</pre>

<h3>Constraints</h3>
<p>
Input Set 1: numberOfTestCases &lt;= 15, n &lt;= 40, m &lt;= 400, q &lt;= 10 </p>
<p>Input Set 2: numberOfTestCases &lt;= 20, n &lt;= 150, m &lt;= 3000, q &lt;= 30</p>
<p>Edge weights are less than or equal to 10^6
</p>