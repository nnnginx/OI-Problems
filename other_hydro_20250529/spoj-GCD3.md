<p>Given N, M and K (1 &lt;= N, M &lt;= 100^200 and 1 &lt;= K &lt;= 16) which<br><br>N = a + b<br>M = a^2 + b^2 - (2^K - 2) * a * b<br><br>with a &gt; 0, b &gt; 0 and gcd(a, b) = 1.<br><br>Your task is to find gcd(N, M).</p>
<h3>Input</h3>
<p>The input file consists of several data sets. The first line contains<br>the number of data sets T (1 &lt;= T &lt;= 10000). The fallowing T lines<br>describe the data sets, one triple (N, M, K) for each.</p>
<h3>Output</h3>
<p>For each data test in the input write the gcd(N, M).</p>
<h3>Example</h3>
<pre><strong>Input:<br><br></strong>2<br>648570884104668119354133 420644191708310845403065233058235585438328857465 5<br>8017723549 59173349743176010825 9<br>
<strong>Output:<br><br></strong>1<br>1<br><hr><br>Note: For the first trio a = 648570884104668119354126 and b = 7.<br>For the second a = 8016478423 and b = 1245126.<br></pre>