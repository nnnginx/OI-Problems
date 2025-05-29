<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>King Graff, the ruler of the land of Feerie, feels that he is not quite rich enough. As such, he would like to impose travel tolls on his people! After all, why should they get to walk around his kingdom for free?</p>
<p>Feerie consists of $N$ ($1 \leq N \leq 10^5$) towns (numbered $1..N$), and $N-1$ roads. The $i$th road runs between distinct towns $A_i$ and $B_i$, in both directions. Every pair of towns is connected by exactly one path of connected roads. Currently, all travel is free, but King Graff is interested in charging for passage through certain towns.</p>
<p>He is planning to have a meeting with the royal computer scientest - that would be you. The meeting will last $M$ ($1 \leq M \leq 10^5$) minutes, and in the $i$th minute, one of two things will occur, described by $T_i$. If $T_i=$ "T", Graff will proclaim that town $X_i$ shall henceforth cost $Y_i$ ($0 \leq Y_i \leq 10^9$) dollars to pass through, and you'll update the map accordingly. Otherwise, if $T_i=$ "Q", he will ask you how much a trip from town $X_i$ to a different town $Y_i$ would currently cost a commoner, in order to gauge the effectiveness of his tolls - and you had better answer quickly! Note that neither the starting nor the ending town's tolls are included in a trip's cost, as they are not passed through. Note also that a town's toll may be modified by Graff mutiple times throughout the meeting, in which case the most recent modification at any point will stand.</p>
<h3>Input</h3>
<p>First line: 1 integer, $N$</p>
<p>Next $N-1$ lines: 2 integers, $A_i$ and $B_i$, for $i = 1..N-1$</p>
<p>Next line: 1 integer, $M$</p>
<p>Next $M$ lines: 1 character, $T_i$, and 2 integers, $X_i$ and $Y_i$, for $i = 1..M$</p>
<h3>Output</h3>
<p>$X$ lines (where $X$ is the number of questions asked by King Graff): 1 integer, the cost of the $i$th trip asked for (in dollars), for $i = 1..X$</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">4</span>
<span style="font-family: 'courier new', courier;">1 3</span>
<span style="font-family: 'courier new', courier;">2 3</span>
<span style="font-family: 'courier new', courier;">4 3</span>
<span style="font-family: 'courier new', courier;">6</span>
<span style="font-family: 'courier new', courier;">Q 1 4</span>
<span style="font-family: 'courier new', courier;">T 3 5</span>
<span style="font-family: 'courier new', courier;">Q 4 2</span>
<span style="font-family: 'courier new', courier;">Q 3 1</span>
<span style="font-family: 'courier new', courier;">T 3 1</span>
<span style="font-family: 'courier new', courier;">Q 1 2</span></pre>
<p><strong>Outut:</strong></p>
<pre><span style="font-family: 'courier new', courier;">0</span>
<span style="font-family: 'courier new', courier;">5</span>
<span style="font-family: 'courier new', courier;">0</span>
<span style="font-family: 'courier new', courier;">1</span></pre>
<pre><span style="font-weight: bold;">Explanation of Sample:</span></pre>
<p>The map of Feerie is illustrated below:</p>
<p><img src="../../../content/sourspinach:grafftol.png" alt=""></p>
<p>The first trip asked for by King Graff goes through towns $1 \rightarrow 3 \rightarrow 4$. Since town 3 has no toll at that point, the trip's cost is 0.</p>
<p>The second trip goes through towns $4 \rightarrow 3 \rightarrow 2$ and has a cost of 5, due to the new toll on town 3.</p>
<p>The third trip goes through towns $3 \rightarrow 1$, passing through no towns and so costing nothing.</p>
<p>The final trip goes through towns $1 \rightarrow 3 \rightarrow 2$ and costs only 1, as town 3's toll is reduced by then.</p>