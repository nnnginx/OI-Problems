<p>The whole world is crazy about subset sum. We define subset sum as sum of all subparts. A subpart is a number which is obtained by erasing certain digits and arranging the remaining numbers in the same order. You have to calculate the subset sum of the given number. Since the number can be very large return the subset sum modulo <strong>m</strong>.</p>
<p>For example if the number is 1357, then the various subparts are 1, 3, 5, 7, 13, 15, 17, 35, 37, 57, 137, 135, 157, 357, 1357 .</p>
<h3>Input</h3>
<p>First line contains <strong>T</strong>(1<strong>&nbsp;</strong>¡Ü&nbsp;<strong>T</strong>&nbsp;¡Ü&nbsp;50)&nbsp;denoting the number of test cases.</p>
<p>Next T lines containing two numbers&nbsp;<strong>n</strong>(0 &lt;&nbsp;<strong>n</strong>&nbsp;&lt; 10<sup>1000</sup>) and <strong>m</strong>(1 &lt;&nbsp;<strong>m</strong>&nbsp;&lt; 10<sup>9</sup>).</p>
<h3>Output</h3>
<p>Print the subset sum modulo <strong>m</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>6</pre>
<pre>111 9</pre>
<pre>111 200</pre>
<pre>456 9</pre>
<pre>456 1000</pre>
<pre>1357 1000</pre>
<pre>1357 5000</pre>
<pre><strong>Output:</strong></pre>
<pre>3</pre>
<pre>147</pre>
<pre>6</pre>
<pre>618</pre>
<pre>333</pre>
<pre>2333</pre>
<p>&nbsp;</p>
<p><span style="color: #339966;"><span style="color: #339966;"><strong><span style="text-decoration: underline;">Time Limit ¡Ö 2*(My Python 3 Program Top Speed)</span></strong></span></span></p>
<p>&nbsp;</p>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>