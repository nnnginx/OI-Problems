<p>You will be given a 2-dimensional grid of letters. Find the length of the longest path of consecutive letters, starting at 'A'. Paths can step from one letter in the grid to any adjacent letter (horizontally, vertically, or diagonally).</p>
<p>For example, in the following grid, there are several paths from 'A' to 'D', but none from 'A' to 'E':</p>
<div><img title="ABC" src="../../../content/simes:ABCPATH-1.png" alt="ABC" width="162" height="108"></div>
<p>One such path is:</p>
<p><img title="ABC path" src="../../../content/simes:ABCPATH-2.png" alt="path" width="163" height="108"></p>
<h3>Input</h3>
<p>Each test case will start with a line contains two integers H, W the height and width of the grid respectively 1 &lt;= H, W &lt;= 50. Then H lines follow each of W uppercase letters only. Input terminates with H = 0 and W = 0.</p>
<h3>Output</h3>
<p>For each test case print <tt>¡°Case C: X¡±</tt> without quotes where C is the case number starting with 1 and X is the solution.</p>
<h3>Example</h3>
<pre><strong>Sample Input:</strong>
4 3
ABE
CFG
BDH
ABC
0 0

<strong>Sample Output:</strong>
Case 1: 4</pre>
<!-- Note: The underscore '_' symbol is only for clarity you should print space instead. -->