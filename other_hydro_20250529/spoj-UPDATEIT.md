<p>You have an array containing n elements initially all 0. You need to do a number of update operations on it. In each update you specify l, r and val which are the starting index, ending index and value to be added. After each update, you add the 'val' to all elements from index l to r. After 'u' updates are over, there will be q queries each containing an index for which you have to print the element at that index.</p>
<h3>Input</h3>
<p>First line consists of t, the number of test cases. (1 &lt;= t &lt;= 10)</p>
<p>Each test case consists of "n u",number of elements in the array and the number of update operations, in the first line (1 &lt;= n &lt;= 10000 and 1 &lt;= u &lt;= 100000)</p>
<p>Then follow u lines each of the format "l r val" (0 &lt;= l,r &lt; n, 0 &lt;= val &lt;=10000)</p>
<p>Next line contains q, the number of queries. (1 &lt;= q &lt;= 10000)</p>
<p>Next q lines contain an index (0 &lt;= index &lt; n)</p>
<h3>Output</h3>
<p>For each test case, output the answers to the corresponding queries in separate lines.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>5 3<br>0 1 7<br>2 4 6<br>1 3 2<br>3<br>0<br>3<br>4<br><strong><br>Output:<br></strong>7<br>8<br>6
</pre>