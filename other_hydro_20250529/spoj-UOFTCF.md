<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>This evening, Alice and Bob have decided to simply go out on a nice walk together. On the way, they'll traverse $S$ ($1 \leq S \leq 50$) different sidewalks. Now that they won't be watching engrossing movies, Bob really wouldn't mind holding Alice's hand - however, this can sometimes be difficult to maintain, due to potential obstacles in their way.</p>
<p>A given sidewalk can be modelled as a two-dimensional grid of cells, with $R$ ($1 \leq R \leq 50$) rows and $C$ ($1 \leq C \leq 50$) columns. The $j$th cell in the $i$th row is referred to as cell ($i$, $j$). Each cell is either walkable (represented by a "."), or is blocked by the neighbourhood dog's droppings ("#"). Alice and Bob will be walking Southwards along it, independently of one another, but both at a rate of exactly one row per second. Needless to say, they'll never walk through cells containing droppings, nor can they ever occupy the same cell as one another. Each of them can start in any cell on row 1, and each second, will move down by a cell, as well as optionally left or right by a cell. In other words, if Alice or Bob is in cell ($i$, $j$), they can then move to either cell ($i+1$, $j-1$), ($i+1$, $j$), or ($i+1$, $j+1$), as long as they don't step off the sidewalk. This continues until they've both made it to row $R$, at which point they step off and make their way towards the next sidewalk on their route. It might also be the case that they're unable to both navigate to the end of the sidewalk, in which case they'll take a detour around it entirely.</p>
<p>Along the way, whenever Alice and Bob find themselves side-by-side (in other words, in cells ($i$, $j$) and ($i$, $j+1$), for some $i$ and $j$), they can hold hands for that second! Bob is interested in coordinating their walk to enable them to hold hands for as long as possible.</p>
<h3>Input</h3>
<p>Line 1: 1 integer, $S$</p>
<p><strong>For each sidewalk:</strong></p>
<p>Line 1: 2 integers, $R$ and $C$</p>
<p>Next $R$ lines: $C$ characters, representing the $i$th row of the sidewalk grid, for $i=1..R$</p>
<h3>Output</h3>
<p><strong>For each sidewalk:</strong></p>
<p>1 integer, the maximal number of seconds Alice and Bob can spend holding hands, or the string "Detour" if they can't both make it to the end.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>5 5<br>#....<br>..##.<br>.#...<br>#.#..<br>....#<br>2 4<br>.##.<br>..##<span>&nbsp;</span></span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">4<br>Detour</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>On the first sidewalk, Bob can ask Alice to walk through cells (1, 3), (2,2), (3, 3), (4, 4), and (5, 3), while he goes through cells (1, 4), (2, 5), (3, 4), (4, 5), and (5, 4). The two of them will then get to hold hands while on rows 1, 3, 4, and 5, for a total of 4 seconds.</p>
<p>However, there's no way for both Alice and Bob to navigate the second sidewalk. They must start in cells (1, 1) and (1, 4), and no walkable cells on the second row can be reached from cell (1, 4).</p>