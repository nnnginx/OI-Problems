<p>Ada the Ladybug is on a trip in Bugindia. There are many cities and some uni-directional roads connecting them. Ada is wondering about the shortest path, which begins in a city and ends in the same city. Since Ada likes short trips, she asked you to find the length of such path for each city in Bugindia.</p>
<h3>Input</h3>
<p>The first line will contain <strong>0 &lt; N ¡Ü 2000</strong>, the number of cities.</p>
<p>Then <strong>N</strong> lines follow, each containing <strong>N</strong> integers <strong> 0 ¡Ü     H<sub>ij</sub> ¡Ü 1</strong>. One means, that there is a road between <strong> i </strong> and <strong> j </strong> (zero means there isn't a road).</p>
<h3>Output</h3>
<p>Print <strong>N</strong> lines, the length of shortest path which begins in city <strong>i</strong> and ends in city <strong>i</strong>. If the path doesn't exist, print "<strong>NO WAY</strong>" instead.</p>
<h3>Example Input</h3>
<pre>5
0 1 1 1 1
1 0 0 0 1
0 0 1 1 0
0 0 1 0 0
0 0 0 1 0
</pre>
<h3>Example Output</h3>
<pre>2
2
1
2
NO WAY
</pre>
<h3>Example Input</h3>
<pre>5
0 1 0 0 1
0 0 1 0 0
0 0 0 1 0
0 0 0 0 1
1 0 0 0 0
</pre>
<h3>Example Output</h3>
<pre>2
5
5
5
2
</pre>