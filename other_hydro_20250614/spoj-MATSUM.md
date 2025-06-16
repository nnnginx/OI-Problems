<p>A N ¡Á N matrix is filled with numbers.  BuggyD is analyzing the matrix, and he wants the sum of certain submatrices every now and then, so he wants a system where he can get his results from a query.  Also, the matrix is dynamic, and the value of any cell can be changed with a command in such a system.</p>

<p>Assume that initially, all the cells of the matrix are filled with 0.  Design such a system for BuggyD.  Read the input format for further details.</p>

<h3>Input</h3>
<p>The first line of the input contains an integer <b>t</b>, the number of test cases.  <b>t</b> test cases follow.</p>

<p>The first line of each test case contains a single integer <b>N</b> (1 &lt;= <b>N</b> &lt;= 1024), denoting the size of the matrix.
</p><p>A list of commands follows, which will be in one of the following three formats (quotes are for clarity):</p>

<ol>
<li><tt>"SET x y num"</tt> - Set the value at cell (x, y) to num (0 &lt;= x, y &lt; <b>N</b>).</li>
<li><tt>"SUM x1 y1 x2 y2"</tt> - Find and print the sum of the values in the rectangle from (x1, y1) to (x2, y2), inclusive.  You may assume that x1 &lt;= x2 and y1 &lt;= y2, and that the result will fit in a signed 32-bit integer.</li>
<li><tt>"END"</tt> - Indicates the end of the test case.</li>
</ol>

<h3>Output</h3>
<p>For each test case, output one line for the answer to each "SUM" command.  Print a blank line after each test case.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
4
SET 0 0 1
SUM 0 0 3 3
SET 2 2 12
SUM 2 2 2 2
SUM 2 2 3 3
SUM 0 0 2 2
END

<b>Output:</b>
1
12
12
13
</pre>

<center><b>Warning: large Input/Output data, be careful with certain languages</b></center>