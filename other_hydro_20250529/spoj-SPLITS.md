<p>Little Petar has been put in charge of maintaining an unpredictable array of strings. Initially, all of the array elements were the same string S, but the array is prone to change; and there is exactly one kind of change that may happen. This is a <strong>split</strong>&nbsp;operation at a given location, X; after it is performed, the location X maintains the string it had before, however all fields to the left and all fields to the right of X containing the same string as X will be given new strings, S<sub>1</sub>&nbsp;and S<sub>2</sub>.</p>
<p>At certain points in time, Petar will be asked to give the string at a given location. He asked you for help.</p>
<h3>Input</h3>
<p>The first line of the standard input contains two numbers, N and Q, the size of the array and the total number of operations and queries, respectively.</p>
<p>The second line contains the string S, the string initially contained within each location of the array.</p>
<p>The following Q lines contain the description of either an operation or a query:</p>
<p>A split operation is represented as "SPLIT X S<sub>1</sub>&nbsp;S<sub>2</sub>", implying that the fields to the left of X, containing the same string as at X, will from now on have the string S<sub>1</sub>, and fields to the right will have the string S<sub>2</sub>.</p>
<p>A query is represented as "QUERY X", implying that Petar is asked to give the string at location X.</p>
<h3>Output</h3>
<p>For each QUERY command given, output a new line containing the string currently located on the given position.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>6 6<br>picsel<br>SPLIT 3 petarv duxserbia<br>SPLIT 5 sasav nikolaj<br>QUERY 1<br>QUERY 3<br>QUERY 5<br>QUERY 6</pre>
<pre><strong>Output:<br></strong>petarv<br>picsel<br>duxserbia<br>nikolaj</pre>
<h3>Explanation</h3>
<p>Initially, the string picsel is located throughout the array. After the first and second split operation, respectively, the array looks as follows:</p>
<p>[petarv, petarv, picsel, duxserbia, duxserbia, duxserbia]</p>
<p>[petarv, petarv, picsel, sasav, duxserbia, nikolaj]</p>
<p>The answers to the queries then clearly follow from the final state of the array.</p>
<h3>Constraints</h3>
<ul>
<li>1 &lt;= N, Q &lt;= 10<sup>5</sup></li>
<li>1 &lt;= X &lt;= N</li>
<li>1 &lt;= |S|, |S<sub>1</sub>|, |S<sub>2</sub>| &lt;= 50</li>
<li>The strings will consist solely of lowercase letters of the English alphabet.</li>
<li>All strings appearing in the operations will be unique.</li>
</ul>