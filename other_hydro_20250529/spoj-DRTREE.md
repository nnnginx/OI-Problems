<p>
You are given a rooted tree with N nodes, numbered from 1 to N. Initially node 1 is the root. Each node i has a weight W[i]. You have to perform two types of operations: 
<br>
<b>"S a"</b> - Find the sum of weights of node <b>a</b>'s sub-tree nodes (including node <b>a</b>).
<br>
<b>"R a"</b> - Change root of the tree to <b>a</b>.
</p>

<h3>Input</h3>

<p>
<b>Line 1:</b> N (1 &lt;= N &lt;= 10<sup>5</sup>), number of nodes.
<br>
<b>Line 2:</b> N space-separated integers, weights of nodes from 1 to N. <b>i</b>'th integer is W[i] (1 &lt;= W[i] &lt;= 10<sup>9</sup>).
<br>
<b>Line 3:</b> N-1 space-separated integers, <b>i</b>'th integer is the parent of node <b>i+1</b>.
<br>
<b>Line 4:</b> Q, the number of operations (1 &lt;= Q &lt;= 10<sup>5</sup>).
<br>
<b>Lines 5 .. 5+Q-1:</b> Every line contains a space separated character and an integer. Character describes the type of the operation, and integer is the node number.
</p>

<h3>Output</h3>

<p>
For each operation of type 'S', output the operations result in a separate line.
</p>

<h3>Example</h3>

<pre><b><u>Input:</u></b>
5
2 1 1 1 2
1 1 2 2
3
S 2
R 2
S 1

<b><u>Output:</u></b>
4
3
</pre>