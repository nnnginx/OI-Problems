<p>
You are given a tree (an undirected acyclic connected graph) with <b>N</b> nodes, and edges numbered 1, 2, 3...<b>N</b>-1. Each edge has an integer value assigned to it, representing its length.
</p>
<p>
We will ask you to perfrom some instructions of the following form:
</p>

<ul>
<li><b>DIST a b</b> : ask for the distance between node <b>a</b> and node <b>b</b><br>
or
</li><li><b>KTH a b k</b> : ask for the <b>k</b>-th node on the path from node <b>a</b> to node <b>b</b> 
</li></ul>

<p>
<b>Example:</b><br>
<b>N</b> = 6 <br>
1 2 1 // edge connects node 1 and node 2 has cost 1 <br>
2 4 1 <br>
2 5 2 <br>
1 3 1 <br>
3 6 2 <br>
<br>
Path from node 4 to node 6 is 4 -&gt; 2 -&gt; 1 -&gt; 3 -&gt; 6 <br>
<b>DIST 4 6</b> : answer is 5 (1 + 1 + 1 + 2 = 5) <br>
<b>KTH 4 6 4</b> : answer is 3 (the 4-th node on the path from node 4 to node 6 is 3) <br>
</p>

<h3>Input</h3>
<p>
The first line of input contains an integer <b>t</b>, the number of test cases (<b>t</b> &lt;= 25). <b>t</b> test cases follow.
</p><p>For each test case:</p> 
<ul>
<li>In the first line there is an integer <b>N</b> (<b>N</b> &lt;= 10000)
</li><li>In the next <b>N</b>-1 lines, the i-th line describes the i-th edge: a line with three integers <b>a b c</b> denotes an edge between <b>a</b>, <b>b</b> of cost <b>c</b> (<b>c</b> &lt;= 100000)
</li><li>The next lines contain instructions <b>"DIST a b"</b> or <b>"KTH a b k"</b>
</li><li>The end of each test case is signified by the string "<b>DONE</b>".
</li></ul>
<p>There is one blank line between successive tests.
</p>

<h3>Output</h3>
<p>For each <b>"DIST"</b> or <b>"KTH"</b> operation, write one integer representing its result.</p>
<p>Print one blank line after each test.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
1

6
1 2 1
2 4 1
2 5 2
1 3 1
3 6 2
DIST 4 6
KTH 4 6 4
DONE

<b>Output:</b>
5
3
</pre>