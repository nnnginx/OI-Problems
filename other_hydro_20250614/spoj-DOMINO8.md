<p>Mirko received an N × N table for his birthday, where a non-negative integer is written in each field</p>
<p>of the table. Unfortunately, the written numbers are too large for Mirko’s taste, so he will place K</p>
<p>dominoes on top of the table that will cover the fields that are too large.</p>
<p>More precisely, Mirko places the dominoes according to the following rules:</p>
<p>• each domino covers two fields of the table that are adjacent in a row or in a column,</p>
<p>• the dominoes do not overlap (but can touch),</p>
<p>• the sum of all visible (uncovered) fields needs to be as small as possible.</p>
<p>It is your task to determine the required minimal sum of visible fields. The test data will be such that</p>
<p>it will always be possible to place K dominoes without overlapping..</p>
<h3>Input</h3>
<p>The first line of input contains the integers N (1 &lt;= N &lt;= 2000), the dimensions of the table, and K</p>
<p>(1 &lt;= K &lt;= 8), the number of dominoes. Each of the following N lines contains N integers from</p>
<p>the interval [0, 1000]. These N × N numbers describe Mirko’s table</p>
<h3>Output</h3>
<p>The first and only line of output must contain the minimal sum of visible fields after covering the</p>
<p>table with dominoes.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 1</pre>
<pre>2 7 6</pre>
<pre>9 5 1</pre>
<pre>4 3 8
<strong>Output:</strong>
31</pre>
<pre><strong><br></strong></pre>
<pre><strong>Input:</strong></pre>
<pre>4 2</pre>
<pre>1 2 4 0</pre>
<pre>4 0 5 4</pre>
<pre>0 3 5 1</pre>
<pre>1 0 4 1</pre>
<pre><span style="font-weight: bold;">Output:</span></pre>
<pre>17</pre>
<pre><strong>Clarification of the first example:</strong> We place the domino so it covers fields with numbers 9 and 5.&nbsp;</pre>
<pre><strong>Clarification of the second example:</strong> We place the dominoes so they cover fields [4, 5] and [5, 4] in the third column.</pre>