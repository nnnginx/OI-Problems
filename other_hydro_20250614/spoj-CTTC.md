<p>
Little boy Arik is playing with tree. He is counting the number of children of each node.</p>

<p>
For this, he starts with root node 1. And traverse the full tree in DFS (Depth First Search) style. 
For simplicity, see the following figure.
</p>

<p>For Tree - 1, his traversing sequence is 1 2 2 3 3 1. He starts with root node 1. Then he starts visiting first child 2, then finishes his traversing at 2. Then he starts visiting second child 3, then finishes his traversing at 3. And then finally finishes his traversing at 1.</p>

<p>For Tree - 2, his traversing sequence is 1 2 4 4 2 3 5 5 6 6 3 1. </p>

<h3>Input</h3>
<p>Input starts with an integer t (1 &lt;= t &lt;= 20), which denotes the case numbers. </p>
<p>For each case, you are given n (1 &lt;= n &lt;= 100) in first line. Next line contains 2n integers denoting his sequences of traversing. All nodes are between 1 to n. The root node is always node 1.</p>

<h3>Output</h3>
<p>
For each case print the case number in the first line. Following n lines print each node from 1 to n and number of child of the node. Print a blank line after each test cases. See the sample I/O section for more details about output format.</p>

<h3>Example</h3>
<h4>Input</h4>
<pre>2
3
1 2 2 3 3 1
6
1 2 4 4 2 3 5 5 6 6 3 1</pre>

<h4>Output</h4>
<pre>Case 1:
1 -&gt; 2
2 -&gt; 0
3 -&gt; 0

Case 2:
1 -&gt; 2
2 -&gt; 1
3 -&gt; 2
4 -&gt; 0
5 -&gt; 0
6 -&gt; 0

</pre>