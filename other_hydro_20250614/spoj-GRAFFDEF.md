<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>King Graff, the ruler of the land of Feerie, has a problem - his nation is under attack! Luckily, he has an army at his disposal, composed of a whopping $S$ soldiers (where $S = 2$).</p>
<p>Feerie consists of $N$ ($1 \leq N \leq 100,000$) towns (numbered $1..N$), and $M$ ($1 \leq M \leq 500,000$) roads. The $i$th road runs between distinct towns $A_i$ and $B_i$, in both directions. No pair of towns is directly connected by more than one road, but every pair of towns is connected by at least one path of connected roads. King Graff would like to position his two soldiers in two different towns to prepare for the impending assault - however, since he's not much of a strategist, he'll choose the towns at complete random.</p>
<p>Graff's only real concern is with his enemies using a divide-and-conquer strategy. His soldiers will be susceptible to this type of attack if there exists any single road that, if blocked, will prevent them from reaching each other by any system of connected roads. As the royal computer scientist, your job is to determine the probability that King Graff will be defeated.</p>
<h3>Input</h3>
<p>First line: 2 integers, $N$ and $M$</p>
<p>Next $M$ lines: 2 integers, $A_i$ and $B_i$, for $i = 1..M$</p>
<h3>Output</h3>
<p>1 real number (rounded to 5 decimal places), the probability that the two towns chosen by Graff can be disconnected by the removal of any single road</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">4 4</span>
<span style="font-family: 'courier new', courier;">1 2</span>
<span style="font-family: 'courier new', courier;">1 3</span>
<span style="font-family: 'courier new', courier;">2 4</span>
<span style="font-family: 'courier new', courier;">4 1</span></pre>
<p><strong>Output:</strong></p>
<pre><span style="font-family: 'courier new', courier;">0.50000</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The map of Feerie is illustrated below:</p>
<p><img src="../../../content/sourspinach:graffdef.png" alt=""></p>
<p>King Graff can make 6 possible choices as to where to place his soldiers, and three of those (the three with one of the soldiers being at town 3) result in defeat (if the road between towns 1 and 3 is destroyed). The probability of failure is then $3/6 = 0.5$.</p>