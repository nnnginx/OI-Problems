<p>&nbsp;</p>
<p><strong> Problem description. </strong></p>
<p>The Fibonacci numbers defined  as <strong>f(n) = f(n-1) + f(n-2)</strong> where <strong>f0 = 0 </strong> and <strong>f1 = 1</strong>.&nbsp;</p>
<p><br> We define a function as follows  <strong>D(n,x) = x + x^2 + 2x^3 + 3x^4 + 5x^5 + 8x^6 +...+f(n)x^n </strong> <br> <br> Given two integers n and x, you need to compute <strong>D(n,x) </strong> since the output can be very large output the result modulo <strong>1000000007 (1e9+7) </strong>.</p>
<h3>Input</h3>
<p>Input description.</p>
<ul>
<li>The first line of the input contains an integer <strong>T</strong> denoting the number of test cases. <br> The description of <strong>T</strong> test cases follows.</li>
<li>The first line of each test case contains two integers <strong> n </strong> and <strong>x</strong> as described above. </li>
</ul>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Output description.</p>
<ul>
<li>For each test case, output <strong> D(n,x)%1000000007 </strong> in a seperate line.</li>
</ul>
<p>&nbsp;</p>
<h3>Constraints</h3>
<p>Should contain all the constraints on the input data that you may have. Format it like:</p>
<ul>
<li><strong>1</strong> ¡Ü <strong>T</strong> ¡Ü <strong>1000</strong></li>
<li><strong>0</strong> ¡Ü <strong>n</strong> ¡Ü <strong>10^15</strong></li>
<li><strong>0</strong> ¡Ü <strong>x</strong> ¡Ü <strong>10^15</strong></li>
</ul>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 
7 11

<strong>Output:</strong>
268357683
</pre>
<p>&nbsp;</p>
<h3>Explanation</h3>
<p><strong>D(7,11) = 11 + 11^2 + 2(11^3) + 3(11^4) + 5(11^5) + 8(11^6) + 13(11^7) = 268357683</strong></p>