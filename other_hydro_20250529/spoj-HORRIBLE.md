<p>World is getting more evil and it's getting tougher to get into the Evil League of Evil. Since the legendary Bad Horse has retired, now you have to correctly answer the evil questions of Dr. Horrible, who has a PhD in horribleness (but not in Computer Science). You are given an array of <strong>N</strong> elements, which are initially all 0. After that you will be given <strong>C</strong> commands. They are -</p>
<p>* <strong>0 p q v</strong> - you have to add <strong>v</strong> to all numbers in the range of <strong>p</strong> to <strong>q</strong> (inclusive), where <strong>p</strong> and <strong>q</strong> are two indexes of the array.</p>
<p>* <strong>1 p q</strong> - output a line containing a single integer which is the sum of all the array elements between <strong>p</strong> and <strong>q </strong>(inclusive)</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>In the first line you'll be given <strong>T</strong>, number of test cases.</p>
<p>Each test case will start with <strong>N </strong>(<strong>N</strong> &lt;= 100 000) and <strong>C</strong> (<strong>C</strong> &lt;= 100 000). After that you'll be given <strong>C </strong>commands in the format as mentioned above. 1 &lt;= <strong>p</strong>, <strong>q</strong> &lt;= <strong>N</strong> and 1 &lt;= <strong>v</strong> &lt;= 10^7.</p>
<h3>Output</h3>
<p>Print the answers of the queries.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1<br>8 6<br>0 2 4 26<br>0 4 8 80<br>0 4 5 20<br>1 8 8 <br>0 5 7 14<br>1 4 8<br><br><strong>Output:</strong><br>80<br>508</pre>