<p>Consider the congruence equation system as the following form:<br><br>x[1] = k1 x[p1] + b1 (mod 10007)<br>x[2] = k2 x[p2] + b2 (mod 10007)<br>...<br>x[n] = kn x[pn] + bn (mod 10007)<br><br>We will ask you to achieve some instructions as the following form:</p>
<ul>
<li>A i: Ask the current x[i]'s value. (or "-1" for no solution, "-2" for multiply solution.)</li>
<li>C i k p b: Modify the ith congruence equation to a new one.</li>
</ul>
<h3>Input</h3>
<p>The first two lines are N and Q.<br>Than following Q lines are the query above.</p>
<p>(.. N ¡Ü 30, 000, Q ¡Ü 100, 000 .. .)</p>
<h3>Output</h3>
<p>For each query, print the result.</p>
<h3>Example</h3>
<pre><strong>Input 1:</strong><br>5<br>2 2 1<br>2 3 2<br>2 4 3<br>2 5 4<br>2 3 5<br>5<br>A 1<br>A 2<br>C 5 3 1 1<br>A 4<br>A 5 </pre>
<pre><strong>Output 1:</strong><br>4276<br>7141<br>4256<br>2126<br><strong><br>Input 2:</strong><strong><br></strong>4<br>0 1 0<br>1 3 0<br>1 4 0<br>1 2 0<br>6<br>A 1<br>A 2<br>A 3<br>A 4<br>C 1 1 5 1<br>A 1<br><strong><br>Output 2:</strong><br>0<br>-2<br>-2<br>-2<br>-1<br><br></pre>