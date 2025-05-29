<p>Almost Prime Numbers are composite numbers which are not divisible by certain prime numbers. Given K prime numbers and an integer N, find out the number of Almost Prime Numbers (ie. composite numbers not divisible by any of the given K prime numbers) that are not greater than N.</p>
<h3>Input</h3>
<p>First line of input consists of an integer <strong>T (1&lt;=T&lt;=1000)</strong>, denoting the number of test cases. Then <strong>T</strong> test cases follow. Each case begins with a line containing two integers <strong>N (0&lt;=N&lt;=10^6)</strong> and <strong>K (1&lt;=K&lt;=10)</strong>. The next line contains <strong>K</strong> space separated prime numbers. All the prime numbers are guaranteed to be <strong>less than 50</strong>.</p>
<h3>Output</h3>
<p>For each test case, output a single line in the format <strong>Case X: Y</strong>, where <strong>X</strong> denotes the test case number and <strong>Y</strong> denotes the number of Almost Prime Numbers that are not greater than N.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
1000 3
2 3 5
49 3
2 3 5</pre>
<pre><strong>Output:</strong>
Case 1: 100
Case 2: 1</pre>