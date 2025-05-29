<p><a href="../../../users/tonyxty/">Lambda</a> checks primality in a weird way. He checks the following two conditions.</p>
<ul>
<li>All the digits of the number in the decimal system are primes or one, namely 1, 2, 3, 5 or 7.</li>
<li>It isn't a multiple of 2, 3, 5, 7, 11 or 47 (Why 47? I don't know).</li>
</ul>
<p>In order to estimate the accuracy of his approach, he asks you to calculate the number of decimal integers of a specific length that satisfy the conditions.</p>
<h3>Input</h3>
<p>The first and only line contains  an integer <em>n</em>, denoting the length of integers.</p>
<h3>Output</h3>
<p>The only line contains the answer <strong>modulo 9973</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1<br><br><strong>Output:</strong><br>1<br><br><strong>Input:</strong><br>2<br><br><strong>Output:</strong><br>8<br><br><strong>Input:</strong><br>4<br><br><strong>Output:</strong><br>182<br><br><strong>Input:</strong><br>1000000000<br><br><strong>Output:</strong><br>4589<br><br></pre>
<h3>Constraints</h3>
<p>1 &lt;= <em>n</em> &lt;= 10<sup>9</sup><br>In 50% of testcases, <em>n</em> &lt;= 100</p>
<p>Note: Data corrected and solutions rejudged. Sorry for inconvenience.</p>
<p><strong>Warning: A naive solution won't terminate in 30s. And be careful with certain languages.</strong></p>