<p><img src="/content/ahven:tower.png" style="float: right" hspace="5">Apart from the Hanging Gardens the Babylonians (around 3000-539 b.c.) built the Tower of Babylon as well. The tower was meant to reach the sky, but the project failed because of a confusion of language imposed from much higher above.</p>
<p>For the 2638th anniversary a model of the tower will be rebuilt. <i>n</i> different types of blocks are available. Each one of them may be duplicated as many times as you like. Each type has a height <i>y</i>, a width <i>x</i> and a depth <i>z</i>. The blocks are to be stacked one upon eachother so that the resulting tower is as high as possible. Of course the blocks can be rotated as desired before stacking. However for reasons of stability a block can only be stacked upon another if <i>both</i> of its baselines are shorter.</p>

<h3>Input</h3>
<p>The number of types of blocks <i>n</i> is located in the first line of each test case. On the subsequent <i>n</i> lines the height <i>y<sub>i</sub></i>, the width <i>x<sub>i</sub></i> and the depth <i>z<sub>i</sub></i> of each type of blocks are given. There are never more than 30 different types available.</p>
<p>There are many test cases, which come one by one. Input terminates with n = 0.</p>

<p><strong>Edited:</strong> You can assume that max(<i>x<sub>i</sub></i>, <i>y<sub>i</sub></i>, <i>z<sub>i</sub></i>) &lt;= 2500.</p>

<h3>Output</h3>
<p>For each test case your program should output one line with the height of the highest possible tower.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
5
31 41 59
26 53 58
97 93 23
84 62 64
33 83 27
1
1 1 1
0

<b><tt>Sample output:</tt></b>
342
1
</pre>