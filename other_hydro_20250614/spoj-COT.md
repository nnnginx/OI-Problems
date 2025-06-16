<p>You are given a tree with <strong>N</strong> nodes. The tree nodes are numbered from <strong>1</strong> to <strong>N</strong>. Each node has an integer weight.</p>
<p>We will ask you to perform the following operation:</p>
<ul>
  <li><strong>u v k</strong> : ask for the kth minimum weight on the path from node <strong>u</strong> to node <strong>v</strong></li>
</ul>

<h3>Input</h3>
<p>In the first line there are two integers <strong>N</strong> and <strong>M</strong>. (<strong>N, M</strong> &lt;= 100000)</p>
<p>In the second line there are <strong>N</strong> integers. The ith integer denotes the weight of the ith node.</p>
<p>In the next <strong>N-1</strong> lines, each line contains two integers <strong>u</strong> <strong>v</strong>, which describes an edge (<strong>u</strong>, <strong>v</strong>).</p>
<p>In the next <strong>M</strong> lines, each line contains three integers <strong>u</strong> <strong>v</strong> <strong>k</strong>, which means an operation asking for the kth minimum weight on the path from node <strong>u</strong> to node <strong>v</strong>.</p>

<h3>Output</h3>
<p>For each operation, print its result.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
8 5
105 2 9 3 8 5 7 7
1 2
1 3
1 4
3 5
3 6
3 7
4 8<br>2 5 1<br>2 5 2<br>2 5 3<br>2 5 4<br>7 8 2&nbsp;</pre>
<pre><strong>Output:</strong>
2<br>8<br>9<br>105<br>7&nbsp;</pre>