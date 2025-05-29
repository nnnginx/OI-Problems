<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>A family of Foxen, having caught a pesky farmer on their property, want to teach him a lesson. Of course, they're not cruel - they plan to simply prevent him from returning home to his farm, until he's willing to beg them for mercy.</p>
<p>The Foxen and the farmer live in a forest, which may be viewed as a grid of cells, with $H$ ($1 \leq H \leq 6$) rows of $W$ ($1 \leq W \leq 6$) cells each. Each cell contains either grass (represented by "G"), trees ("T"), the farmer ("F"), or his farm ("H"). The farmer may repeatedly move up, down, left, or right to adjacent cells within the grid, provided that they are not blocked by trees. Due to his overconfidence in exploring the forest, the farmer is not directly adjacent to his farm.</p>
<p>The family of Foxen can also block the farmer's way, by standing in grass-filled cells. He would not, of course, dare to enter a cell with a Fox in it. However, the Foxen do have better things to do, so they'd like to determine the minimum number of cells they must occupy in order to prevent the farmer from ever reaching his farm.</p>
<p>There are $T$ ($1 \leq T \leq 20$) scenarios as described above. For each one, you'd like to answer the Foxen's question. Note that no Foxen might be necessary, if the trees already bar the farmer's way sufficiently.</p>
<h3>Input</h3>
<p>First line: 1 integer, $T$</p>
<p>For each scenario:</p>
<p>First line: 2 integers, $H$ and $W$</p>
<p>Next $H$ lines: $W$ characters, representing the $i$th row of the grid, for $i = 1..H$</p>
<h3>Output</h3>
<p>For each scenario:</p>
<p>1 integer, the minimum number of Foxen necessary to block the farmer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>1 5<br>FGTGH<br>4 5<br>GGGGG<br>GFGTG<br>GTTGH<br>GGGGG</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">0<br>2</span>&nbsp;</pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>In the first scenario, the farmer can already never reach his farm, so no Foxen are necessary.</p>
<p>In the second scenario, one possible placement of two Foxen (each represented by an "X") is as follows:</p>
<pre><span style="font-family: 'courier new', courier;">GGGGX<br>GFGTG<br>GTTGH<br>GGXGG</span></pre>