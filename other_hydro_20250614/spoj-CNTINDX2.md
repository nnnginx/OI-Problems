<p>Let's deal with an array again, the most important data structure of computer science. You will be given an array. Now you have some operations to do. There will be three types of operations:</p>
<ul>
<li>Type 1: Insert a number after a given index</li>
<li>Type 2: Change the value of an index.</li>
<li>Type 3: You will get a number and two indices i &amp; j where i &lt;= j.</li>
</ul>
<p>Now you will have to answer how many time the number appears in the array starting from i to j.</p>

<h3>Input</h3>
<p>Each file contains one test case.</p>
<p>The first line contains and integer N, the number of initial array elements (1 &lt;= N &lt;= 100000) &amp; Q, the number of Queries (1 &lt;= Q &lt;= 100000). Second line contains N integers each in the range from 1 to 100000. Each of the next Q lines contains an opeation. The operations will appear as the formats below:</p>

<ul>
<li>1 x y, where 1 &lt;= x &lt;= length of the array, which means you have to insert number y after the index x.</li>
<li>2 x y, For this operation, you have to change the value of index x to value y.</li>
<li>3 i j x, Here, you have to find how many times x appers in the array from i to j. Here x will always be present in the array and 1 &lt;= i &lt;= j &lt;= length the array.</li>
</ul>

<h3>Output</h3>
<p>For each operation of 3rd type, output the required answer in separated line.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
5 3<br>42 18468 6335 26501 19170<br>2 4 29359<br>2 5 5706<br>3 2 5 5706</pre>

<pre><strong>Output:</strong>
1
</pre>