<p>Problem Courtesy: Ovishek Paul</p>
<p>Department of CSE, SUST</p>
<p>Sylhet, Bangladesh.</p>
<p>.........................................................................................................</p>
<p>Bodi is a "hotash" programmer. Sometimes he writes some code that takes 2777778 hours!!!</p>
<p>Good programmers said Bodi to become efficient. But Bodi just can't be. So he writes another code of&nbsp; 2777778 hours! which is below -</p>
<p>&nbsp;</p>
<p>long long sum = 0;</p>
<p>&nbsp;</p>
<p>for(long long i = L; i&lt;=R; i++){</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sum += i % mod;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sum %= (10<sup>9</sup> + 7);</p>
<p>}</p>
<p>&nbsp;</p>
<p>here, 1 &lt;= L &lt;= R &lt;= 10<sup>18</sup> , 1 &lt;= mod &lt;= 10<sup>18</sup></p>
<p>&nbsp;</p>
<p>Now Bodi is here to you because Bodi recently have known that you are so efficient!!!</p>
<h3>Input</h3>
<p>First line will contain 3 integers L, R, and mod.</p>
<h3>Output</h3>
<p>Just print the final sum.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>4 5 6</p><strong>Output:</strong>
9</pre>
<pre><strong>Input:</strong>
<p>4 10 9</p><strong>Output:</strong>
31<p>&nbsp;</p></pre>