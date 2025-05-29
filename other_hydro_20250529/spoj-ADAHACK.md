<p>Ada the Ladybug's crush Bumblebee Blazewan has a secret diary. Ada wants to read it to see, whether he loves her too. Sadly, the diary is locked with some very strong cipher so she can't read it.</p>
<p>She asked you for help. Unfortunately, you are not able to break through. Yet you observed, that the key generated in the cipher is generated in following way <strong>X<sub>i+1</sub>=(aX<sub>i</sub>+b) mod (10<sup>11</sup>+3)</strong>. You was able to find out first six <strong>X<sub>i</sub></strong>'s. Predicting next will help you to get through - can you do it?</p>
<h3>Input</h3>
<p>There will be no more than <strong>10<sup>5</sup></strong> test-cases.</p>
<p>Each test-case consists of line containing 6 integers <strong>0 ¡Ü     X<sub>i</sub> &lt; 10<sup>11</sup>+3</strong> (<strong>1 ¡Ü i ¡Ü 6</strong>)</p>
<h3>Output</h3>
<p>For each test-case print <strong>X<sub>7</sub></strong> (modulo 100000000003).</p>
<h3>Example Input</h3>
<pre>2 10 34 106 322 970
2 4 4 4 4 4
2 11 47 191 767 3071
0 0 0 0 0 0
2 8 32 128 512 2048
</pre>
<h3>Example Output</h3>
<pre>2914
4
12287
0
8192
</pre>
<h3>Possible setting</h3>
<pre>a=3, b=4, X<sub>1</sub>=2
a=0, b=4, X<sub>1</sub>=2
a=4, b=3, X<sub>1</sub>=2
a=2, b=0, X<sub>1</sub>=0
a=4, b=0, X<sub>1</sub>=2
</pre>