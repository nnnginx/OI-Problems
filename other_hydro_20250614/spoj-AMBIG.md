<h3>Input</h3>
<p>The input is a directed (multi)graph.</p>
<p>The first line gives the number of edges M and the number of nodes N (&gt;=2). Then each edge is described by a line of the form "FROM TO LABEL". Nodes (FROM, TO) are numbers in the range 0.. N-1 and labels are also numbers.</p>
<p>All numbers in the input are nonnegative integers &lt;2000.</p>
<h3>Output</h3>
<p>Print "YES" if there are two distinct walks with the same labelling from node 0 to node 1, otherwise print "NO".</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong><br>4 4<br>0 2 0<br>0 3 0<br>2 1 1<br>3 1 2<br><strong><br>Output:</strong><br>NO</pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong><br>10 9<br>0 2 0<br>2 1 0<br>2 3 0<br>3 4 0<br>4 2 0<br>2 5 0<br>5 6 0<br>6 7 0<br>7 8 0<br>8 2 0<br><strong><br>Output:</strong><br>YES</pre>
<p>In this case the shortest labelling that appears on two walks is 0 repeated 10 times.</p>
<p><img src="./21319/file/h9jMXqVB.png" alt="drawing of example 2" width="554" height="165"></p>