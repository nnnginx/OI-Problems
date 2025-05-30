<p>Mary and Saina participated in London Olympics 2012 and won medals for IndiaJ. After these historic moments, they planned to travel and see various places in London. Since it was their first time in the city, they bought a map to various connecting routes across London. However, the map was not proper as it had a missing entry for one route. They asked the tour planning authorities to get the correct map but all they could get was the shortest distance route map rather than the original map which gives direct distance between any 2 places in London. Mary and Saina prefer taking the direct route rather than the shortest route for travelling. Can you help them calculate the no. of possible values of direct distance which is unknown in the original map? Assume that the places are never more than 100km apart (i.e. direct distance).</p>
<h3>Input</h3>
<p>First line contains N, the no. of places in London.</p>
<p>Next N lines contains total N^2 integers, N space separated integers per line (the direct distance map). The jth column in the ith line contains either a non-negative integer (the distance from ith place to jth place), or -1 indicating the missing entry in the map.</p>
<p>Next N lines contains total N^2 integers, N space separated integers per line (the shortest distance map). The jth column in the ith line contains a non-negative integer (the shortest distance from ith place to jth place).</p>
<p>Note that direct distance from ith to jth city is not always equal to direct distance between jth to ith city and distance between a city to itself is always 0.</p>
<h3>Output</h3>
<p>Output the no. of possible values the missing entry (marked -1 in the original map) takes assuming that shortest distance map is correct.</p>
<h3>Output</h3>
<p>2&lt;=N&lt;=20</p>
<p>All distances are between 0 to 100 (including both).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre style="word-wrap: break-word; white-space: pre-wrap;">4
0 51 61 63
-1 0 66 24
80 83 0 71
60 64 52 0
0 51 61 63
84 0 66 24
80 83 0 71
60 64 52 0</pre>
<strong>Output:</strong> 17</pre>