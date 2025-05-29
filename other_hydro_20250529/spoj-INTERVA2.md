<p>Give you N ( 1 &lt;= N &lt;= 200000 ) intervals, represented as [A, B], for example , interval s represented as [As,Bs].</p>
<p>For two intervals s and t, we say S covered by T if&nbsp; At &lt;= As and Bs &lt;= Bt. Now my problem is easy, just tell me the question below: For each interval, how many intervals can cover it but not covered by it ?</p>
<h3>Input</h3>
<p align="left">The input contains multiple test cases. <br> For each test case, the first line is an integer N ( 1 &lt;= N &lt;= 200000 ), which is the number of intervals. Then come N lines, the i-th of which contains two integers: A<sub>i</sub> and Bi ( A<sub>i </sub>, B<sub>i </sub>will not exceed the 32-bit integer) specifying the two parameters described above.</p>
<h3>Output</h3>
<p align="left">For each test case, output one line containing n space-separated integers, the i-th of which specifying the number of intervals that can cover it but not covered by it.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input</strong><p>3</p><p>0 1</p><p>-1 2</p><p>-2 3</p><p>&nbsp;</p><p>2</p><p>0 1</p><p>0 1</p><strong>Output:</strong><br><p align="left">2 1 0</p><p align="left">0 0</p></pre>