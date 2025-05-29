<p>There are <strong>N</strong> cities numbered from 1 to N, connected by <strong>M</strong> flights. Note that a flight from city 1 to 2 doesn't necessarily mean there is a flight from 2 to 1, and some cities may not be connected by any flights. Also, there is at most one directed flight from one city to another one. The i-th flight connects city <strong>U<sub>i</sub></strong> with city <strong>V<sub>i</sub></strong>, takes <strong>W<sub>i</sub></strong>&nbsp;seconds, plus a constraint: the current accumulated travel time cannot exceed <strong>L<sub>i</sub></strong>&nbsp;when you are in U<sub>i</sub>&nbsp;and plan to go to V<sub>i</sub>&nbsp;from there<sub>&nbsp;</sub>for health reason.</p>
<p>Duck wants to travel, but he will be very tired if he takes too many flights! Therefore, he doesn't want to take more than <strong>K</strong> flights. Can you find out the shortest travel time for all pairs of cities by not taking more than K flights and following the accumulated travel time constraint of each flight?</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>.&nbsp; (1 ¡Ü T ¡Ü 20)</p>
<p>For each test case, it starts with <strong>N</strong>, <strong>M</strong>, <strong>K</strong>. (2 ¡Ü N ¡Ü 50, 0 ¡Ü M ¡Ü N ¡Á&nbsp;(N - 1), 1 ¡Ü K ¡Ü N - 1)</p>
<p>Following M lines, each consisting <strong>U<sub>i</sub></strong>, <strong>V<sub>i</sub></strong>, <strong>W<sub>i</sub></strong>, <strong>L<sub>i</sub></strong>. (1 ¡Ü U<sub>i</sub>, V<sub>i</sub> ¡Ü N where U<sub>i</sub> ¡Ù V<sub>i</sub>, 1 ¡Ü W<sub>i</sub> ¡Ü 10<sup>4</sup>, 1 ¡Ü L<sub>i</sub> ¡Ü 10<sup>4</sup> ¡Á 50)</p>
<h3>Output</h3>
<p>Output a N ¡Á N distance matrix, printing out the shortest travel time for all pairs of cities. If one city is not reachable from one city, print out -1 instead.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
8 15 3
1 2 4 10
1 7 7 28
1 8 4 27
2 3 9 34
2 6 6 14
2 7 8 7
2 8 1 12
3 5 10 24
5 3 8 39
5 4 6 28
5 6 5 11
6 5 6 9
7 2 4 6
7 6 7 12
8 3 3 3

6 9 5
1 2 10 31 
1 3 14 58
1 5 23 24
3 1 12 12
3 2 4 19
4 1 20 53
4 5 25 47
5 4 13 47
6 2 4 39

<strong>Output:</strong>
0 4 13 -1 23 10 7 4 
-1 0 4 18 12 6 8 1 
-1 -1 0 16 10 15 -1 -1 
-1 -1 -1 0 -1 -1 -1 -1 
-1 -1 8 6 0 5 -1 -1 
-1 -1 14 12 6 0 -1 -1 
-1 4 13 19 13 7 0 5 
-1 -1 3 19 13 -1 -1 0 
0 10 14 36 23 -1 
-1 0 -1 -1 -1 -1 
12 4 0 48 35 -1 
20 30 34 0 25 -1 
33 -1 47 13 0 -1 
-1 4 -1 -1 -1 0
</pre>
<h3>Explanation</h3>
<p><img src="file://fRLtAVbD.png" alt="" width="904" height="471"></p>
<p>Select some results to explain, won't go through all..</p>
<p>In case 1, 1 -&gt; 3 is 13 through 2, rather than 7 through 8 because&nbsp; 1 -&gt; 8 is 4, and 8 to 3 has a accumulated time constraint which is 3.<br> 8 -&gt; 6 is not reachable although there is exactly one path connecting them and within K, the constraint of 5 -&gt; 6 is 11, which is larger than accumulated time of 13.</p>
<p>In case 2, 5 -&gt; 2 is not reachable. Only one path connecting 5 to 1 which takes 33. From 1 -&gt; 2 the shortest time is 10 but its constraint is 31 which is larger than 33. So we pass through 3 instead and the total time becomes 47. Unluckily the constraint of 3 -&gt; 2 also limits the reachability.</p>