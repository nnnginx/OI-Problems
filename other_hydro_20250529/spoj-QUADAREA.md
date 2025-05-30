<p>You are trying to build a house, but unfortunately you currently have only four available walls with side lengths a, b, c, and d. You want your house to be as big as possible, so you would like to know the largest possible area of any quadrilateral you can construct with these four side lengths.</p>

<h3>Input</h3>
<p>The first line contains the integer T (1 �� T �� 2,000), the number of tests. Each test contains a single line with four real numbers: a, b, c, and d (0 &lt; a, b, c, d &lt; 1,000). Note that it will always be possible to form a valid quadrilateral with these lengths; that is, the sum of any three side lengths will be strictly larger than the other one.</p>

<h3>Output</h3>
<p>For each test case, print a single line containing the largest possible area. Your output will be accepted if it is within 0.01 of the official answer.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
1 2 1 2
0.5 0.5 0.5 0.5

<b>Output:</b>
2.00
0.25
</pre>

<p>For the first test case, it is optimal to construct a rectangle, and for the second, a square is optimal.</p>