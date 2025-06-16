<p>Given an undirected weighted graph {<i>V</i>,<i>E</i>}. Your task to calculate the importance of each node.</p>
<p>The importance of a node <i>v</i> (I(v)) can be defined as follow:</p>
<img src="/content/john_jones:import1.jpg">
<p>C<sub>s,t</sub> is the number of different shortest paths from s to t, C<sub>s,t</sub>(v) is the number of different shortest paths from s to t through v.</p>

<h3>Input</h3>
<p>Multiple test cases, the number of them is given in the very first line. </p>
<p>For each test case: </p>
<p>The first line contains two space-separated integers n(n&lt;=100) and m(m&lt;=4500), the number of nodes in the graph and the number of edges in the graph. The nodes are numbered from 1 to n. m lines follow, each contains 3 integers a, b, c, 1&lt;=a, b&lt;=n, 1&lt;=c&lt;=1000, a!=b, which denotes that there is an undirected edge between node a and node b weighted c. You may assume that there is at most one edge between any pair of nodes, and the number of shortest paths between any pair of nodes is at least 1 and at most 10<sup>10</sup>. </p>

<h3>Output</h3>
<p>For each test case: </p>
<p>Your Output should contains n lines, each contains one single real number, with 3 decimal places after radix point. The number in the <i>i</i>th line denotes the importance of the <i>i</i>th node. </p>

<h3>Example</h3>
<pre><b>Input:</b>
1
4 4
1 2 1
2 3 1
3 4 1
4 1 1

<b>Output:</b>
1.000
1.000
1.000
1.000
</pre>