<p>A <b>tree</b> consists of a node and some (zero, one or two) subtrees connected
to it. These subtrees are called children.</p>
<p>A <b>specification</b> of the tree is a sequence of digits. If the number of
children in the tree is:</p>
<ul>
<li>zero, then the specification is a sequence with only one element '0';
</li><li>one, the specification begins with '1' followed by the specification of the
  child;
</li><li>two, the specification begins with '2' followed by the specification of the
  first child, and then by the specification of the second child.
</li></ul>
<p>Each of the vertices in the tree must be painted either red or green or blue.<br>
However, we need to obey the following rules:</p>
<ul>
<li>the vertex and its child cannot have the same color,
</li><li>if a vertex has two children, then they must have different colors.
</li></ul>
<p>How many vertices may be painted green?</p>

<h3>Task</h3>
<p>
Write a program which:
</p><ul>
<li>reads the specification of the tree from the standard input,
</li><li>computes the maximal and the minimal number of vertices that may be painted
  green,
</li><li>writes the results in the standard output.
</li></ul>

<h3>Input</h3>

<p>
The number of test cases t is in the first line of input, then t test cases follow in separate lines.
Each test case consists of one word (no
longer then 10000 characters), which is a specification of a tree.</p>

<h3>Output</h3>

<p>Your program should write for each test case 
exactly two integers separated by a single space, which respectively
denote the
maximal and the minimal number of vertices that may be painted green.</p>

<h3>Example</h3>
<pre><b>Sample input:</b>
1
1122002010

<b>Sample output:</b>
5 2
</pre>