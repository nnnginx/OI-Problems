<p>Roger was having fun solving his problems until he found this one.&nbsp;As you know, an undirected connected graph with <strong>N</strong> nodes and <strong>N-1</strong> edges is called a tree.&nbsp;You are given an integer <strong>'K'</strong> and a tree consisting of <strong>'N'</strong> nodes. Each node <strong>'i'</strong> has a value <strong>a(i)</strong> associated with it.</p>
<p>We call a path <strong>'P'</strong> of tree valid if following conditions are satisfied:</p>
<ul>
<li><strong>P</strong>&nbsp;has at least 2 nodes associated with it.</li>
<li><strong>Max a(u) - Min a(u) &gt;= K</strong> (u belongs to the nodes present in the choosen P).</li>
</ul>
<p>Your task is to count the number of Valid Paths.</p>
<h3>Input</h3>
<p>The first line contains two space-separated integers<strong> N</strong> and <strong>K</strong>.</p>
<p>The second line contains <strong>N</strong> space-separated positive integers <strong>a(1), a(2), ..., a(n).</strong></p>
<p>Then the next <strong>n - 1</strong> line each contains a pair of integers <strong>u</strong> and <strong>v</strong> denoting that there is an edge between u and v.</p>
<h3>Output</h3>
<p>Print the number of Valid Paths.</p>
<h3>Example</h3>
<pre><strong>SAMPLE INPUT</strong>
3 1
1 2 3
1 2
2 3

<strong>SAMPLE OUTPUT</strong>
3</pre>
<h3>CONSTRAINTS</h3>
<p>1 &lt;= N &lt;= 5000<br> 1 &lt;= u,v &lt;= N<br> 0 &lt;= K &lt;= 10^9<br> 0 &lt;=  ai &lt;= 10^9</p>
<p>&nbsp;</p>
<p>Like Trees? Try the problems: <strong>RTREE</strong>, <strong>RTREE3</strong> as well</p>