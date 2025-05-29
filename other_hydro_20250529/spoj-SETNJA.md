<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/SETNJA/en/">English</a></td> 
<td width="50%"><a href="/problems/SETNJA/vn/">Vietnamese</a></td> 
</tr></tbody></table>



<p>In an infinite binary tree:
</p><ul>
<li> Each node has exactly two children ¨C a left and a right child.
</li><li> If a node is labeled with the integer X, then its left child is labeled 2*X and its right child
2*X+1.
</li><li>The root of the tree is labeled 1.
</li></ul>
<p>A walk on the binary tree starts in the root. Each step in the walk is either a jump onto the left child,
onto the right child, or pause for rest (stay in the same node).
</p><p>A walk is described with a string of letters 'L', 'R' and 'P':
</p><ul>
<li> 'L' represents a jump to the left child;
</li><li> 'R' represents a jump to the right child;
</li><li> 'P' represents a pause.
</li></ul>
<p>The value of the walk is the label of the node we end up on. For example, the value of the walk LR is
5, while the value of the walk RPP is 3.
</p><p>A set of walks is described by a string of characters 'L', 'R', 'P' and '*'. Each '*' can be any of the three
moves; the set of walks contains all walks matching the pattern.
</p><p>For example, the set L*R contains the walks LLR, LRR and LPR. The set ** contains the walks LL, LR,
LP, RL, RR, RP, PL, PR and PP.
</p><p>Finally, the value of a set of walks is the sum of values of all walks in the set.
</p><p>Calculate the value of the given set of walks.
</p><h3>Input</h3>
<p>A string describing the set. Only characters 'L', 'R', 'P' and '*' will appear and there will be at most
10000 of them.
</p><h3>Output</h3>
<p>Output the value of the set.

</p><h3>Example</h3>

<pre><b>Input:</b>
L*R

<b>Output:</b>
25

</pre>