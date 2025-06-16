<p>Trees comes in many varieties other than the popular binary tree. In general, a tree is a connected acyclic
graph. That is, it consists of some number of vertices N (which we¡¯ll assume is at least one in this problem),
and N ¨C 1 edges, each of which connects a pair of vertices.

</p><p></p><p>
A ¡°labeled tree¡± is a tree in which each vertex has been given a ¡°label.¡± For simplicity, let us assume these
labels are the integers 1 through N. In how many different ways may a tree with N vertices be labeled? By
¡°different¡± we mean that no rearrangement of two trees with the same number of vertices with different
labeling will be identical. (Note that although we commonly associate data with each vertex, and identify
one vertex as the root of the tree, that¡¯s not significant in this problem.)

</p><p></p><p>
Let¡¯s consider some examples. The figure below shows all possible arrangements of trees with N = 1, 2, 3,
4, or 5 vertices. The number shown below each tree is the number of different ways in which the vertices
in each tree can be labeled.

</p><p></p><p>
</p><center><img src="/content/steinersp:label1.jpg" alt="Illustration" border="0" width="100%"></center>

<p></p><p>
Clearly a tree with only one vertex can be labeled in only one way ¨C by assigning the label ¡°1¡± to the single
vertex. A tree with two vertices can also be labeled in only one way. For example, although the two trees
shown on the left below appear to be different, the first can be easily transformed into the second.
(Imagine the edges are strings, so the vertices can be easily repositioned without losing their connectivity.)

</p><p></p><p>
</p><center><img src="/content/steinersp:label2.jpg" alt="Illustration" border="0" width="100%"></center>

<p></p><p>
There are, however, three possible ways to label the vertices in a 3-vertex tree, as shown on the right
above. No matter how you rearrange the labeled vertices in any of the three trees, you cannot produce any
of the other labeled trees.

</p><p></p><p>
In a similar manner, the various arrangements of four vertices in a tree yield a total of 16 possible labelings
¨C 12 for the four vertices ¡°in a row,¡± and 4 for the other configuration. There are three possible
arrangements of the vertices in a tree with N = 5, with a total of 125 possible

</p><h3>Input</h3>
<p>There will be multiple cases to consider. The input for each case is an integer N specifying the number of
vertices in a tree, which will always be between 1 and 10. The last case will be followed by a zero.

</p><h3>Output</h3>
<p>For each input case, display the case number (1, 2, ¡­), the input value of N, and the number of different
ways in which a tree with N vertices may be labeled. Use the format shown in the examples below.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
3
4
5
0

<b>Output:</b>
Case 1, N = 2, # of different labelings = 1
Case 2, N = 3, # of different labelings = 3
Case 3, N = 4, # of different labelings = 16
Case 4, N = 5, # of different labelings = 125
</pre>