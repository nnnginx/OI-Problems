There are <strong>N</strong> unique colors in the universe, numbered from <strong>1</strong> to <strong>N</strong>. George Michael wants to create a rainbow using these colors. The rainbow will consist of exactly <strong>M</strong> layers. For each layer, George Michael selects a color uniformly randomly from the <strong>N</strong> colors and colors the layer with it.

George Michael wonders what will be the probability that there will be at least <strong>K</strong> distinct colors in the rainbow after all the layers are colored in this way.

<br><br>

<h3>Input</h3>
The first line of the input contains an integer <strong>T</strong>, denoting the number of test cases. Each of the next <strong>T</strong> lines will contain three integers, <strong>N</strong>, <strong>M</strong> and <strong>K</strong>.

<br><br>

<h3>Constraints</h3>
<strong><li>1 ≤ T ≤ 20</li></strong>
<strong><li>1 ≤ N, M, K ≤ 2 * 10<sup>5</sup></li></strong>

<h3>Output</h3>
For each test case, print the case number and the probability that the rainbow will contain at least <strong>K</strong> distinct colors after all the layers are colored. Formally, let this probability be an irreducible fraction <strong>P / Q</strong>. Then you need to print <strong>(P * Q<sup>-1</sup>)</strong> modulo <strong>1000000007</strong>, where <strong>Q<sup>-1</sup></strong> is the modular inverse of <strong>Q</strong> modulo <strong>1000000007</strong>. You may safely assume that there will be a unique modular inverse of <strong>Q</strong> modulo <strong>1000000007</strong>.


<h3>Sample Input</h3>
<pre>3
1 1 1
2 2 2
4 2 2


</pre>

<h3>Sample Output</h3>
<pre>Case 1: 1
Case 2: 500000004
Case 3: 750000006

</pre>

<h3>Challenge(!)</h3>
<a href="https://www.spoj.com/problems/BANSTAND/">Colored Development</a>