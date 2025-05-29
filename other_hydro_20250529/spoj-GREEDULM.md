<p>

In the following we define the basic terminology of trees.
A <b>tree</b> is defined inductively: It has a <b>root</b> which is either an <b>external node</b> (a leaf), or an <b>internal node</b> having a sequence of trees as its children.
An internal node is also called the <b>parent</b> of the roots of its child trees.
The <b>level</b> of a node in a tree is defined inductively: The root has level <code>0</code>, and the level of a node is <code>1</code> more than the level of its parent node.


</p><p>

Every internal node of a <b>binary tree</b> has precisely two children, its left sub-tree and its right sub-tree.
Every internal node of a <b>labelled binary tree</b> is additionally marked with a string, its label.
A <b>binary search tree</b> is a labelled binary tree where every internal node <code>t</code> satisfies the following condition: All labels of nodes in the left sub-tree of <code>t</code> are less than the label of <code>t</code> which is, in turn, less than all labels of nodes in the right sub-tree of <code>t</code>.
For this condition, we assume lexicographic, i.e., alphabetic order on the strings.


</p><p>

An <b>inorder traversal</b> of a tree is defined recursively: A leaf is just visited, and for an internal node first its left sub-tree is traversed inorder, then the node itself is visited, finally its right sub-tree is traversed inorder.
It follows that an inorder traversal of a binary search tree yields the labels in lexicographic order.
Note that binary search trees whose shapes differ may nevertheless yield the same sequence of strings while being traversed inorder.

</p><p>

When a given string <code>s</code> is looked for in a binary search tree, we compare <code>s</code> to the label <code>l</code> of the root.
We are done if <code>s=l</code>, otherwise if <code>s&lt;l</code> we continue to search in the left sub-tree, and if <code>s&gt;l</code> in the right sub-tree.
If a leaf is reached, we know that <code>s</code> is not in the tree.


</p><p>

The number of comparisons performed in such a search procedure depends on <code>s</code> and the actual shape of the search tree.
Therefore, there is an interest in constructing binary search trees that store a given sequence of strings but provide as efficient access as possible.
Of course, we don't know in advance which strings will be looked up in the tree, so we need to make some assumptions.

</p><p>

Let <code>n</code> be the number of strings that are to be stored in the binary search tree.
Let <code>K<sub>1</sub>,...,K<sub>n</sub></code> be these strings in lexicographic order.
Let <code>p<sub>1</sub>,...,p<sub>n</sub></code> and <code>q<sub>0</sub>,...,q<sub>n</sub></code> be <code>2n+1</code> non-negative real numbers such that <code>¡Æ<sub>i=1..n</sub> p<sub>i</sub> + ¡Æ<sub>i=0..n</sub> q<sub>i</sub> = 1</code>.
The interpretation of these numbers is:

</p><ul>
<li><code>p<sub>i</sub></code> = probability that the search argument <code>s</code> is <code>K<sub>i</sub></code>.
</li><li><code>q<sub>i</sub></code> = probability that <code>s</code> lies (lexicographically) strictly between <code>K<sub>i</sub></code> and <code>K<sub>i+1</sub></code>.

</li></ul>

<p>
By convention, <code>q<sub>0</sub></code> is the probability that <code>s</code> is less than <code>K<sub>1</sub></code>, and <code>q<sub>n</sub></code> is the probability that <code>s</code> is greater than <code>K<sub>n</sub></code>.
We want to find a binary search tree containing nodes with labels <code>K<sub>1</sub>,...,K<sub>n</sub></code> that minimises the expected number of comparisons in the search, namely

</p><center>
<code>cost = ¡Æ<sub>i=1..n</sub> p<sub>i</sub>*(1 + level of internal node K<sub>i</sub>) + ¡Æ<sub>i=0..n</sub> q<sub>i</sub>*(level of leaf between K<sub>i</sub> and K<sub>i+1</sub>)</code>.

</center>
<p>
The leaf between <code>K<sub>i</sub></code> and <code>K<sub>i+1</sub></code> is that leaf reached in the search for a string <code>s</code> that lies (lexicographically) strictly between <code>K<sub>i</sub></code> and <code>K<sub>i+1</sub></code>.
Adhere to the convention stated above for the border cases.


</p><p>

The following figure illustrates the first test case of the sample input.
It shows the two possible binary search trees, the probabilities and the associated costs.

</p><p>

</p><center>
<img src="./22659/file/PYkWUa20.png">
</center>

<h3>Input Specification</h3><p>

The input contains several test cases.
Every test case starts with an integer <code>n</code>.
You may assume that <code>1&lt;=n&lt;=200</code>.
Then follow <code>2n+1</code> non-negative integers denoting frequencies.
Let <code>s</code> be the sum of all frequencies.
You may assume that <code>1&lt;=s&lt;=1000000</code>.
The probabilities <code>p<sub>1</sub>,...,p<sub>n</sub></code> and <code>q<sub>0</sub>,...,q<sub>n</sub></code> are calculated in this order by dividing the frequencies by <code>s</code>.
The last test case is followed by a zero.


</p><h3>Output Specification</h3><p>

For each test case devise a binary search tree whose cost is minimal for the specified probabilities.
Output the integer <code>cost*s</code> for such a tree.

</p><h3>Sample Input</h3><p>
<small>
</small></p><pre><small>2
20 15 15 25 25
35
142 35 58 5 20 5 10 9 15 23 129 4 52 5 38 18 9 7 2 4 266 93 5 18 18 27 5 10 11 180 4 32 21 3 21
0 55 27 36 85 31 58 3 334 0 98 27 113 89 180 0 62 12 0 37 0 3 64 70 0 277 0 0 0 170 0 18 76 27 3 29
0
</small></pre><small>
</small>

<h3>Sample Output</h3><p>

</p><pre>160
13637

</pre>