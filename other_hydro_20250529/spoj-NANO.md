<p>You're living in the future, way beyond the singularity and the exhaustion of ipv6, and you want to plan a fastest trip between your own planet and the planet of the your favourite restaurant.</p>
<p>You have a map of one-directional nanobot ferry lines between the planets in your system. The map states the distance <strong>d<sub>ij</sub></strong> between each (connected) pair of planets <strong>i</strong> and <strong>j</strong>, but due to the rapid technical evolution of this time, you estimate the travel time from <strong>i</strong> to <strong>j</strong> is <strong>d<sub>ij</sub>/t</strong> where <strong>t</strong> is the time at which you choose to depart from <strong>i</strong>. (It is impossible to travel at t=0).</p>
<h3>Input</h3>
<p>The first line contains <strong>T</strong> the number of test cases.</p>
<p>The first line of each test case contains integers <strong>t0</strong>, <strong>N</strong>, <strong>M</strong> where</p>
<ul>
<li><strong>t0</strong> is the time at which you start your trip. 0&nbsp;��&nbsp;<strong>t0</strong>&nbsp;��&nbsp;10<sup>9</sup></li>
<li><strong>N</strong> is the number of planets in your system, numbered 0...N-1. 0 &lt; <strong>N</strong>&nbsp;�� 2.5*10<sup>5</sup></li>
<li><strong>M</strong> is the number of connections between planets. 0 &lt; <strong>M</strong>&nbsp;�� 2.5*10<sup>5</sup></li>
</ul>
<p>The following <strong>M</strong> lines of each test case contain integers <strong>i</strong>, <strong>j</strong>, <strong>d</strong> where</p>
<ul>
<li><strong>i</strong> is the source planet. 0 �� <strong>i</strong> &lt; <strong>N</strong></li>
<li><strong>j</strong> is the destination planet. 0 �� <strong>j</strong> &lt; <strong>N</strong></li>
<li><strong>d</strong> is the distance from <strong>i</strong> to <strong>j</strong>. 0 �� <strong>d</strong>&nbsp;��&nbsp;10<sup>9</sup></li>
</ul>
<h3>Output</h3>
<p>The arrival time at planet <strong>N</strong>-1 when starting at planet 0 at time <strong>t0</strong>, or "Impossible" (quotes for emphasis) if there is no possible route.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
0 5 5
0 2 2
2 3 3
3 4 4
0 1 5
1 4 6
0 2 1
1 1 0</pre>
<pre><pre><strong>Output:</strong>
4.91760625098
Impossible
</pre>
</pre>