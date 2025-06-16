<p>There is a long gap with fixed width of 1 unit in the ground with <strong>N + 1&nbsp;</strong>vertices, which is composed of <strong>N</strong>&nbsp;segments with same width. A segment&nbsp;connects to at most one segment on its head and tail vertically or horizontally, that is, it can connect to at most two segments. The long gap formed by those segments is simply a open polyline. Duck doesn't like the gap, he is given a set of tiles and wants to know if the long gap can be tiled by the limited number of tiles. There are <strong>M</strong> distinct tiles, each with <strong>K<sub>i</sub></strong>&nbsp;and has <strong>C<sub>i</sub>&nbsp;</strong>segments. It is not necessary to use all tiles, and Duck can rotate the tile to fill the gap. It is guaranteed that both long gap and tiles are open polyline with fixed width of 1 unit. Can you help him check if he is possible to do so.</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>. (1 ¡Ü T ¡Ü 25)</p>
<p>For each test case, it starts with the number of segments of the long gap <strong>N</strong>. (1 ¡Ü N ¡Ü 20)</p>
<p>Following N lines, each consisting of one uppercase character <strong>W1<sub>i</sub></strong>, either up (U), down(D), left(L) or right(R), and one integer <strong>F1<sub>i</sub></strong>, indicating the direction to turn to and the length of that segment. (1 ¡Ü ¡Æ<sup>n</sup><sub>i=1 </sub>F1<sub>i</sub><sub> </sub>¡Ü 100)</p>
<p>Next line is the number of distinct tiles <strong>M</strong>. (1 ¡Ü M ¡Ü 15)</p>
<p>For each distinct tile, it starts with two integers, the available amount of that tile <strong>K<sub>i</sub></strong> and number of segments&nbsp;<strong>C<sub>i</sub></strong>. (1 ¡Ü K<sub>i</sub>, ¡Æ<sup>M</sup><sub>i=1 </sub>K<sub>i</sub>&nbsp;¡Ü 15, 1 ¡Ü C<sub>i</sub> ¡Ü 20)</p>
<p>Following C<sub>i</sub> lines, same as above, one uppercase character <strong>W2<sub>i</sub></strong> and one integer&nbsp;<strong>F2<sub>i</sub></strong> indicating the direction and the length of that segment.</p>
<h3>Output</h3>
<p>If it is possible to tile the gap with given tiles, print "YES", else "NO". (without quotes)</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
16
L 4
U 2
L 7
U 2
L 4
D 4
R 2
D 2
L 3
D 2
R 6
U 1
R 2
D 4
L 3
U 1
7
2 5
D 6
L 2
U 3
L 2
D 2
1 2
D 7
L 2
2 2
D 2
R 2
1 1
R 8
3 1
U 3
4 1
D 4
2 2
R 3
U 1

2
R 6
U 2
2
1 2
D 3
L 2
1 1
U 2

<strong>Output:</strong>
YES
NO
</pre>
<h3>Explanation</h3>
<p><img src="file://mSHJ0NSW.png" alt="" width="797" height="452"></p>