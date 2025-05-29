<p>Given a tree and a set of edges <strong>K</strong>, find total number of distinct paths in the tree consisting of all the edges in <strong>K</strong>. Two paths are distinct if the end nodes of the paths are different.  Also, a path like (1-&gt;2-&gt;3) is same as (3-&gt;2-&gt;1).</p>
<p>A path is defined as a series of edges which connect a sequence of vertices which are all distinct.</p>
<h3>Input</h3>
<p>First line denotes the number of test cases <strong>T</strong> (&lt;=100) <br><strong>T</strong> test cases follow. <br>Each Test case is defined as: <br>First line contains <strong>n</strong> (1&lt;=n&lt;=2*10^4) and <strong>k</strong> (&lt;=n-1) which are the number of nodes and size of the edge set, respectively. <br>n-1 lines follow, each defining an edge between pair of nodes <strong>u</strong> and <strong>v</strong>. <br>nodes are numbered 1 to n. <br>A single line consisting of <strong>k</strong> space separated indices (0-based, in order they appear in the input) of edges which are in the set.</p>
<h3>Output</h3>
<p>For each test case, output a single integer denoting the number of  distinct paths in the tree consisting of all the edges in the set.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 <br>2 1 <br>1 2 <br>0 <br>3 1 <br>1 2 <br>2 3 <br>1 <br>7 3 <br>1 6 <br>1 2 <br>1 5 <br>2 4 <br>4 7 <br>2 3 <br>0 5 4

<strong>Output:</strong>
1 <br>2 <br>0
</pre>