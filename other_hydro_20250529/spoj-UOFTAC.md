<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Everyone knows that Foxen love digging holes. You've been observing one Fox in particular, who's preparing to burrow underground in search of treasures. When viewed from the side, as a cross-section, his digging site can be represented as a grid of cells, $H$ ($1 \leq H \leq 100$) deep and $W$ ($1 \leq W \leq 100$) across. Every cell contains either dirt (represented by "D"), stone ("S"), empty space ("E"), or a treasure ("T"). The surface can also be traversed, effectively giving the grid an additional row of empty cells above the topmost row.</p>
<p>The Fox starts immediately above the top-left cell, which is guaranteed to not be empty. It has a set of $N$ ($1 \leq N \leq 1000$) actions in mind before it starts its dig, which it will execute in order. Each action consists of moving either left (represented by "L"), right ("R"), or down ("D") by one cell. If the cell that the Fox would move to contains stone, or is beyond the boundaries of the grid in any direction, it will skip that action. If it enters a cell with a previously-uncollected treasure, it will collect it, leaving the cell empty. If the cell immediately below the Fox is ever empty, it will fall down until this is no longer the case. Note that collecting treasure occurs before falling, and that the Fox stops falling if it hits the bottom of the grid.</p>
<p>There are $T$ ($1 \leq T \leq 20$) scenarios as described above. For each one, you'd like to determine how many treasures the Fox will collect throughout the course of its dig.</p>
<h3>Input</h3>
<p>First line: 1 integer, $T$</p>
<p>For each scenario:</p>
<p>First line: 3 integers, $H$, $W$, and $N$</p>
<p>Next $H$ lines: $W$ characters, representing the $i$th row of the grid, for $i = 1..H$</p>
<p>Next $N$ lines: 1 character, representing the $i$th action, for $i = 1..N$</p>
<h3>Output</h3>
<p>For each scenario:</p>
<p>1 integer, the number of treasures collected in total.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>2 3 4<br>DDD<br>TES<br>R<br>D<br>R<br>L<br>3 2 6<br>TE<br>TE<br>ET<br>R<br>R<br>L<br>R<br>L<br>R</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">1<br>2</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>In the first scenario, the Fox moves right along the surface, then digs down to the first row. As the cell below it is empty, it immediately falls to the 2nd row. It ignores its next action, as the cell to its right is filled with stone, and finally moves left to claim a treasure.</p>
<p>In the second scenario, it moves to the right and promptly falls all the way down to the 2nd row. Because the Fox is already in the rightmost column, it ignores the action to move right. It then moves left, collects the treasure there, and then falls to the bottom row. Finally, it moves back and forth between the bottom-left and bottom-right cells twice - however, it only collects the treasure in the latter cell the first time.</p>