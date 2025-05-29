<p>MegaCity of the future is a rectangular grid of streets. Each intersection has integer Cartesian coordinates x and y. To get from intersection a with coordinates x<sub>a</sub>, y<sub>a</sub> to intersection b with coordinates x<sub>b</sub>, y<sub>b</sub> you need to drive exactly | x<sub>a</sub> - x<sub>b</sub> | + | y<sub>a</sub> - y<sub>b</sub> | blocks. Usually, it takes 10 time units to drive one block, so one can easily compute the time it takes to get from a to b. However, traffic jams that occur in MegaCity turn estimation of minimal driving time into a complex problem that you have to solve.</p>
<p>Traffic jams in MegaCity affect a rectangular area that is specified by coordinates of its bottom-left and top-right corners. The time to travel one block in the traffic jam is specified. All streets that are strictly inside the rectangular region are affected by the traffic jam. Sometimes, it is better to drive around the traffic jams to save time, but sometimes it is better to drive through some traffic jams as shown in the example - 17 blocks are driven outside of traffic jams, taking 10 time units per block, and 2 blocks in the light traffic jam with 11 time units per block.</p>
<p><img src="./22234/file/AQihh0A2.png" alt=""></p>
<h3>Input</h3>
<p>Multiple test cases. The number of them is given in the very first line. For each test case:</p>
<p>The first line contains four integer numbers x<sub>a</sub>, y<sub>a</sub>, x<sub>b</sub> and y<sub>b</sub>, coordinates of the start and finish intersections. The second line contains a single integer number n (0 &lt;= n &lt;= 1000) which specifies the number of traffic jams. The following n lines describe traffic jams. Each traffic jam is described by five integer numbers x<sub>1,i</sub>, y<sub>1,i</sub>, x<sub>2,i</sub>, y<sub>2,i</sub> and t<sub>i</sub>, where first four numbers are coordinates of the bottom-left and top-right corners of the jammed area (x<sub>1,i</sub> &lt; x<sub>2,i</sub>, y<sub>1,i</sub> &lt; y<sub>2,i</sub>), and t<sub>i</sub> (10 &lt; t<sub>i</sub> &lt;= 10<sup>8</sup>) is the time it takes to travel one block inside this traffic jam. All coordinates are from 0 to 10<sup>8</sup> inclusive. Areas of traffic jams neither intersect nor touch each other. Start and finish points are different and do not lie inside nor on the border of any traffic jam.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>A single integer - the minimal driving time from intersection a to intersection b.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
1 6 15 3
4
2 1 3 7 44
5 2 10 4 33
8 5 11 9 22
12 1 14 8 11

<strong>Output:</strong>
192
</pre>
<p><strong>Warning: A naive algorithm may not run in time!</strong></p>