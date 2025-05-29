<p>As you might already know, Ada the Ladybug is a farmer. Beside fruit and vegetable, Ada grows flowers. At the moment she plans to go to a competition with her dahlias. The evaluation of bunch of dahlias is simple: Jury sorts all dahlias by the diameters of blooms and takes the maximal difference between any two adjacent dahlias. This will be the score.</p>
<p>The problems is that Ada's flowers are not in sorted order and she wants to know what score she would get if the passes all flowers to jury. To make job easier for you (or at least Ada hopes so), she created a formula which will give you the diameters of blooms (0 to N-1) in actual order: <strong>A<sub>i+1</sub>=(a*A<sub>i</sub>+b)%c</strong>.</p>
<h3>Input</h3>
<p>The first and the only line contains five integers (<strong>N,a,b,c,A<sub>0</sub></strong>): <strong> 2 ¡Ü N ¡Ü     4*10<sup>7</sup></strong>, the number of flowers, and <strong>0 ¡Ü a, b ¡Ü     10<sup>18</sup></strong>, <strong>1 ¡Ü c ¡Ü 10<sup>18</sup></strong>, <strong>0 ¡Ü     A<sub>0</sub> &lt; c</strong></p>
<h3>Output</h3>
<p>Output the maximum difference of elements (if they would be sorted).</p>
<h3>Example Input</h3>
<pre>10 2 3 31 7</pre>
<h3>Example Output</h3>
<pre>8
</pre>
<h3>Example Input</h3>
<pre>4 4 6 11 6
</pre>
<h3>Example Output</h3>
<pre>2
</pre>
<h3>Example Input</h3>
<pre>50 3 11 41 0
</pre>
<h3>Example Output</h3>
<pre>8
</pre>
<h3>Example Input</h3>
<pre>1000 666 777 1234567 11
</pre>
<h3>Example Output</h3>
<pre>10817
</pre>
<h3>Example Input</h3>
<pre>10000000 612 521 124578541254695 666666
</pre>
<h3>Example Output</h3>
<pre>230017823
</pre>