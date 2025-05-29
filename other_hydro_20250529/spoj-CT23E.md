<div>
<p>Recently Bob invented a new game with a tree (we  should remind you, that a tree is a connected graph without cycles): he  deletes any (possibly, zero) amount of edges of the tree, and counts the  product of sizes of the connected components left after the deletion.  Your task is to find out the maximum number that Bob can get in his new  game for a given tree.</p>
</div>
<div>
<div><strong>Input</strong></div>
<p>The first input line contains  integer number <span><em>n</em></span> (<span>1 ≤ <em>n</em> ≤ 700</span>) — amount of vertices in the  tree. The following <span><em>n</em> - 1</span> lines  contain the description of the edges. Each line contains the pair of  vertices' indexes, joined by an edge, <span><em>a</em><sub><em>i</em></sub></span>, <span><em>b</em><sub><em>i</em></sub></span> (<span>1 ≤ <em>a</em><sub><em>i</em></sub>, <em>b</em><sub><em>i</em></sub>  ≤ <em>n</em></span>). It's guaranteed that the graph described in the  input is a tree.</p>
</div>
<div>
<div><strong>Output</strong></div>
<p>Output the only number — the  maximum product of sizes of the connected components, that Bob can get  after deleting some of the tree's edges.</p>
</div>
<h3>Example</h3>
<pre><strong>Input:</strong><br><pre>8<br>1 2<br>1 3<br>2 4<br>2 5<br>3 6<br>3 7<br>6 8</pre>
<br><br><strong>Output:</strong><br>18<br></pre>