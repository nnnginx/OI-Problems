<p>Given a directed graph, may contains repeated edges. We assume that the graph contains and only contains K edge-disjoint branchings rooted by node 0.<br>A branching for a graph is a set of directed edges that from a certain root (root, in this problem, is node 0) we can find one path to every other node in the graph by only the edges in the branching.<br>K edge-disjoint branching is K branchings that share no common edges.<br>Your task which is easy and funny is to find out the K branchings.</p>
<h3>Input</h3>
<p>The first line of input contains a single integer T, (T&lt;=20), denoting the number of test cases.<br>For each test case:<br>The first line contains two integers N and K, (2&lt;=N&lt;=500,2&lt;=K&lt;=6), which is the number of the nodes in the graph and the number of edge-disjoint branchings.<br>Then next (N-1)*K lines contains the information about the edges. There are 2 integers X and Y in every line, meaning there exist an edge from X to Y in the graph.</p>
<h3>Output</h3>
<p>You should output the branchings you have found.<br>For every test cases, print the number of test case at the start of output, then you should output K lines.<br>Each line is about a branching which contains N-1 integers that the ID of the edges in this branching.<br>The ID of edges starts with 0. Every edge will appear and only appear once in the output.<br>See samples for further details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>2 2<br>0 1<br>0 1<br>3 2<br>0 1<br>0 2<br>2 1<br>1 2</pre>
<pre><strong>Output:</strong>
Case 1:<br>0<br>1<br>Case 2:<br>0 3<br>1 2</pre>
<p><strong>Test data have been enhanced.</strong></p>