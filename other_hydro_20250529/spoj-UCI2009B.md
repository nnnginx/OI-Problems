<p style="text-align: justify;">We all got too excited when we learned (A + B)^2 = A^2 + 2AB + B^2. After solving this problem, maybe you could get even more excited because you will have to calculate (A + B)^N, where (0 &lt;= N &lt;= 1000).</p>
<p style="text-align: justify;">Follow the rules below when giving the answer:</p>
<ol>
<li style="text-align: justify;">Consecutive terms must be separated by a '+' character.</li>
<li style="text-align: justify;">At the i-th term, A must be raised to N - i and B must be raised to i (0&lt;=i&lt;=N).</li>
<li style="text-align: justify;">Binomial coefficients must not be printed, print their prime factorization instead.</li>
<li style="text-align: justify;">Use '^' for exponentiation and 'x' for multiplication in step 3.</li>
<li style="text-align: justify;">Avoid the use of number 1 when possible.</li>
</ol>
<p style="text-align: justify;">See sample output for clarification.</p>
<h3>Input</h3>
<p style="text-align: justify;">Input starts with an integer T, representing the number of test cases (1&lt;=T&lt;=15). T lines follow, each one consisting of an integer N, (0&lt;=N&lt;=1000).</p>
<h3>Output</h3>
<p style="text-align: justify;">For each test case, print (A + B)^N, on a single line.</p>
<h3>Example</h3>
<pre style="text-align: justify;"><strong>Input:</strong><br>6<br>0<br>1<br>2<br>3<br>4<br>5<br><br><strong>Output:</strong><br>1<br>A+B<br>A^2+2xAB+B^2<br>A^3+3xA^2B+3xAB^2+B^3<br>A^4+2^2xA^3B+2x3xA^2B^2+2^2xAB^3+B^4<br>A^5+5xA^4B+2x5xA^3B^2+2x5xA^2B^3+5xAB^4+B^5<br><br><strong>Warning: Large output. Be careful with certain languages.</strong><br></pre>