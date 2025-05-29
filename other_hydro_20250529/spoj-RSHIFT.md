<p>All the numbers in a computer is represented as 64-bit 2's complement form.</p>
<p>You have to write a program to perform the following task :-</p>
<ul>
<li>Read the number (given in decimal form).</li>
<li>Shift all the bits towards right (the first bit is removed), i.e the second bit from right is shifted to first position, third to second and so on.</li>
<li>Add a zero to the last position.</li>
<li>Write the result back in decimal form</li>
</ul>
<p>&nbsp;</p>
<p>For example 10 is represented as:</p>
<p>0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 1010</p>
<p>After step 2 the result is:</p>
<p>_000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0101</p>
<p>After step 3 the result is:</p>
<p>0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0000 0101</p>
<p>Finally the output is: 5</p>
<h3>Input</h3>
<p>The first line contains <strong>T </strong>representing the number of test cases (T&lt;=500000). Then T lines follows each containing a input number.</p>
<h3>Output</h3>
<p>Print T lines, each containing the result of each test case.</p>
<h3>Constraints</h3>
<p>All input and output numbers will fit in signed 64-bit integer. Large I/O. A fast code written in fast language is likely to pass.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><table border="0"><tbody><tr><td>5<br>1<br>2<br>3<br>4<br>5</td></tr></tbody></table></pre>
<pre><strong>Output:</strong></pre>
<pre><table border="0"><tbody><tr><td>0<br>1<br>1<br>2<br>2</td></tr></tbody></table></pre>