<p>Farmer John has challenged Bessie to the following game: FJ has a board with dots marked at N (2 ≤ N ≤ 200) distinct lattice points. Dot i has the integer coordinates X<sub>i</sub> and Y<sub>i</sub> (-1,000 ≤ X<sub>i</sub>, Y<sub>i</sub> ≤ 1,000).</p>

<p>Bessie can score a point in the game by picking two of the dots and drawing a straight line between them; however, she is not allowed to draw a line if she has already drawn another line parallel to it. Bessie would like to know her chances of winning, so she has asked you to help find the maximum score she can obtain.</p>

<h3>Input</h3>
<p>There will be multiple test cases. For each case, the first line contains the integer N, and each of the next N lines gives a pair of integers, X<sub>i</sub> and Y<sub>i</sub>. The file ends with the case N = 0, which should not be processed.</p>

<h3>Output</h3>
<p>For each test case, print a single integer representing the maximum number of lines Bessie can draw, no two of which are parallel.</p>

<h3>Example</h3>

<pre><b>Input:</b>
4
-1 1
-2 0
0 0
1 1
0

<b>Output:</b>
4
</pre>

<p>Bessie can draw lines of the following four slopes: -1, 0, ⅓, and 1.</p>