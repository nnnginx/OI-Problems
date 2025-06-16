<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Jim-Bob lives in a strange city where the streets don¡¯t necessarily run NS or EW. Instead, the $N$&nbsp;($1 \leq N \leq 10^5$) streets run seemingly at random, sometimes crossing over each other by bridges, and intersecting with one another at exactly $K$&nbsp;($1 \leq K \leq 1000$) intersections. Each intersection consists of some streets coming together, as well as a traffic light.</p>
<p>Street $i$&nbsp;starts at intersection $s_i$<strong><sub>&nbsp;</sub></strong>($1 \leq s_i \leq&nbsp;K$), and ends at a different intersection $e_i$<strong><sub>&nbsp;</sub></strong>($1 \leq e_i \leq&nbsp;K$), going through no other intersections in between. It takes $t_i$&nbsp;($1 \leq t_i \leq&nbsp;1000$) minutes to travel down street $i$&nbsp;(this number is derived from the length, the average pothole size, and the amount of roadkill). Each road can be travelled in either direction in the same amount of time.</p>
<p>The traffic lights in this city are also strange. First of all, each one only alternates between green and red. Each light also cycles through these colours at a different rate ¨C the traffic light located at intersection $i$&nbsp;stays green for $g_i$&nbsp;($1 \leq g_i \leq&nbsp;1000$) minutes, then stays red for $r_i$&nbsp;($1 \leq r_i \leq&nbsp;1000$) minutes, then goes back to green, and so on.</p>
<p>Jim-Bob always obeys the law, and will never run a red light. If he arrives at an intersection while the light is green, he can pass right through it. Otherwise, he must wait there until the light turns green. If he gets to an intersection just as the traffic light is turning red, he must wait. It takes no time to drive through an intersection, so the light will never turn red on him as he drives through.</p>
<p>Jim-Bob starts at his house, also known as intersection $1$. As soon as he leaves his house, all the traffic lights turn green, starting their green-red-green cycle. He wishes to drive to Billy-Bob¡¯s house (which is right at intersection $K$) as fast as possible. Neither the starting nor the finishing intersections have traffic lights, so their $g$&nbsp;and $r$&nbsp;values will be given as 0. Find the minimum number of minutes Jim-Bob can take to drive from his house to Billy-Bob¡¯s.</p>
<h3>Input</h3>
<p>Line $1$: 2 integers, $N$&nbsp;and $K$</p>
<p>Next $N$&nbsp;lines: 3 integers, $s_i$, $e_i$, and $t_i$, for $i=1..N$</p>
<p>Next $K$&nbsp;lines: 2 integers, $g_i$ and $r_i$, for $i=1..K$</p>
<h3>Output</h3>
<p>A single integer ¨C the minimum number of minutes it takes to drive from Jim-Bob¡¯s house to Billy-Bob¡¯s. It will always be possible to do this.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">7 6</span>
<span style="font-family: 'courier new', courier;">1 2 4</span>
<span style="font-family: 'courier new', courier;">1 3 1</span>
<span style="font-family: 'courier new', courier;">3 5 2</span>
<span style="font-family: 'courier new', courier;">2 4 2</span>
<span style="font-family: 'courier new', courier;">2 5 6</span>
<span style="font-family: 'courier new', courier;">5 4 2</span>
<span style="font-family: 'courier new', courier;">5 6 10</span>
<span style="font-family: 'courier new', courier;">0 0</span>
<span style="font-family: 'courier new', courier;">5 5</span>
<span style="font-family: 'courier new', courier;">1 20</span>
<span style="font-family: 'courier new', courier;">2 5</span>
<span style="font-family: 'courier new', courier;">10 2</span>
<span style="font-family: 'courier new', courier;">0 0</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">19</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>Jim-Bob can drive to intersection 2 (4 min), drive on to intersection 4 (2 min), wait for the green light (1 min), drive down to intersection 5 (2 min), and finally drive to Billy-Bob¡¯s house (10 min). This is a total of 19 minutes.</p>
<p>Note: The traffic light at intersection 3 only stays green for 1 minute, which means that Jim-Bob would just miss it if he drove directly there. On the other hand, he makes the green lights at intersections 2 and 5 just in time, as they turn red 1 minute after he passes.</p>
<p>&nbsp;</p>