<p>You are given a tree with&nbsp;<strong>N</strong>&nbsp;nodes.  
The tree nodes are numbered from&nbsp;<strong>1</strong>&nbsp;to&nbsp;<strong>N</strong>.  
Each node has an integer weight.</p>

<p>We will ask you to perform the following operation:</p>
<ul>
  <li><strong>u v</strong>&nbsp;: ask for how many different integers that represent the weight of nodes there are on the path from <strong>u</strong> to <strong>v</strong>.</li>
</ul>

<h3>Input</h3>

<p>In the first line there are two integers&nbsp;<strong>N</strong>&nbsp;and&nbsp;<strong>M</strong>. (<strong>N</strong> &lt;= 40000, <strong>M</strong> &lt;= 100000)</p>
<p>In the second line there are&nbsp;<strong>N</strong>&nbsp;integers. The i-th integer denotes the weight of the i-th node.</p>
<p>In the next&nbsp;<strong>N-1</strong>&nbsp;lines, each line contains two integers&nbsp;<strong>u</strong>&nbsp;<strong>v</strong>, which describes an edge (<strong>u</strong>, <strong>v</strong>).</p>
<p>In the next&nbsp;<strong>M</strong>&nbsp;lines, each line contains two integers&nbsp;<strong>u</strong>&nbsp;<strong>v</strong>, which means an operation asking for&nbsp;how many different integers that represent the weight of nodes there are on the path from&nbsp;<strong>u</strong>&nbsp;to&nbsp;<strong>v</strong>.</p>

<h3>Output</h3>
<p>For each operation, print its result.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
8 2
105 2 9 3 8 5 7 7
1 2
1 3
1 4
3 5
3 6
3 7
4 8
2 5
7 8</pre>

<pre><strong>Output:</strong>
4
4</pre>