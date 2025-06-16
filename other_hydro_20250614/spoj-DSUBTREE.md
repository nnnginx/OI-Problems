<p>Given an unrooted tree, the subtree is defined as a connected component of the given tree. Two subtrees are considered the same if there exists a map from nodes of one tree to another so that the edges of both trees are corresponding the same pair of nodes after mapping.</p>
<p>Your task is to find out how many distinct subtrees for a given unrooted tree.</p>
<h3>Input</h3>
<p>The input consists of multiple test cases. The first line of input contains an integer denoting the number of test cases.</p>
<p>For each test case, the first line contains one integer <strong>n</strong> denoting the number of nodes of the given tree. (1 &lt;= <strong>n</strong> &lt;= 15)</p>
<p>Then <strong>n</strong>-1 lines follow, each line contains two integers denoting an edge of the tree. The index of the node counts from 1.</p>
<h3>Output</h3>
<p>For each test case, output the number of distinct subtrees for the given tree.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3
1 2
1 3
9
9 4
4 3
1 3
7 4
1 6
5 7
2 4
6 8

<strong>Output:</strong>
Case #1: 3
Case #2: 21
</pre>