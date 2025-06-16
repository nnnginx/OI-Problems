<p>Operation bits - A new operation conducted by the secret team currently working on a project on security enhancement. Mr.Abay, the team head, has found a new pattern on the perfect squares. This can be used as a outer cover for his project as its securing power is low. So he assign you this problem to find the key based on the given conditions:</p>
<p>"An two adjacent perfect squares have their absolute difference as an odd number except when a and b are equal. Your task is to find the key which is deined as:&nbsp;</p>
<p><span style="white-space: pre;"> </span>key(a,b) where a and b are perfect squares is ( ( AND( absolute difference betwen every adjacent perfect squares in [a,b]) ) AND ( XOR( absolute difference betwen every adjacent perfect squares in [a,b]) ) )"</p>
<p>Find the key for the given inputs :)</p>
<h3>Input</h3>
<p>The input begins with a number T (1&lt;=T&lt;=1000) where T is the number of testcases.</p>
<p>T lines follow</p>
<p>Each line has two numbers a and b (0 &lt; a &lt;= b &lt;= 10^6)</p>
<p>It is assured that a and b are perfect squares.</p>
<h3>Output</h3>
<p>For each test case print the corresponding key&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>1 4</pre>
<pre>25 49</pre>
<pre><strong>Output:</strong>
3</pre>
<pre>0</pre>
<pre>for test case 1 we have key=(3)&amp;(3)=3</pre>