<p>You are given a weighted <acronym title="Directed Acyclic Graph">DAG</acronym>. For each vertex, calculate the sum of the weights of the vertices within its reach (including itself).</p>
<h3>Input</h3>
<p>The first line contains an integer T, denoting the number of test cases.</p>
<p>For each test case, the first line contains two positive integers n and m, denoting the number of vertices and the number of edges in the DAG.</p>
<p>The second line contains n positive integers w<sub>1</sub>..w<sub>n</sub>, denoting the weights of vertices.</p>
<p>The next m lines contain two positive integers u,v, denoting an edge from u to v.</p>
<h3>Output</h3>
<p>For each test case, print a line consisting of n numbers, denoting the sum for each vertex.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>4 3<br>510 713 383 990 <br>4 1<br>4 2<br>2 1<br>4 4<br>450 379 230 520 <br>3 4<br>2 4<br>2 3<br>2 4<br><br><strong>Output:</strong><br>510 1223 383 2213<br>450 1129 750 520<br></pre>
<h3>Constraints</h3>
<p>Input Set 1: numberOfTestCases &lt;= 40, n &lt;= 100, m &lt;= 10000</p>
<p>Input Set 2: numberOfTestCases &lt;= 2, n &lt;= 1000, m &lt;= 500000</p>
<p>Input Set 3: numberOfTestCases &lt;= 2, n &lt;= 20000, m &lt;= 500000</p>
<p>The weights are no more than 1000</p>