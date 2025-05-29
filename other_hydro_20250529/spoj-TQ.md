<p>Little Yuan is two years old and she is learning about some triangles and quadrangles. She is such a smart girl that she soon realizes two triangles can form a quadrangle <strong>without overlapping each other</strong>. She picks up a lot of triangles and uses them to form some quadrangles. Unfortunately, she is not good at this kind of jigsaw game and makes some mistakes.</p>
<p>As her brother, you are curious about whether she has made a mistake when forming two triangles into a quadrangle. You are thinking about to write a program to determine it.</p>
<p><strong>Notice that the quadrangle in this problem is defined as a simple polygon with four vertexes. And you may also assume that all triangles and quadrangle have positive area.</strong></p>
<p>Note that two graphs are considered as the same if and only if they can overlap completely by <strong>shifting, rotation and flipping</strong>.</p>
<h3>Input</h3>
<p>There are multiple test cases. The first line of input contains a single integer T denoting the number of test cases. (T &lt; 1000)</p>
<p>For each test case, there are 10 lines in total.The first 3*2 lines describe the two triangles. Each line with two numbers denotes the coordinates of a point.The next 4 lines describe the quadrangle in clockwise order or counter-clockwise order.</p>
<p>All coordinates are integers and less than 15000 in absolute value.</p>
<h3>Output</h3>
<p>For each test case, output <strong>Yes</strong> if the given triangles can form the given quadrangle&nbsp;without overlapping, <strong>No</strong> otherwise. See the example for more output format details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
0 0
0 1
1 0
0 0
0 1
1 0
-1 0
0 0
1 0
0 1
0 0
-1 1
1 0
0 0
0 1
1 0
-1 0
0 0
1 0
0 1

<strong>Output:</strong>
Case #1: Yes
Case #2: No
</pre>
<p><em>This problem is first solved by team</em> <strong>FreeJourney</strong> (Wuhan University)<em> at 83 minutes after the onsite contest starts.</em></p>
<p>The test set of this problem is not the same as that of the onsite contest.</p>