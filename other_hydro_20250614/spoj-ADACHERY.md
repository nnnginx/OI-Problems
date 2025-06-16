<p>As you might already know, Ada the Ladybug is a farmer. She grows cherry and now she wants to collect them. She is wondering about the number of cherries she will collect. But befor you could help here, you shall know some biological facts:</p>
<p>Firstly, almost everyone think that cherry-tree is a tree. But it might not be true - in fact, it is a graph.</p>
<p>Secondly, you have to know, how a cherry looks like. It is not hard to recognize a chery - it is a node, which is connected to another two nodes, which are NOT connected.</p>
<p><strong>NOTE</strong>: Even though the cherry-tree structure might be weird, note that there won't be any multi-branches nor self-branches. Anyway do not assume it is not a cherry-forest.</p>
<p><strong>This is a cherry:</strong></p>
<p><img title="Cherry" src="../../content/morass:cherry.png" alt="Cherry"></p>
<p><strong>This is NOT a cherry:</strong></p>
<p><img title="Not a cherry" src="../../content/morass:notcherry.png" alt="Not a cherry"></p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains two integers <strong> 1 ¡Ü N, M ¡Ü 10<sup>5</sup></strong>, the number of nodes of cherry-tree and the number of branches (edges) connecting them.</p>
<p>The next <strong>M</strong> lines contains two integers <strong>0 ¡Ü a, b &lt; N</strong>, the branch connecting two nodes.</p>
<h3>Output</h3>
<p>Print a single line - the number of cherries on the cherry-tree.</p>
<h3>Example Input</h3>
<pre>4 2
1 2
3 2
</pre>
<h3>Example Output</h3>
<pre>1
</pre>
<h3>Example Input 2</h3>
<pre>5 4
1 2
1 3
1 4
1 0
</pre>
<h3>Example Output 2</h3>
<pre>6
</pre>
<h3>Example Input 3</h3>
<pre>6 6
0 1
0 2
2 1
0 3
1 4
5 3
</pre>
<h3>Example Output 3</h3>
<pre>5
</pre>