<p>You are given a parent array <strong>P</strong> of length <strong>N</strong> that represents a binary tree with N nodes, which may be unbalanced, balanced, complete or full. The array indexes are values in tree nodes and the array values represent the parent node of that particular index, a value -1 means that particular index is the root of the tree. This gives both left child and right child or only left child, for a parent, right child cannot exist without left child. You are required to count the total number of potential isosceles triangles in the binary tree. A potential isoscele triangle is the two sides of equal length must be formed by two paths of equal length from a parent or root. Due to the nature of binary tree, not three sides are connected, you can just ignore the remaining unconnected side.</p>
<p>Consider a parent array [1, 5, 5, 2, 2, -1, 3], it constructs a binary tree like:&nbsp;</p>
<p><img src="file://V0josmmb.png" alt="" width="262" height="211"></p>
<p>There are 4 potential isosceles triangles in total, they are (1, 5, 2), (0, 5, 4), (3, 2, 4) and (3, 2, 5) respectively.</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>. (1 ¡Ü T ¡Ü 50)</p>
<p>For each test case, it starts with one integer representing the number of nodes or length of the array&nbsp;<strong>N</strong>. (1 ¡Ü N ¡Ü 10<sup>5</sup>)</p>
<p>The next line has N integers, <strong>P<sub>i</sub></strong> is the node's parent node (-1 is the root) and <strong>i</strong> is its value. (-1&nbsp;¡Ü P<sub>i</sub> ¡Ü N - 1)</p>
<h3>Output</h3>
<p>Print the total number of potential isosceles triangles.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3

7
1 5 5 2 2 -1 3

20
-1 0 0 1 1 3 5 4 7 4 8 8 9 10 10 9 15 15 16 16

5
3 0 1 -1 2
</pre>
<pre><strong>Output:</strong>
4
20
0
</pre>
<h3>Explanation</h3>
<p>Let's visualize the sample input:</p>
<p><img src="file://qT6C8C7e.png" alt="" width="1053" height="418"></p>
<p>Case 1 is just the sample mentioned above.</p>
<p>Case 2 has 20 potential isosceles triangels: (1, 0, 2), (3, 1, 4), (5, 1, 9), (6, 1, 15), (7, 4, 9), (8, 4, 15), (10, 4, 17), (12, 9, 15), (10, 8, 11), (16, 15, 17), (13, 10, 14), (18, 16, 19), (4, 1, 0), (1, 4, 7), (4, 9, 12), (7, 8, 11), (9, 15, 16), (8, 10, 14), (15, 16, 19) and (4, 15, 18).</p>
<p>Case 3 has no triangles.</p>