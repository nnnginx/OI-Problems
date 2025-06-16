<p>Ada the Ladybug lives on a bush. A typical bush consists of some fruits connected with branches. Ada wants to travel between some fruits. Problem is that each edge can stand only some <strong>X<sub>i</sub></strong> weigth (so if some         creature  with more weigth would like to travel over the edge, it would         break and the creature would fall of the bush).</p>
<p>Ada wants to make several travels so she asks you (for each such travel) to how many distinct fruits she can get?</p>
<h3>Input</h3>
<p>The first line of each test-case will contain three integers <strong>2 ¡Ü N ¡Ü     10<sup>5</sup></strong>, the number of  fruits, <strong> 1 ¡Ü M ¡Ü     2*10<sup>5</sup></strong>, the number of edges and <strong>1 ¡Ü Q ¡Ü     3*10<sup>5</sup></strong>, the number of queries.</p>
<p>The next <strong>M</strong> lines will contain three integers <strong>0 ¡Ü a, b &lt;     N (a ¡Ù b)</strong>, the fruits which are connected by and edge and <strong>1 ¡Ü     X<sub>i</sub> ¡Ü 10<sup>5</sup></strong>.</p>
<p>The next <strong>Q</strong> lines will contain two integers <strong>0 ¡Ü a &lt;     N</strong>, the fruit Ada starts in and <strong>1 ¡Ü Y ¡Ü     10<sup>5</sup></strong>, her actual weigth.</p>
<p><strong>NOTE</strong> Multiedges are allowed.</p>
<h3>Output</h3>
<p>For each query, output the number of fruits Ada can get to.</p>
<h3>Example Input</h3>
<pre>4 4 3
1 2 4
2 3 3
3 0 4
0 1 3
1 3
1 4
1 5
</pre>
<h3>Example Output</h3>
<pre>4
2
1
</pre>
<h3>Example Input</h3>
<pre>8 10 8
1 3 3
1 2 2 
3 5 1
3 4 3
2 4 7
5 6 2
4 6 8
4 7 3
7 0 1
6 0 4
1 3
1 4
0 5
6 6
6 1
2 3
0 4
5 2
</pre>
<h3>Example Output</h3>
<pre>7
1
1
3
8
7
4
8
</pre>