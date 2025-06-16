<p>Chintu and his father Nikka, on their vacations, went to The Amazing Maze. But unfortunately, Chintu is has been separated from his father. His father Nikka has to find him as soon as possible in the maze or else Chintu will start crying soon.</p>
<p>The Amazing Maze is actually pretty amazing! The maze is built in a rectangular grid fashion. There are walls (#) and walking cells (.) in the grid. One can only walk through walking cells and so cannot jump off the wall. The amazing part is that each wall becomes a walking cell at some point of time (Neglect the transition time). Alternatively one can say that at some time t1 units, the wall will become walking cell and so one can step on to it at t1 time <strong>and at any time after t1</strong>. One can only move to adjacent walking cells from a walking cell. Adjacent cells mean the immediate up, down, right and left walking cells. It takes 1 unit of time to go from current cell to any adjacent cell. One can also wait on a particular walking cell for an adjacent wall to become a walking cell.</p>
<p>Nikka has the map of the maze with the information of the time at which the walls becomes walking cells. <strong>Also he knows at which walking cell he is situated and at which walking cell Chintu is situated.</strong> Help Nikka find out the minimum time required to reach to his son Chintu.</p>
<h3>Input</h3>
<p>First line contains T, the number of test cases.</p>
<p>Each case begins with two integers, M and N, the dimensions of maze.</p>
<p>Next contains M lines each containing N characters. Each character is either a ¡°#¡± or a ¡°.¡± as described above. This maze is the snapshot at time t=0.</p>
<p>Next M lines contain N space separated non negative integers. For each ¡°.¡±, there will be a 0 and for each ¡°#¡±, there will be a positive integer which represent the time at which that wall (#) will become a walkable cell.</p>
<p>Next line contains x1 and y1 denoting the position of Nikka in the maze.</p>
<p>Next line contains x2 and y2 denoting the position of Chintu in the maze.</p>
<h3>Output</h3>
<p>Output T lines each containing an integer, the minimum time required for Nikka to reach Chintu.</p>
<h3>Constraints</h3>
<p>1&lt;=T&lt;=10 <br> 1&lt;=M&lt;=200<br> 1&lt;=N&lt;=200<br> 0&lt;=x1, x2&lt;M<br> 0&lt;=y1, y2&lt;N</p>
<p>For all #¡¯s, time ¡°t¡± will be &gt; 0 and &lt;= 10^4.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>2</p><p>1 5</p><p>..#..</p><p>0 0 1 0 0</p><p>0 0</p><p>0 4</p><p>3 3</p><p>.##</p><p>##.</p><p>##.</p><p>0 1 2</p><p>3 4 0</p><p>6 7 0</p><p>0 0</p>2 2

<strong>Output:</strong>
4
</pre>
<pre>4</pre>