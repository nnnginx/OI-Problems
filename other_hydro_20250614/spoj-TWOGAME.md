<p>Alice started playing a new simple game. &nbsp;She starts with the pair of integers (1, 1) and then she may a) duplicate one of the numbers or b) subtract the smaller number from the bigger one. &nbsp;So the game may proceed as follows: &nbsp;she starts with (1, 1), then she moves to (2, 1), then to (4, 1), then to (4, 2), then to (8, 2), then to (6, 2), etc.</p>
<p>She is now wondering if given an arbitrary pair of positive integers (A, B), will she be able to reach at this pair using the proceduce described above ?</p>
<h3>Input</h3>
<p>The first line contains a single positive integer T (T ¡Ü 500), denoting the number of test cases to solve. &nbsp;Each test case consists of a single line containing two positive integers A, B (A, B ¡Ü 10<sup>18</sup>).</p>
<h3>Output</h3>
<p>For each test case print a single line with the character Y if it is possible for Alice to reach the given pair or N if it is impossible.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3</pre>
<pre>6 2</pre>
<pre>5 1</pre>
<pre>3 3

<strong>Output:</strong>
Y
</pre>
<pre>Y</pre>
<pre>N</pre>