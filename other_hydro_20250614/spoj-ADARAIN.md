<p> Ada the Ladybug is currently growing plants. She has a very long furrow, in
which she does so. It is so long, that most of water falling from rains drops
just onto a part (segment) of the furrow. Ada doesn't want the plants to
wither, so she records all rains to know, how much water every particular plant
got. Sadly, there are so many rains that she couldn't handle
this alone!</p>

<p> At first, you will be given <b>N</b> queries with <b>[L,R]</b> segments
telling you, where all of the <b>N</b> rains fallen. Afterward <b>M</b> queries
follows, with number <b>i</b> - the i-th plant for which you want to know, the
number of rains, which has fallen onto it.

</p><h3>Input</h3>
The first line will contain <b>0&lt; N,M ¡Ü 10<sup>5</sup></b>,<b>0&lt; W ¡Ü 10<sup>6</sup></b>, number of
rains, number of questions and size of furrow respectively.
<p>Then <b>N</b> lines follow, each containing two integers
<b>0 ¡Ü L ¡Ü R &lt;W</b>, symbolizing left and right plant in segment on which
i-th rain has fallen.</p>
<p>Afterward <b>M</b> lines follow, each containing a number
<b>0 ¡Ü a &lt; W</b>, asking for number of rains which has fallen on plant number
<b>a</b></p>

<h3>Output</h3>
Print <b>M</b> lines (for each query of second type), with integer indicating
number of rains, which has fallen on the plant in query.

<h3>Example Input</h3>
<pre>6 7 10
0 9
3 5
4 6
4 8
1 8
5 5
1
5
9
4
9
6
7
</pre>
<h3>Example Output</h3>
<pre>2
6
1
5
1
4
3
</pre>