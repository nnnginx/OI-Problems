<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Alice has convinced Bob to accompany her on a shopping trip! For some reason, he seems reluctant to spend too much time on it, but she has every intention of hitting every single store at $M$ ($1 \leq M \leq 100$) different malls today. Still, she's promised to get it over with as quickly as possible.</p>
<p>A given mall can be modelled as a two-dimensional grid of cells, with $R$ ($1 \leq R \leq 100$) rows and $C$ ($1 \leq C \leq 100$) columns. Each cell contains either a wall (represented by a "#"), open space ("."), a store ("S", of which there is at least one), or Bob's car ("C", of which there is exactly one). Alice and Bob can walk from one cell to a horizontally- or vertically-adjacent one in 1 minute if neither cell is blocked by a wall.</p>
<p>The two of them will start at Bob's car, and walk to a store (possibly passing through other stores on the way) so that Alice can do what she does best, which only takes her 60 minutes. At that point, due to the large volume of items purchased, they'll need to return to the car to drop them off. This process will repeat until all stores in the mall have been visited, in some order. It's guaranteed that each store is reachable from the car.</p>
<p>To reassure Bob that they won't spend too much time at each mall, Alice will leave a stopwatch running until the final items have been dropped off in the car. However, sneaky as she is, Alice will only start timing when she actually starts shopping at the first store they decide to visit. She'd like to know how much time will be spent at each mall - though she's sure that it won't be much at all.</p>
<h3>Input</h3>
<p>Line 1: 1 integer, $M$</p>
<p><strong>For each mall:</strong></p>
<p>Line 1: 2 integers, $R$ and $C$</p>
<p>Next $R$ lines: $C$ characters, representing the $i$th row of the mall grid, for $i=1..H$</p>
<h3>Output</h3>
<p><strong>For each mall:</strong></p>
<p>1 integer, the minimal number of minutes required to visit all stores and return to the car, as per Alice's stopwatch.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>4 4<br>..S#<br>.##C<br>....<br>S.#S<br>1 5<br>SSCSS</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">202<br>250</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>At the first mall, Alice and Bob can decide to visit the top store, followed by the bottom-left, and finally the bottom-right. In this case, they'll spend 60 minutes shopping, 8 minutes returning to the car, 5 minutes walking to the second store, 60 minutes shopping, 5 minutes returning to the car, 2 minutes walking to the third store, 60 minutes shopping, and 2 minutes again returning to the car. This is a total of 202 minutes.</p>
<p>At the second mall, they can decide to visit the stores left-to-right. This shopping trip will take $60+2+1+60+1+1+60+1+2+60+2=250$ minutes.</p>