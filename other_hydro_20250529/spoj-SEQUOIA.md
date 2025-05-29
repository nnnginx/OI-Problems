<blockquote>
<p><em><strong>"</strong></em><em>Sequoiadendron giganteum (giant sequoia, Sierra redwood, or Wellingtonia) is the sole species in the genus Sequoiadendron, and one of three species of coniferous trees known as redwoods, classified in the family Cupressaceae in the subfamily Sequoioideae, together with Sequoia sempervirens (Coast Redwood) and Metasequoia glyptostroboides (Dawn Redwood). The common use of the name "sequoia" generally refers to Sequoiadendron, which occurs naturally only in the various groves that exist on the western slopes of the Sierra Nevada Mountains of California.</em> " - Wikipedia.</p>
</blockquote>
<p>We'll slightly redefine this beautiful tree to fit our needs:</p>
<p>We say our tree is infinite, and rooted in 0. We recursively define the tree as follows:</p>
<p>Let x be the root of a subtree. For all i from [ 0, lg( x - dad(x) )&gt;, we say the children of x are of the form 2<sup>i</sup> + x, where dad(x) is the index of x's parent. 0 has infinitely many childern. Odd nodes have no children.</p>
<p>&nbsp;</p>
<p>You will be given several queries, each consisting of two integers: A and B. You're asked to output the index of the lowest common ancestor of A and B. We define the lowest common ancestor of two nodes to be the node closest to A and B that lies on paths from A to 0 and from B to 0.</p>
<h3>Input</h3>
<p>The first line of input contains an integer N, the number of queries. ( 1 &lt;= N &lt;= 100000 )</p>
<p>The next N lines contain a pair of integers, A and B. ( 0 &lt;= A, B &lt;= 10<sup>18</sup> )</p>
<h3>Output</h3>
<p>You are asked to output N lines, where the i-th line corresponds to the answer to the i-th query.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>15 13<br>11 7<br><strong>Output:</strong>
12<br>0</pre>