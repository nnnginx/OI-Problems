<p>It was Arbor Day. Alice implemented an <a href="http://en.wikipedia.org/wiki/Red-black_tree" target="_blank">RB-tree</a>, Bob composed a <a href="http://en.wikipedia.org/wiki/Segment_tree" target="_blank">segment tree</a>, I made a <a href="http://en.wikipedia.org/wiki/Binary_tree" target="_blank">binary tree</a> - we all have a bright outlook.<br><br>Lambda is always making mistakes while implementing segment trees (See his history of submissions). He then decides to draw a "segment tree". He puts <em>n</em> points on a plane, link certain pairs of them to form segments and all the segments form a tree. As a normal tree, it satisfies the following conditions:</p>
<ol>
<li>Consider points as vertices, segments as edges, it forms a <a href="http://en.wikipedia.org/wiki/Tree_%28graph_theory%29" target="_blank">rooted tree</a>.</li>
<li>Each node <em>u</em> is <strong>strictly higher</strong> than its parent, namely <em>y<sub>u</sub></em> &gt; <em>y</em><sub><em>parent_of_u</em></sub>.</li>
<li>Segments may only intersect on their endpoints.</li>
</ol>
<p>Lambda wants to minimize the total length of segments. <strong>The tree can be rotated to satisfy above conditions.</strong></p>
<h3>Input</h3>
<p>First line of input contains single integer <em>n</em> (1 ¡Ü <em>n</em> ¡Ü 500).<br>Next <em>n</em> lines each contain two integers <em>x<sub>i</sub></em>, <em>y<sub>i</sub></em> denoting the coordinate of <em>i</em>-th point (0 ¡Ü <em>x<sub>i</sub></em>, <em>y<sub>i</sub></em> ¡Ü 1000). Points are distinct.</p>
<h3>Output</h3>
<p>The one and only line contains a real number representing the minimum length.<br>Your answer must be rounded up to 4 digits after the decimal point.</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong><br>6<br>0 1<br>1 0<br>2 1<br>4 1<br>5 0<br>6 1<br><br><strong>Output:</strong><br>7.6569<br><br><strong>Illustration:</strong><br><img src="../../../content/xfastx:SEGTREE_sample1.gif" alt="sample1"><br></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong><br>10<br>0 0<br>0 1<br>1 2<br>2 3<br>1 4<br>3 4<br>-1 2<br>-2 3<br>-1 4<br>-3 4<br><br><strong>Output:</strong><br>12.3137<br><br><strong>Illustration:</strong><br><img src="../../../content/xfastx:SEGTREE_sample2.gif" alt="sample1"><br>This is just a sample test case. There's no negative in the real test data.<br></pre>