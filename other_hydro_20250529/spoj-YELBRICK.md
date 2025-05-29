<p>
After Dorothy¡¯s memorable adventure in the Land of Oz, traffic along the Yellow Brick Road got really intense, making some sections of it nearly impossible to cross because of the holes along the road. The Land of Oz engineers are having trouble to pave this road, because the yellow stone is in short supply, forcing them to buy stones from different suppliers. As you already know, every road in the Land of Oz must be built using bricks that are perfect and identical cubes. To maximize the durability of the road, it also must be built using the least number of bricks possible. The problem is that each supplier provides stones of different sizes, that must be cut in order to make the bricks for the road.
</p>

<p>
Can you help the engineers to find which is the best brick size to use to maximize the road durability ?
</p>

<h3>Input</h3>
<p>Each test case is given using several lines. The first line contains an integer N representing the number of different suppliers of yellow stone (2 ¡Ü N ¡Ü 1000). For simplicity, we assume that the engineers will buy exactly one stone from each supplier. Each of the next N lines contains three integers Ai, Bi, Ci (0 &lt; Ai, Bi, Ci ¡Ü 1000, 1 ¡Ü i ¡Ü N) that describe, respectively, the width, height and depth of each stone provided by the i-th supplier. The last test case is followed by a line containing one zero.</p>

<h3>Output</h3>
<p>For each test case, print one line containing the minimum number of identical cubes that can be cut from the given stones.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
1 2 3
4 5 6
2
4 4 4
2 2 2
0

<strong>Output:</strong>
126
9
</pre>