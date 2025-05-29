<p>

Read the statement of problem G for the definitions concerning trees.
In the following we define the basic terminology of heaps.
A <b>heap</b> is a tree whose internal nodes have each assigned a <b>priority</b> (a number) such that the priority of each internal node is less than the priority of its parent.
As a consequence, the root has the greatest priority in the tree, which is one of the reasons why heaps can be used for the implementation of priority queues and for sorting.

</p><p>

A binary tree in which each internal node has both a label and a priority, and which is both a binary search tree with respect to the labels and a heap with respect to the priorities, is called a <b>treap</b>.
Your task is, given a set of label-priority-pairs, with unique labels and unique priorities, to construct a treap containing this data.

</p><h3>Input Specification</h3><p>

The input contains several test cases.
Every test case starts with an integer <code>n</code>.
You may assume that <code>1&lt;=n&lt;=50000</code>.
Then follow <code>n</code> pairs of strings and numbers <code>l<sub>1</sub>/p<sub>1</sub>,...,l<sub>n</sub>/p<sub>n</sub></code> denoting the label and priority of each node.
The strings are non-empty and composed of lower-case letters, and the numbers are non-negative integers.
The last test case is followed by a zero.


</p><h3>Output Specification</h3><p>

For each test case output on a single line a treap that contains the specified nodes.
A treap is printed as <code>(&lt;left sub-treap&gt;&lt;label&gt;/&lt;priority&gt;&lt;right sub-treap&gt;)</code>.
The sub-treaps are printed recursively, and omitted if leafs.

</p><h3>Sample Input</h3><p>

</p><pre>7 a/7 b/6 c/5 d/4 e/3 f/2 g/1
7 a/1 b/2 c/3 d/4 e/5 f/6 g/7
7 a/3 b/6 c/4 d/7 e/2 f/5 g/1
0
</pre>

<h3>Sample Output</h3><p>

</p><pre>(a/7(b/6(c/5(d/4(e/3(f/2(g/1)))))))
(((((((a/1)b/2)c/3)d/4)e/5)f/6)g/7)
(((a/3)b/6(c/4))d/7((e/2)f/5(g/1)))
</pre>