<p>Ada the Ladybug loves trips. She travels around world taking photos and souvenirs. This week she went to Buganda. Common Tourist would surely travel around main city and some conurbations, but Ada has different politics. She wants to go as far as possible (because photos from outlying places are much more valuable).</p>
<p>Problem is, that Buganda is very large so she can barely guess such places. Luckily, you are around so she asked you for help. Can you tell her, how far and how many cities are most distant (if the shortest path is used)?</p>
<h3>Input</h3>
<p>The first line will contain three integers <strong>1 ¡Ü N ¡Ü 5*10<sup>5</sup>, 0     ¡Ü M ¡Ü 10<sup>6</sup>, Q</strong>, the number of cities in Buganda, the number of roads and number of queries (possible arrival cities).</p>
<p>Then <strong>M</strong> lines follow, with three integers <strong>0 ¡Ü A, B &lt; N, 0 ¡Ü     L ¡Ü 10</strong>, <strong>A, B</strong> are cities, which the (bidirectional) road connets and <strong>L</strong> is length of the road.</p>
<p>Afterward, <strong>Q</strong> lines follow, each with number <strong>0 ¡Ü q<sub>i</sub> &lt; N</strong>, meaning the city of arival.</p>
<p>You are asured that <strong>max(N,M)*Q</strong> will be always         lesser/equal than <strong>10<sup>7</sup></strong></p>
<p><strong>Gentle warning</strong>: Since we are in real world and not in some "graph theory", multiedges and self-edges are completely valid!</p>
<h3>Output</h3>
<p>For each query print two numbers: The distance of most distant place(s) and number of such places.</p>
<h3>Example Input</h3>
<pre>10 10 10
1 1 1
1 2 1
1 2 3 
3 1 1
5 4 10
8 5 10
5 6 5
6 7 3
6 9 3
9 7 4
0
1
2
3
4
5
6
7
8
9
</pre>
<h3>Example Output</h3>
<pre>0 1
1 2
2 1
2 1
20 1
10 2
15 2
18 2
20 1
18 2
</pre>
<h3>Most distant cities (explanation)</h3>
<pre>0
2 3
3
2
8
4 8
4 8
4 8
4
4 8
</pre>