<p>Given a rooted tree, a permutation of its nodes is valid if the following holds: for each pair of nodes <strong>a</strong> and <strong>b</strong>, if <strong>a</strong> is an ancestor of <strong>b</strong>, then <strong>a</strong> appears before <strong>b</strong> in the permutation. Let <strong>P(t)</strong> be the number of valid permutations for a tree <strong>t</strong>.<br><br>Given an integer N, you can construct all the possible trees of N nodes, numbered from 1 to N, <em><strong>rooted at </strong></em><strong>1</strong>. I'd like to know what's the sum of <strong>P(t)</strong> <strong><em>for all</em></strong> <strong>t</strong> that can be constructed for the given N.</p>
<p><strong>We consider two trees equal iff each node in the second tree has the same parent as it does in the first one.&nbsp;</strong></p>
<p style="text-align: center;"><img title="trees" src="../../../content/syntax_error:ttop.png" alt="trees for N = 3" width="247" height="153"></p>
<p style="text-align: center;"><em>The picture shows all the possible trees for N = 3.</em></p>
<h3>Input</h3>
<p>A single integer N ( 1 &lt;= N &lt;= 1000000 ).</p>
<h3>Output</h3>
<p>A single integer representing the solution modulo 1000000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong> <br>3<br><strong>Output:</strong> <br>4</pre>
<p><strong>Explanation:</strong> If you take a look at the picture, you'll see that the first two trees have one valid permutation each, and the third tree has two, namely { 1, 2, 3 } and { 1, 3, 2 }. The total is, of course, 4.</p>