<p>Mr. B has recently discovered the grid named "spiral grid". Construct the grid like the following figure. (The grid is actually infinite. The figure is only a small part of it.)</p>
<p><img src="../../../content/john_jones:spiralgr1.jpg" alt=""></p>
<p>Considering traveling around it, you are free to any cell containing a composite number or 1, but traveling to any cell containing a prime number is disallowed. You can travel up, down, left or right, but not diagonally. Write a program to find the length of the shortest path between pairs of nonprime numbers, or report it's impossible.</p>
<p><img src="../../../content/john_jones:spiralgr2.jpg" alt=""></p>
<h3>Input</h3>
<p>Each test case is described by a line of input containing two nonprime integer 1 &lt;=<strong>x</strong>, <strong>y</strong>&lt;=10,000.</p>
<h3>Output</h3>
<p>For each test case display its case number followed by the length of the shortest path or <strong>impossible</strong> in one line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 4
9 32
10 12

<strong>Output:</strong>
Case 1: 1
Case 2: 7
Case 3: impossible
</pre>