<p>You are given a tree (an acyclic undirected connected graph) with <b>N</b> nodes, and edges numbered 1, 2, 3...<b>N</b>-1.
</p><p>We will ask you to perfrom some instructions of the following form:</p>
<ul>
<li><b>CHANGE i ti</b> : change the cost of the i-th edge to ti<br>
or
</li><li><b>QUERY a b</b> : ask for the maximum edge cost on the path from node a to node b
</li></ul>

<h3>Input</h3>
<p>The first line of input contains an integer <b>t</b>, the number of test cases (<b>t</b> &lt;= 20). t test cases follow.
</p><p>For each test case:</p> 
<ul>
<li>In the first line there is an integer <b>N</b> (<b>N</b> &lt;= 10000),
</li><li>In the next <b>N</b>-1 lines, the i-th line describes the i-th edge: a line with three integers <b>a b c</b> denotes an edge between <b>a</b>, <b>b</b> of cost <b>c</b> (<b>c</b> &lt;= 1000000),
</li><li>The next lines contain instructions <b>"CHANGE i ti"</b> or <b>"QUERY a b"</b>,
</li><li>The end of each test case is signified by the string "<b>DONE</b>".
</li></ul>
<p>There is one blank line between successive tests.

</p><h3>Output</h3>
<p>For each "<b>QUERY</b>" operation, write one integer representing its result.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1

3
1 2 1
2 3 2
QUERY 1 2
CHANGE 1 3
QUERY 1 2
DONE

<b>Output:</b>
1
3
</pre>