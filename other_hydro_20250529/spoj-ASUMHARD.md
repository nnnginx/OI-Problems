<p>f(n) is defined as: f(n) = 1<sup>k</sup>+2<sup>k</sup>+3<sup>k</sup>+...+n<sup>k</sup>, so it is the sum of the k-th power of all natural numbers up to n.</p>
<p>In this problem you are about to compute,</p>
<p>f(1) + f(2) + f(3) + ... + f(n)</p>
<h3>Input</h3>
<p>The first line is an integer&nbsp;<strong>T</strong>(1 ¡Ü&nbsp;<strong>T</strong>&nbsp;¡Ü 54,321), denoting the number of test cases. Then,&nbsp;<strong>T</strong>&nbsp;test cases follow.</p>
<p>For each test case, there are two integers&nbsp;<strong>n</strong>(1 ¡Ü&nbsp;<strong>n</strong>&nbsp;¡Ü 123,456,789) and <strong>k</strong>(0 ¡Ü <strong>k</strong><strong>&nbsp;</strong>¡Ü&nbsp;321) written in one line, separated by space.</p>
<h3>Output</h3>
<p>For each test case output the result of the summatory function described above.</p>
<p>Since this number could be very large, output the answer modulo 1,234,567,891.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5<br>2 3<br>10 3<br>3 3<br>100 0<br>100 1

<strong>Output:</strong>
10<br>7942<br>46<br>5050<br>171700</pre>
<p style="text-align: center;"><strong><span style="font-size: small;">Warning: A naive algorithm may not run in time</span></strong></p>
<p>&nbsp;</p>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>