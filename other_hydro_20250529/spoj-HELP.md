<p>
Preparing a problem for a programming contest takes a lot of time.
Not only do you have to write the problem description and write a
solution, but you also have to create difficult input files.
In this problem, you get the chance to help the problem setter
to create some input for a certain problem.<br>
For this purpose, let us select the problem which was not solved
during last year's local contest. The problem was about
finding the optimal binary search tree, given the probabilities that
certain nodes are accessed. Your job will be: given the desired optimal
binary search tree, find some access probabilities for which this binary
search tree is the unique optimal binary search tree. Don't worry if
you have not read last year's problem, all required definitions are provided
in the following.<br>
Let us define a <b>binary search tree</b>
inductively as follows:<br>
</p>
<ul>
  <li>The empty tree which has no node at all is a binary search tree</li>
  <li>Each non-empty binary search tree has a root, which is a node
labelled with an integer, and two binary search trees as left and right
subtree of the root</li>
  <li>A left subtree contains no node with a label �� than the label of
the root</li>
  <li>A right subtree contains no node with a label �� than the label of
the root</li>
</ul>
<p>Given such a binary search tree, the following <b>search procedure</b>
can be used to locate a node in the tree:<br>
Start with the root node. Compare the label of the current node with
the desired label. If it is the same, you have found the right node.
Otherwise, if the desired label is smaller, search in the left subtree,
otherwise search in the right subtree.<br>
The <b>access cost</b> to locate a node is the number of nodes you
have to visit until you find the right node.
An <b>optimal binary search tree</b> is a binary search tree
with the minimum expected access cost.</p>
<h3>Input Specification</h3>
<p>The input file contains several test cases.<br>
Each test case starts with an integer <i>n</i> (<i>1 �� n ��
50</i>),
the number of nodes in the optimal binary search tree.
For simplicity, the labels of the nodes will be integers from <i>1</i>
to <i>n</i>. The following <i>n</i> lines describe the structure of
the
tree. The <i>i</i>-th line contains the labels of the roots
of the left and right subtree of the node with label <i>i</i>
(or -1 for an empty subtree). You can assume that the
input always defines a valid binary search tree.<br>
The last test case is followed by a zero. </p>
<h3>Output Specification</h3>
<p>For each test case, write one line containing the access frequency
for each node in increasing order of the labels of the nodes.
To avoid problems with floating point precision, the frequencies should
be written as integers, meaning the access probability for a node will be the
frequency divided by the sum of all frequencies. Make sure that you
do not
write any integer bigger than 2<sup>63</sup> - 1 (the maximum value fitting in
the
C/C++ data type <i>long long</i> or the Java data type <i>long</i>).
Otherwise, you may produce any solution ensuring that there is exactly
one optimal binary search tree: the binary search tree given in the
input.
</p>
<h3>Sample Input</h3>
<pre>3
-1 -1
1 3
-1 -1
10
-1 2
-1 3
-1 4
-1 5
-1 6
-1 7
-1 8
-1 9
-1 10
-1 -1
0
</pre>
<h3>Sample Output</h3>
<pre>1 1 1
512 256 128 64 32 16 8 4 2 1
</pre>
<hr>
<b><i>Note that the first test case in the sample input describes a
tree looking like </i></b>
<pre>  2  
 / \ 
1   3
</pre>