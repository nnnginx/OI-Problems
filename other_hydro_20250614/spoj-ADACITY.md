<p>Ada the Ladybug and her friends are on trip in Bugraine. Most of them are in different cities at the moment. They want to spread as much as possible, make hologram-skype to show all others the city. They have agreed, to make this call in time <strong>T</strong>.</p>
<p>The cities are connected with bi-directional roads. Each of the road has some length (which equals to time it takes to travel between two cities).</p>
<h3>Input</h3>
<p>The first line will contain the number of test-cases.</p>
<p>The first line of each test-case begins with four integers: <strong>N,M,F,T</strong>, number of cities, number of roads, number of friends (Ada inclusive) and time they have: <strong>1 ¡Ü N,F ¡Ü 500</strong>, <strong> 0 ¡Ü M ¡Ü 10<sup>5</sup>, 0 ¡Ü T ¡Ü     5*10<sup>8</sup></strong></p>
<p>Then a line with <strong>F</strong> integers follows, <strong> 1 ¡Ü H<sub>i</sub> ¡Ü     N</strong>, the city, where <strong>i</strong><sup>th</sup> friend currently is.</p>
<p>Afterward <strong>M</strong> lines follow, with three integers <strong>A,B,L</strong>, <strong>1 ¡Ü     A,B ¡Ü N, 1 ¡Ü L ¡Ü 10<sup>6</sup></strong>, indicating a road, which connect cities <strong>A,B</strong> with length of <strong>L</strong></p>
<p>PS: There might exist multiple roads between two cities and there might also be a "circular route" which begins and ends in the same city!</p>
<h3>Output</h3>
<p>For each test-case, print maximal number of different cities Ada and her friends can end up at after <strong>T</strong> time!</p>
<h3>Example Input</h3>
<pre>3
5 5 4 3
1 1 1 1
1 2 3
1 5 2
5 4 2
4 3 1
2 3 2
7 7 6 3
6 6 2 2 2 2
1 7 5
1 2 5
7 2 4
2 3 2
3 4 3
5 4 1
2 5 2
5 5 4 4
1 1 1 1
1 2 3
1 5 2
5 4 2
4 3 1
2 3 2


</pre>
<h3>Example Output</h3>
<pre>3
5
4
</pre>
<h3>Output Explanation</h3>
<p>In <strong>first</strong> test-case, all 4 friends begin in same node. From this node, one can get to nodes <strong>2</strong> and <strong>5</strong>, or stay in the node (in time ¡Ü 3). Since everyone is in node 1, best they can do is to choose one friend who goes to 5, one who goes to 2 and the rest of them can stay so with "1,1,2,5" they can occupy 3 different nodes (at most).</p>
<p>In <strong>second</strong> test-case, friends on <strong>6</strong> can go nowhere (just stay in 6). Friends on 2 can go to <strong>3,4,5</strong> or stay on <strong>2</strong>. So with friends in <strong>6,6,2,3,4,5</strong> we get maximum of 5 different cities.</p>
<p>Last (<strong>third</strong>) test-case is same as first - except for time. This one additional time-unit will let friends go to <strong>4</strong> (or to nodes which they can go in first test-case). "1,2,4,5" would make 4 different cities!</p>