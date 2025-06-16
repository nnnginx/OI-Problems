<p>For every given number n we define x(n) as distance from n to the first number after n in form of 99...99. For example x(100)=899, x(45)=54, etc. Given several n numbers you have to find the Z<sub>p</sub>, where x(n)<span style="color: #000020; font-size: 13px; background-color: #f6f9e0;">กิ</span>n mod p.</p>
<h3>Input</h3>
<p>First line of input icontains one number T (T&lt;20) - the number of test cases. In each of the next T lines contains one number each to represent n (0&lt;n&lt;30000000).</p>
<h3>Output</h3>
<p>In each line you have to write one number - the least p&gt;1 that x(n)<span style="color: #000020; font-size: 13px; background-color: #f6f9e0;">กิ</span>n mod p. If there is no such p the line should contain -1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>234</pre>
<pre>5

<strong>Output:</strong>
3
</pre>
<pre>-1</pre>
<pre>Explanation:</pre>
<pre>x(234)=765. 765 mod 3=0, 234 mod 3=0 =&gt; 765<span style="color: #000020; font-size: 13px; background-color: #f6f9e0;">กิ</span>234 mod 3</pre>