<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The heated competition of the ACM-ICPC World Finals continues, and The Team is at the top of their game! Well, okay, maybe they're not actually doing so well, according to the scoreboard, yet. But they have a plan!</p>
<p>The contest is taking place in a huge room with a regular grid of desks. The columns and rows are each numbered $1..10^6$, and the desk in the $x$th column and $y$th row is considered to have coordinates ($x$,$y$). The Team is sitting at coordinates ($X$,$Y$). There are $N$ ($1 \leq N \leq 10^6$) opposing teams (conveniently numbered $1..N$), with team $i$ having $m_i$ ($1 \leq m_i \leq 10^6$) members, all sitting at coordinates ($x_i$,$y_i$). No desk is occupied by more than one team, and all other desks are empty.</p>
<p>Now, The Team is interested in removing some of the more dangerous opponents from the competition. To accomplish this, they have a number of water balloons at their disposal (after all, where in the contest rules does it say that water balloons are not allowed?). Always conservative, they would first like to answer $Q$ ($1 \leq Q \leq 10^6$) queries - for the $i$th query, how many balloons it would theoretically take to take out all of the members of team $q_i$?</p>
<p>In order to do any real damage, the water balloons will of course have to be thrown extremely hard - in fact, in a perfectly straight line, and not over any obstacles besides empty desks. This means that, if team $j$ lies exactly on the line segment from The Team to team $i$, then every member of team $j$ must be dispatched before any members of team $i$ can be hit. It takes one balloon to knock one person out (the members of The Team have received plenty of training, so they're not about to miss a throw). Note that these queries are all only theoretical (for the moment) - so each should be answered assuming that all teams are still untouched.</p>
<p>The members of The Team will need to carefully choose with opponents to take out, based on how well they're doing and how many balloons it would take, so they're already answered all of their queries in their heads. Maybe, if you can answer them as well, you can also adopt such techniques in the future...</p>
<h3>Input</h3>
<p>First line: 4 integers, $N$, $Q$, $X$, and $Y$</p>
<p>Next $N$ lines: 3 integers, $x_i$, $y_i$, and $m_i$, for $i = 1..N$</p>
<p>Next $Q$ lines: 1 integer, $t_i$, for $i = 1..Q$</p>
<h3>Output</h3>
<p>$Q$ lines: 1 integer, the number of balloons that would be required to take out team $t_i$, for $i = 1..Q$.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">6 6 3 2</span>
<span style="font-family: 'courier new', courier;">5 6 3</span>
<span style="font-family: 'courier new', courier;">2 1 5</span>
<span style="font-family: 'courier new', courier;">4 4 2</span>
<span style="font-family: 'courier new', courier;">4 3 1</span>
<span style="font-family: 'courier new', courier;">5 4 2</span>
<span style="font-family: 'courier new', courier;">7 6 1</span>
<span style="font-family: 'courier new', courier;">6</span>
<span style="font-family: 'courier new', courier;">5</span>
<span style="font-family: 'courier new', courier;">4</span>
<span style="font-family: 'courier new', courier;">3</span>
<span style="font-family: 'courier new', courier;">2</span>
<span style="font-family: 'courier new', courier;">1</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">4</span>
<span style="font-family: 'courier new', courier;">3</span>
<span style="font-family: 'courier new', courier;">1</span>
<span style="font-family: 'courier new', courier;">2</span>
<span style="font-family: 'courier new', courier;">5</span>
<span style="font-family: 'courier new', courier;">5</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The following grid shows the positions of the $N$ opposing teams (marked with their numbers), as well as The Team (marked with a "T"). The line segments represent direct lines of sight to the opponents.</p>
<p><img src="../../../content/sourspinach:goodf.jpg" alt=""></p>
<p>As can be seen, team 6 is blocked by teams 4 and 5. Therefore, taking them out would require $1+2+1=4$ balloons in total. Similarly, team 5 is blocked by team 4, and requires $1+2=3$ balloons. Teams 4, 3, and 2 are not blocked by any others, and so only require 1, 2, and 5 balloons, respectively. Finally, team 1 is blocked by team 3, and would require $2+3=5$ balloons to dispose of.</p>